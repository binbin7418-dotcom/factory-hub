# 总图 ATLAS（仓库 · 文件夹 · Skills 导航）

> 2026-11-02 建立。用途：任何东西「在哪、是干嘛的、找什么看哪里」先查这张图。规则：新建仓/新项目/新 skill 当天补进本图；项目每次更新连同 GitHub 备份一起更新（2026-11-02 用户下令）。
> 数字口径：仓库清单为 2026-11-02 GitHub API 实查（公开仓 39 个）；在售数以 PRODUCTS.md 与各线状态文件为准。

## 一、GitHub 仓库地图（binbin7418-dotcom）

### 中枢与门户（先看这里）
| 仓 | 是什么 | 找什么看哪 |
|---|---|---|
| factory-hub | 全线中枢：产品注册表、每日运营清单、总图 | PRODUCTS.md（注册表）、DAILY-OPS.md（每日清单）、ATLAS.md（本图） |
| binbin7418-dotcom.github.io | 根集合站：全部工具落地页门户 + GSC 验证文件 | 根目录 sitemap；验证文件 google313065ad0232e20b.html 勿删 |
| sku-ops-landing | SKU Operations Copilot 落地页（sku.vn-node.cc.cd） | index.html |

### 产品工具仓（每个 = 一个 Gumroad $29 工具：源码 + Actions 云构建 + docs/ 落地页）
在售 26：sheetfix、feedfix、audiofix、shopifycsvfix、listclean、silencecut、pagesmith-pdf、stampbatch、dupelens、contactfix、printready、imagebatch、qrbatch、dateshift、metascrub、audiobookspecfix、invoicebatch、statementsift、puzzlepress、mailmend、ledgerlink、deckshrink、stitchchart、codewordforge、redactready、formfillbatch。
不卖（仓保留）：epubfix（从未上架）、subtitlefix（已下架，引擎保留）。
找构建产物：仓内 Actions 的 build 工作流 artifact（双层 zip）；找落地页文案：docs/index.html。

### 服务与数据仓
| 仓 | 是什么 | 备注 |
|---|---|---|
| whatsapp-lead-receptionist | n8n 行业包共用引擎样品仓（12 节点，实测过） | 行业包 16 个在售的底座 |
| geoip-city-data | GeoIP 城市库数据仓（325 分片，DB-IP CC BY 4.0） | ✅ 2026-11-02 全量入库（API 核验 327/327、大小零差异）；v3 worker 已部署生产并线上 5 条验真全对（城市级已通） |
| page2md | 他早年的网页转 Markdown 工具（RapidAPI 第一款的源头） | 2026-03 后未更新 |

### 他本人的早期仓（非 Muse 产品线，不动）
AmazonReady（TS，2026-03）、vvhub（TS，Codex for OSS 申请材料）、XRSS（空仓）、RSSHub（fork，942MB）、binbin7418-xiaohongshu-mcp（2025 年，82MB）。

### 私有仓（公开 API 看不到，凭登记）
| 仓 | 是什么 | 状态 |
|---|---|---|
| wechat-miniapp-studio | 小程序三件（01 本官听你说 / 02 拍万物学英语 / 03 这单我报销），Codex 主跑 | 以仓内 docs/product-registry.md 为准 |
| video-product | PitchReel 引擎 2026-10-31 快照 | 已过期；当前版见 pitchreel 仓 |
| fashion-film-factory | 服装线资产（模特库 43 张 + README） | 2026-11-02 已落仓核验；knowledge 文档待补传 |
| skills-backup | 自有 skills + 外部技能索引备份（zip） | 2026-11-02 建成并经第二窗口复核（Private＋zip＋README 在列） |
| product-factory | 产品工厂备份：总表/第五批/n8n 包源码（zip） | 2026-11-02 建成并经第二窗口复核（Private＋zip＋README 在列） |
| rapidapi-sources | RapidAPI 全部 worker 源码备份（zip） | 2026-11-02 建成并经第二窗口复核（Private＋zip＋README 在列） |
| story-koubo | 故事实验备份：稿件/管线代码/报告（zip，不含母带与场景图） | 2026-11-02 建成并经第二窗口复核（Private＋zip＋README 在列） |
| pitchreel | PitchReel 引擎与网站源码备份（zip） | 2026-11-02 建成并经第二窗口复核（Private＋zip＋README 在列） |

## 二、本地工作区地图（~/workspace/）

| 文件夹 | 是什么 | 找什么看哪 |
|---|---|---|
| factory-hub | 中枢文档本地版 | PRODUCTS.md / DAILY-OPS.md / ATLAS.md |
| product-factory | 工具与 n8n 包的生产区 | 产品线总表.md；batch5/ 第五批交付物；n8n-packs/ 行业包（BATCH2-STATUS.md） |
| video-mcp | PitchReel 引擎 + 网站（主力一） | web/（站点与定价 PRICING-AND-LAUNCH.md、客服 SUPPORT.md、自测 SELFTEST-20261101.md）；GAPS.md 缺口表；tools/spotcheck.py 第二道闸 |
| fashion-film-factory | 服装线（主力二） | BLUEPRINT.md 蓝图；MODEL-BASE-PLAN.md 模特方案；models/ 模特库；knowledge/ 方法资产（姿势/气场/运镜/拉片） |
| story-koubo-experiment | 图文故事口播实验二 | remake-v2/ 起为新格式样片；稿件 EP01 苏轼 |
| goals/seo | 新词出海 SEO 站（引擎线） | site/（newkw.pages.dev 源码，10 页已上线） |
| rapidapi-batch* | RapidAPI 各批源站与 worker | batch3/geoip 含城市版 v2 worker 与数据暂存 |
| custom-skills | 自有 skills（9 个） | INDEX.md 总索引（触发场景+负样本） |
| external-skills | 外部 skills 实物库 | INDEX.md 逐卡登记（用途/许可/状态/路径） |
| research_notes | 全部调研报告存档 | 按日期目录：search-demand-20261101（选品）、history-sample-scout-20261101（选题）等 |
| cf-node | 自建 CF 代理节点 | .secrets.json（凭证级勿外传）；subscription-url.txt |
| user/files | 他发来的原始材料 | 小程序全套、图包原图（归档后以各项目目录为准） |

