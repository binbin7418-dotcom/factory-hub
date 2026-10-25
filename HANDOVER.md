# 交接手册（HANDOVER）

接手者（人或智能体）按本手册可独立完成：开发 → 测试 → 构建 → 上架 → 核验 → 维护。所有配方均为 2026-10-25 实测有效的做法；与本手册冲突的「据说成功了」一律以核验纪律为准。

## 0. 核验纪律（最重要，先读）

- 浏览器代理/子任务的完成回执**真假混杂**：run ID、哈希、文件大小、截图描述都可能编造。**唯一可信的核验**是接手者亲自做：
  - 仓库状态：GitHub 公开 API `api.github.com/repos/binbin7418-dotcom/<repo>/git/trees/main?recursive=1`（全树+大小）、`/commits`、`/actions/runs`。注意页面缓存：重复打开同一 URL 会返回旧快照，核验要换未拉过的 URL 变体（改 per_page、加 ?ref=main）。
  - 落地页/产品页：亲自抓取公开 URL 看渲染内容。
  - 安装包：本地解包，确认内含 `<产品名>/<产品名>.exe` 且 zip 完整性通过，才算「包可用」。
- 建仓/补文件**分批派工**（每批 ≤2 个文件），每批后 API 核验再继续。
- 数字纪律：销量、收入、评价只认平台后台真实数据；文案只写种子验收的实测数字。

## 1. 账号与资产（密码一律在保险库，本文不写明文）

| 资产 | 标识 | 备注 |
|---|---|---|
| GitHub | binbin7418-dotcom | 用 Google 会话登录；云端浏览器新窗口可能无会话，复用已有登录窗口 |
| 运营邮箱 | binbin7418@gmail.com | 注册/运营默认邮箱；邮箱验证码自行去 Gmail 取 |
| Gumroad | binbinster.gumroad.com | 国家 China，PayPal 收款，最低打款 $100、周结 |
| RapidAPI | 账号 Bin Bin | GitHub 会话登录；收款 PayPal 1060207169@qq.com，抽成 25%，月结 |
| Fiverr | @visionwei（Display name: Bin W） | ID 验证与税表已完成（非美身份 compliant）；收款走 Payoneer |
| Cloudflare | muse-deploy 账户令牌 | 部署 Pages 用；令牌值不落任何文件 |

硬规矩（血泪教训，违反必出事）：
- 带登录态的浏览器任务**禁止更换浏览器环境**（换环境必丢登录态）。
- 登录优先用浏览器已有会话，其次保险库已存登录试一次；两条不通就停下报告，**不向用户弹新凭证卡、不二次索取凭证**。
- Google 在云端触发「验证身份」时只有通行密钥一条路（需蓝牙近距离，云端必失败）——这类会话过期后不要反复试，攒到其他时机。
- 给浏览器代理派活时，文案全文直接写进任务文本（它读不到授权文件的文本内容，只能用授权文件做上传）。

## 2. Gumroad 工具线配方（每个新产品照抄）

1. 本地开发（目录 `~/workspace/<产品小写>-product/`）：引擎 + GUI + PyInstaller spec + 《产品文案.md》（名称/描述/slug 定稿，描述含 VERIFIED, NOT VIBES 实测节）。
2. 种子验收：按 PIPELINE 第三关跑，数字记进文案与 README。
3. 建 GitHub 仓（公开）：经浏览器网页 UI 逐文件创建（VM 终端无 GitHub 推送权限）：引擎、gui.py、spec、`.github/workflows/build-windows.yml`（PyInstaller 云构建）、README.md、docs/index.html（落地页）。
4. 启用 Pages：Settings → Pages → Deploy from a branch → main → /docs（该页偶发要求重新验证登录，换窗口重试，不要向用户要密码）。
5. 等 Actions 构建成功 → 下载 artifact（外层 zip 内含内层 -Windows.zip）→ 本地验包 → 内层改名存为 `<产品名>-Windows-package.zip`。
6. Gumroad 上架：新建产品 → 名称/价格 $29 一次性/描述全文粘贴（分两段粘，粘后核对全文）→ 上传内容文件（等 Files 区出现真实文件名+非零大小才发布）→ URL slug 按文案 → 发布后打开公开页核验价格与购买按钮。
7. 更新 PRODUCTS.md 与产品线总表。

已知坑：浏览器下载同步（browser_downloads）可能停摆——包下载到浏览器侧但落不了本地盘，此时 Gumroad 浏览器直传也走不通（文件选择器够不到浏览器下载目录），只能等同步恢复；已为最后 3 个产品设 cron `gumroad-final3-watch` 每 30 分钟自动检查并接管上架。

## 3. RapidAPI 线配方

1. 源站：单文件 Worker 逻辑用 esbuild 打成 `_worker.js`，部署到 Cloudflare Pages 高级模式（该账号独立 Workers 全部报错 1101，不可用）；wrangler 用 muse-deploy 令牌部署。源站目录：第一批 `~/workspace/rapidapi-batch/`、page2md 在 `~/workspace/rapidapi-first-api/`、第二批 `~/workspace/rapidapi-batch2/`。
2. Hub 上架：Provider 后台建 API → 绑源站 endpoint → 定价三档（免费层引流 + PRO + ULTRA）→ 公开前用网关地址实测每个 endpoint 返回正确。
3. 可发现性：标题/简介带用户会搜的原词；新 API 搜索排名靠调用量爬升，属正常冷启动。
4. 维护：看 Hub 数据（订阅/调用/错误率）决定死磕哪个；源站改版后必须重测网关。

## 4. n8n 线配方

- Fiverr：新卖家 Active gig 上限 **4 个**。编辑描述走 Manage Gigs → Edit → 点聚焦 contenteditable 编辑器 → 用 fill 按单行分块追加；FAQ 答案上限 300 字符、套餐描述上限 100 字符；图库只有第 1 槽能被浏览器可靠上传，第 2/3 张图需人工补。PerimeterX 按住验证在高强度操作后需隔夜冷却，不要换环境硬试。
- 获客：n8n 社区 Jobs 帖的公开回复已被版主关闭，应征走帖内邮箱/申请表/私信三渠道（用户已批准全用）；每日巡检 cron `n8n-gig-daily-ops` 在跑。
- 交付底座：Zie619/n8n-workflows（MIT）在 `~/workspace/底座开发/base-n8n-workflows/`，署名与 LICENSE 必须保留；demo 用实测版工作流 JSON（11 条用例全过）。

## 5. 本地工作目录地图（~/workspace/）

- 产品工厂总表：`product-factory/产品线总表.md`
- Gumroad 各产品：`sheet-product/ feed-product/ epub-product/ audio-product/ shopifycsv-product/ listclean-product/ silencecut-product/ subtitle-product/ printready-product/ imagebatch-product/ qrbatch-product/`
- RapidAPI：`rapidapi-first-api/ rapidapi-batch/ rapidapi-batch2/`
- n8n 生意线：`接单雷达/`（文案包、demo）、`底座开发/`
- 中枢文档本地副本：`factory-hub/`（与 GitHub 中枢仓同内容）

## 6. 运维节奏

- 每日：`n8n-gig-daily-ops`、`daily-project-scout`（约 09:52）自动跑；心跳巡检盯 Fiverr 订单/客户消息、n8n 社区私信、Etsy 外联回复。
- 有真实订单/客户回复/第一笔到账：第一时间通知用户。其余攒批汇报，夜间（23:00–09:00）不打扰。
- 每季度：复查各平台政策、价格、竞品动向，更新 PIPELINE 与本手册。
