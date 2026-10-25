# 产品注册表（PRODUCTS）

状态口径：在售 = 公开页可购买且经亲自核验；建成待上架 = 仓库/构建/落地页全部完成，只差最后上架动作。收入一律以真实到账为准，当前全部为 0。

## 一、Gumroad 工具线（目标 100，当前 11）

统一形态：本地运行（数据不出本机）→ 检查/修复 → 复检出报告；Windows 一键包；$29 一次性。落地页统一在 binbin7418-dotcom.github.io/<产品名小写>/，源码仓 github.com/binbin7418-dotcom/<产品名小写>。

| # | 产品 | 一句话 | 状态 | Gumroad / 种子验收摘要 |
|---|---|---|---|---|
| 0 | SheetFix（样板） | Excel 审计修复 | 在售 | binbinster.gumroad.com/l/sheetfix-excel-audit；13 条缺陷修 5、连带消除共 8、剩 5 判断级、新引入 0 |
| 1 | FeedFix | Google Shopping Feed 修复 | 在售 | /l/feedfix-google-shopping-feed-repair；12 商品 21 问题修 10、剩 11（5 阻断）、新引入 0 |
| 2 | EPUBFix | EPUB 发布前检查修复 | 在售 | /l/epubfix-epub-check-repair；种子 6 缺陷结构类修 2、剩 3（2 阻断） |
| 3 | AudioFix | 播客响度标准化+剪静音 | 在售 | /l/audiofix-podcast-loudness；-29.9→-15.9 LUFS、剪静音 4.2s、PASS |
| 4 | ShopifyCsvFix | Shopify 商品 CSV 修复 | 在售 | /l/shopifycsvfix-product-csv-repair；5 行 14 问题修 11、剩 3 阻断 |
| 5 | ListClean | 邮箱列表本地清洗 | 在售 | /l/listclean-local-email-list-cleaner；12 行→干净 7、去重 1、无效拒 2、一次性域名 1 |
| 6 | SilenceCut | 口播视频剪静音/气口 | 在售 | /l/silencecut-talking-head-silence-remover；9s→6.5s、静音 3.0→0.4s（边界：删口水词需转写，文案已明示） |
| 7 | SubtitleFix | SRT/VTT 字幕修复 | 在售 | /l/subtitlefix-srt-vtt-repair；分隔符/重叠/零时长/空条共 4 修、复检 PASS |
| 8 | PrintReady | KDP 印刷 PDF 预检修复 | 建成待上架 | slug: printready-kdp-pdf-precheck；5 页种子书 2 处结构修复、复检如实报 3 阻断；卡点：安装包回传通道停摆，cron 自动接管中 |
| 9 | ImageBatch | 卖家图片批量预处理 | 建成待上架 | slug: imagebatch-marketplace-photo-prep；EXIF 摆正/限尺寸/剥元数据/整夹小 67%；同上卡点 |
| 10 | QRBatch | CSV 批量二维码+打印版 | 建成待上架 | slug: qrbatch-bulk-qr-print-sheets；5 行→4 码、2 警告、A4 300dpi 打印版；同上卡点 |

另有旧产品：SKU Operations Copilot（$19，在售，0 销量，binbinster.gumroad.com/l/shopify-sku-ops-copilot，落地页 sku.vn-node.cc.cd）。

## 二、RapidAPI 线（目标 100，当前 12）

统一：免费层 + PRO/ULTRA 订阅；源站 Cloudflare Pages；网关实测全过；真实订阅 0。

| 批次 | API | 定价（PRO 起） | 源站目录 |
|---|---|---|---|
| 一 | Page2MD、QRGen、MetaExtract、Feed2JSON、MD2HTML、TextLens | $15/$49 档 | rapidapi-batch/、rapidapi-first-api/（page2md） |
| 二 | EmailCheck、CryptoPulse、WeatherNow、FXRates、PhoneCheck、DomainIntel | PRO $5–10 | rapidapi-batch2/ |

搜索可见性（2026-10-25）：PhoneCheck 约 39 位、CryptoPulse 约 68 位、WeatherNow 约 81 位，其余暂未进前 100——新列表常态，靠调用量爬升。

## 三、n8n 线（目标 100 个模板/服务资产，当前 10 个产品位：8 个已落地、2 个进行中）

- Fiverr gig 在架 4 个：主 gig（n8n 自动化代建 $90/$140/$290）、WhatsApp 自动回复+线索打分（$90/$190/$390）、修复/诊断、Looker Studio 报表；均 3 图满库。卖家 @visionwei。
- 待发 2 个（被新卖家 4 个上限挡住）：AI 客服智能体（$90/$240/$490）、线索获取+打分（$90/$190/$390）；文案与图在 ~/workspace/接单雷达/ 对应目录。
- Gumroad 行业包 3 个（2026-10-25 新增，$49 一次性，含设置答疑；引擎与 Fiverr/社区样品同一套，出厂文件逐字提取验收，每包 7/7 全过；本地 ~/workspace/product-factory/n8n-packs/）：
  - 地产版 WhatsApp Lead Receptionist for Real Estate Agents：在售 binbinster.gumroad.com/l/whatsapp-receptionist-real-estate（热线索实测 100 分）
  - 汽修版 WhatsApp Lead Receptionist for Auto Repair Shops：在售 /l/whatsapp-receptionist-auto-repair（热线索实测 85 分）
  - 美容版 WhatsApp Lead Receptionist for Beauty Salons & Spas：建成待上架（热线索实测 95 分；2026-10-25 撞 Gumroad 每日新建 10 个上限，已排 10-26 上午自动补上架，slug: whatsapp-receptionist-beauty-salon）
- n8n 官方模板库：第 10 个产品位。提交路径已摸清（n8n.io/workflows → Creator hub → creators.n8n.io），但保险库 n8n.io 登录被创作者门户拒绝（Login error — Unauthorized），待用户更新该登录后再提交；社区展示帖（待平台审批）暂代官方渠道占位。
- 样品资产：WhatsApp Lead Receptionist 工作流（仓 github.com/binbin7418-dotcom/whatsapp-lead-receptionist；社区展示帖待平台审批）；线索打分 demo 实测版（11 用例全过，Hot ≥70 / Warm ≥45）。
- 社区应征：累计 6 封（邮箱/私信），截至 2026-10-25 暂无回复，巡检持续盯。

## 维护记录

- 2026-10-25：中枢仓建立；11 个落地页全部上线核验；3 个产品等安装包回传后由 cron `gumroad-final3-watch` 自动上架。
- 2026-10-25 下午：n8n 线扩到 10 个产品位——Gumroad 行业包 3 个建成并逐包验收（地产/汽修已在售，美容待次日补上架）；n8n 模板库提交卡在创作者门户登录，路径已记录待办。