## 三、Skills 总表

### 自有 skills（9 个，详见 custom-skills/INDEX.md）
| Skill | 干嘛的 | 什么时候用 |
|---|---|---|
| video-production | 视频生产统一管线（MCP+双闸 QA） | 做/改/质检自有视频产品时 |
| fiverr-seller-ops | Fiverr 卖家运营手册（visionwei） | 巡检 gig、回客户、改 gig 时 |
| platform_listing_capacity_check | 上架前先数平台名额 | 给任何平台开发/上架新品之前 |
| cf-global-edge-node | CF 边缘节点搭建与排障 | 建/修个人代理节点时 |
| visitor_safe_service_checks | 以访客身份验服务真活着 | 网站上线、换机恢复、巡检时 |
| credential_ask_discipline | 凭证与本人验证只集中问一次 | 长流程多站点登录之前 |
| local-verify-before-assert | 下结论前先查一手来源 | 写事实断言、引案例数字之前 |
| opire-bounty | Opire 赏金打法（该线已淘汰，仅存档） | 不再执行 |
| recovered-skill-notes | 旧笔记归档（retired） | 仅查旧资料时 |

系统 skills（/opt/muse/skills/，平台自带）：购物、旅行、邮件、日程、文档、媒体生成等通用能力，需要时按名调用，不属自有资产。

### 外部 skills（实物在 external-skills/，逐卡见其 INDEX.md）
- 工具型（可直接调用）：女娲 nuwa（风格蒸馏标准工具）、GSAP 官方（动效规范，只学不引本体）、image-prompt-reverse（图片反推提示词）、rtmlib/DWPose（姿势提取，本机跑通）、Higgsfield 官方 9 个（只学 MCP 与工作流，不花它的钱）。
- 视频方法库：HyperFrames（渲染引擎上游）、seedance2、motion-prompt 两仓（运镜词库，分工不重复）、cinematic-video-prompt、explainer-video-cn（科普 rubric）、papercut-explainer（分镜纪律）、arabic-motion-graphics（节奏数字）、story-studio（故事工坊，语料只学结构严禁洗稿）、image-story-video-wizard、animate、vibe-knowledge-film、pixelfx、huashu-motion、mg-styles-15、digital-human-koubo（数字人底座，路线搁置中）。
- 审美与建站：Motionsites（只学方法，其推广植入不执行）。
- 服装线方法源：lookbook 四仓（只学方法，图库一张不搬）、editorial-allure-prompting、试穿代码库（FASHN/Leffa 等，待 GPU）、Fashion-AI（爆款基因库思想）、LinkFox 官方样本（ShareURL 常驻规则不采用）。

## 四、待学习清单（排队消化，学完划掉并注明落点）
1. 服装线打包成正式自有 skill（11+ 件知识文档已有，缺 SKILL.md 三件套）——服装线开跑前完成。
2. story-studio 剪映草稿导出适配（plan 字段映射一次，生成后须在剪映打开验收）。
3. Skills 检索复测（目录刷新后重跑第 9 条「查仓库星数」负样本）。
4. HyperFrames 0.8.223 整片重渲升级判定（现锁 0.8.78）；faster-whisper 接入判定（每周学习轮次跟进）。
5. 女娲蒸馏法落到服装线人物风格与故事线叙事风格各一次实作。
6. lemo-opuscar 风格语法消化（2026-11-02 入库 external-skills/lemo-opuscar）：ink-wash 并入故事线 FORMAT-STANDARD 画风锁定章（故事线定版时）；whiteboard/dataviz 等对位科普模板语言时再取。

## 五、排查清单（未关的问题，关一个划一个）
- [x] GeoIP 数据仓余 277 文件上传 + v3 worker 部署 + 线上 5 条验真。（2026-11-02 02:12 完工，见 memory/2026-11-02.md）
- [ ] newkw 站 GSC 提交 + IndexNow（SEO 计时未开始，最急）。
- [ ] factory-hub 的 PRODUCTS.md 同步 GitHub（本地已新、GitHub 侧停在 10-29）。
- [ ] 根集合站 sitemap 补入新工具落地页。
- [ ] video-product 私有仓用 video-mcp 当前源码更新（排除缓存与成片大文件）。
- [ ] story-koubo-experiment、custom-skills、external-skills 建备份仓。
- [ ] PitchReel Standard 时长文案口径（实测 83s vs 标称 ≈60s）微调。
- [ ] spotcheck 的 asr_numbers 补阿拉伯数字等价形（中文片误报）。
- [ ] 邀请码 samseah 池计数读不到、夜影小窝 DNS 间歇不可达（监测缺口，非下架证据）。
- [ ] Danish_Koul_14 客户对话静默（等回复，不主动追第二封）。

## 六、找东西速查
- 某个产品在没在卖、卖多少钱 → factory-hub/PRODUCTS.md
- 今天该干什么 → factory-hub/DAILY-OPS.md
- 仓在哪、文件在哪 → 本图一、二节
- 某个能力怎么做 → custom-skills/INDEX.md（自有）或 external-skills/INDEX.md（外部）
- 某个结论的证据 → research_notes/ 对应日期报告
- 某条线的规矩 → ~/AGENTS.md + 对应 GOAL.md
