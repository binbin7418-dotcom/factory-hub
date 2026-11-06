# 资产总表 ASSET-INDEX（2026-11-07 首版）

维护规则（2026-11-07 Vision 下令，凌晨 03:00 固定功课）：每一行一个产品/项目——名称、所属线、在线状态、GitHub 仓（链接，无仓写「无仓」及原因）、仓内与本地是否一致、最近核对日。总表是长期记忆与次日计划的依据，必须与现实一致，不许凭印象写；未核对的写「未核对」并注明须补查什么，不写推测。
分类依据：~/workspace/factory-hub/ASSET-MAP.md（2026-11-07 定版）。核对方法：GitHub API 公开仓 trees/文件大小对照；私有仓只能经浏览器已登录会话复核，API 看不到。
最近核对日：2026-11-07（首版；未逐项核对的行以「未核对」标注）。

## A. 产品独立仓（公开——卖货需要）

| 产品/项目 | 所属线 | 在线状态 | GitHub 仓 | 仓内与本地是否一致 | 最近核对日 |
|---|---|---|---|---|---|
| PitchReel 简历视频站 | PitchReel | 在线：https://pitchreel.newkwlab.com/ health 200 ok（2026-11-07 03:0x 复核） | 私有仓 pitchreel（源码备份仓，zip 形态；ASSET-MAP 写「公开」与现实不符，以现实为准：私有） | 未核对（私有仓，API 看不到；本地 video-mcp 21GB 含 data/orders/demo，快照须走 zip 路线） | 2026-11-07（仅在线状态；仓内容未核） |
| SnapDuo 趋势梗合照站 | SnapDuo | 在线：https://api.newkwlab.com/duo/ 200（26,117 B，2026-11-07 03:0x 复核）；/duo/health ok | 公开仓 https://github.com/binbin7418-dotcom/snapduo | 一致：仓内 9 文件与本地对应文件大小逐一对上；唯一差异是 README.md 仅仓内有（170 B，本地无同名文件，不算缺口） | 2026-11-07 |
| Starlight Stories 个性化故事书 | 故事书 | 在线：https://api.newkwlab.com/book/ 200（42,438 B）；/book/health ok | 公开仓 https://github.com/binbin7418-dotcom/storybook-site | 一致：仓内 7 文件与本地对应文件大小逐一对上；媒体文件按规矩未入仓 | 2026-11-07 |
| PaperStage 纸片动画 | PaperStage | 在线：https://api.newkwlab.com/clip/ 200（44,710 B）；/clip/health ok | 公开仓 https://github.com/binbin7418-dotcom/paperstage-site | 一致：仓内 6 文件与本地对应文件大小逐一对上；媒体文件（样片/场景图）按规矩未入仓 | 2026-11-07 |
| Fashion Citywalk 纸片时尚 | PaperStage/时尚 | 在线：https://api.newkwlab.com/walk/ 200（64,486 B，六款版）；/walk/health ok | 无仓——首批欠账第 1 笔，今晚建仓（公开仓 fashionwalk-site） | 不一致：本地 ~/workspace/fashionwalk-site/ 42MB（含 8 支样片 mp4，媒体不进仓）；待传文本文件 10 个（README.md、web/app.py、web/site/index.html、web/site/llms.txt、fashion_config.example.json、deploy/README.md、SPEC.md、BUILD-REPORT.md、REDESIGN.md、SWAP-REPORT.md），真实配置 fashion_config.json 与 .bak-precut 备份不传 | 2026-11-07 |
| 免费 AI 网关 | 网关 | 在线：EC2 悉尼 3.106.189.249，/health、/tts、/ocr、/chat、/vision 2026-11-04 公网复测全通 | 公开仓 https://github.com/binbin7418-dotcom/free-ai-gateway（2026-11-04 更新） | 未核对（本地对照未查） | 未核对 |
| agent-catalog 机器可读产品目录 | Agent 目录 | 在线：https://binbin7418-dotcom.github.io/agent-catalog/ 200（250,422 B，与仓内一致）；catalog.json 在线 315,881 B，与仓内/本地根目录一致 | 公开仓 https://github.com/binbin7418-dotcom/agent-catalog | 一致（以本地根目录 catalog.json 315,881 B 为准；deploy-v1/ 为 11-03 旧构建、文件更小，不作对照基准） | 2026-11-07 |
| HTML 演示模板包（20 套） | PPT 模板 | 未上架（Gumroad 上架待定价拍板） | 公开仓 https://github.com/binbin7418-dotcom/html-slides-template-pack | 不一致：仓落后于本地——仓内仅 44 文件（首批 3 套）；本地 20 套已齐（289 文件），最终 zip html-slides-template-pack.zip 16.3MB/410 文件已于 11-06 14:43 打好，增量清单 html-slides-upload-manifest-v2.txt 已备；约 300 个新增文件待分批上传（多夜量，不在一夜硬搬） | 2026-11-07 |
| 新词卖货站三站 | SEO/新词 | 在线：terra/genie4/kling4.newkwlab.com https 200（11-06 复核） | 公开仓 terra-cost-calculator、genie4-prompt-builder、kling4-prompt-builder（均 2026-11-06 更新，Clarity＋Bing 验证标签已入） | 未核对（本地对照未查） | 未核对 |
| Gumroad 单品工具仓（37 个） | 产品工厂 | 在售 42 个工具类（见 PROGRESS）；各仓落地页在 docs/ | 公开仓：sheetfix、feedfix、audiofix、shopifycsvfix、listclean、silencecut、pagesmith-pdf、stampbatch、dupelens、contactfix、printready、imagebatch、qrbatch、dateshift、metascrub、audiobookspecfix、invoicebatch、statementsift、puzzlepress、mailmend、ledgerlink、deckshrink、stitchchart、codewordforge、redactready、formfillbatch、crosswordpress、logicgridpress、sudokupress、qifsift、woocsvfix、mathsheetpress、iifsift、calcudokupress、futoshikipress、mosaiccolorpress、shikakupress、cryptogrampress、queenspress、binairopress、mazepress（37 个，不含 epubfix/subtitlefix 两个不卖仓） | 存在性已核（API 清单 64 公开仓内均在列，最近更新 2026-10-25–11-04）；逐仓 tree 与本地对照未核对，分批补 | 2026-11-07（仅存在性） |
| SKU Ops 落地页 | 产品工厂 | 在线：sku.vn-node.cc.cd | 公开仓 sku-ops-landing | 未核对 | 未核对 |
| GeoIP 城市库数据仓 | RapidAPI 数据 | 在线：v3 worker 已部署生产（11-02 线上 5 条验真全对） | 公开仓 geoip-city-data（325 分片，2026-11-02 API 核验 327/327） | 2026-11-02 已核一致；此后未变，未重核 | 2026-11-02 |
| WhatsApp Lead Receptionist 引擎 | n8n 底座 | 样品仓（n8n 行业包 20 个的底座） | 公开仓 whatsapp-lead-receptionist | 未核对 | 未核对 |
| page2md | 早期工具 | 未在售（他早年作品，2026-03 后未更新） | 公开仓 page2md | 未核对 | 未核对 |

## B. 集合仓（ASSET-MAP 规划；现实：多为私有备份仓，未按规划建集合仓）

| 产品/项目 | 所属线 | 在线状态 | GitHub 仓 | 仓内与本地是否一致 | 最近核对日 |
|---|---|---|---|---|---|
| RapidAPI 服务源码备份 | RapidAPI | 83 个在售（11-06 全量核对） | 私有仓 rapidapi-sources（zip 备份） | 未核对（私有仓，API 看不到）；本地 ~/workspace/backups-staging/rapidapi/ 有 batch1–15＋first-api.zip；修复快照 rapidapi-repair-20261106.zip（477,590 B，含 5 品修复后源码＋dist）已备未传——首批欠账第 2 笔，今晚传 | 2026-11-07（仅本地备料） |
| 产品工厂备份 | 产品工厂 | — | 私有仓 product-factory（总表/第五批/n8n 包源码 zip，2026-11-02 第二窗口复核） | 未核对（此后改动未追踪） | 2026-11-02 |
| skills 备份 | 能力资产 | — | 私有仓 skills-backup（2026-11-02 建成复核） | 不一致：lemo-opuscar 112MB 全仓未入（超网页单文件 25MB 上限，待瘦身方案）；2026-11-05 新入库 clone-website、motionsites-web-builder 未进备份 | 2026-11-07（缺口已知） |
| 故事实验备份 | 故事线 | 故事线已暂停 | 私有仓 story-koubo（2026-11-02 建成复核） | 未核对（此后改动未追踪） | 2026-11-02 |
| 搞笑动画线资产 | 动画线（已停） | 已停，资产留档 | 私有仓 comedy-line（5 包，2026-11-03 根目录亲核；EP02 成片 2026-11-05 补传，API 复核 10 文件/10 提交） | 2026-11-05 已核一致；此后无改动 | 2026-11-05 |
| 服装线资产 | 服装线（底座封存） | 底座封存，43 图模特库 | 私有仓 fashion-film-factory（43 图＋知识文档＋蓝图，2026-11-03 核验齐全） | 2026-11-03 已核一致；此后无改动 | 2026-11-03 |
| 小程序三件 | 小程序 | Codex 主跑，Muse 不碰代码 | 私有仓 wechat-miniapp-studio | 未核对（非 Muse 资产，不主动核） | 未核对 |
| video-product（旧快照） | PitchReel | 已过期（当前版见 pitchreel 仓） | 私有仓 video-product（2026-10-31 快照） | 已过期，不追踪 | 2026-10-31 |
| rapidapi-services / gumroad-tools / n8n-packs / video-line / seo-workbench | 集合仓规划 | — | 无仓——ASSET-MAP 规划未建，按「先 A 类欠账、再 B/C」分批执行，不一夜全搬 | — | — |

## C. 能力资产仓（ASSET-MAP 规划，未建）

| 产品/项目 | 所属线 | 在线状态 | GitHub 仓 | 仓内与本地是否一致 | 最近核对日 |
|---|---|---|---|---|---|
| skills-vault / tools-mcp / media-assets | 能力资产 | — | 无仓——规划未建 | 本地有实物：~/workspace/custom-skills/（9 个自有）、~/workspace/external-skills/（实物库＋INDEX.md）、~/workspace/custom-connectors/（连接器文档与助手脚本） | — |

## D. 记忆与经营仓（私有）

| 产品/项目 | 所属线 | 在线状态 | GitHub 仓 | 仓内与本地是否一致 | 最近核对日 |
|---|---|---|---|---|---|
| factory-hub 总控 | 中枢 | — | 公开仓 https://github.com/binbin7418-dotcom/factory-hub | 一致：ATLAS.md / PROGRESS.md / DAILY-OPS.md 远端 blob SHA 与本地完全一致（2026-11-07 03:0x API 核验）；ASSET-MAP.md（本地 3,456 B，11-07 01:47 建）与本表 ASSET-INDEX.md 尚未同步，今晚传 | 2026-11-07 |
| nano-daily-growth 每日修炼汇总 | 经营 | — | 私有仓 nano-daily-growth（11-05 篇 03:50 经浏览器会话复核在位） | 2026-11-06 篇已于昨夜同步并复核；2026-11-07 篇（今晚新写）待同步 | 2026-11-07 |
| nano-memory 记忆镜像 | 记忆 | — | 无仓——规划未建（待他把 Obsidian 保险库文件发来再接管迭代） | — | — |
| project-console 项目总控台 | 经营 | 已下线（2026-11-05 他令别公开，仓库改 Private、Pages 404） | 私有仓 project-console（源码备份 project-source.zip 在仓内） | 未核对 | 未核对 |

## E. 归档仓

| 产品/项目 | 所属线 | 在线状态 | GitHub 仓 | 仓内与本地是否一致 | 最近核对日 |
|---|---|---|---|---|---|
| archive-lines | 归档 | — | 无仓——规划未建 | 已关账线（动画线、故事线等）资产仍在各自原仓，未集中归档 | — |

## F. 未归类 / 他方资产（不属 Muse 产品线，登记备查）

| 产品/项目 | 说明 | GitHub 仓 | 最近核对日 |
|---|---|---|---|
| Mika | 公开仓，描述 "An on-device AI agent for Android that operates apps and the web to get things done for you."，2026-11-04 建，约 50MB；不在 ATLAS 内，来源/归属待主会话确认；本地 ~/workspace/backups-staging/mika/ 为空目录 | 公开仓 https://github.com/binbin7418-dotcom/Mika | 2026-11-07（仅仓存在性与描述） |
| vision-core-private | Codex 的控制面（AGENTS.md＋33 份注册表/规则），无记忆正文；他方资产，Muse 只读参考 | 私有仓 vision-core-private | 2026-11-07（据 01:55 第二轮深挖结论） |
| apify-product-factory | 他的 Apify 线私有仓，Muse 不运营、不审计、不修复 | 私有仓 apify-product-factory | — |
| AmazonReady / vvhub / XRSS / RSSHub（fork）/ binbin7418-xiaohongshu-mcp | 他早年的开源仓与 fork，不动 | 公开仓（均在 64 公开仓清单内） | — |
| binbin7418-dotcom.github.io | 根集合站（全部工具落地页门户＋GSC 验证文件） | 公开仓 binbin7418-dotcom.github.io | 未核对 |

## 今晚补齐进度（2026-11-07 首跑）

- 已补：本表首版建立；video-mcp 新快照 pitchreel-src-20261107.zip 已打好（49MB、229 文件，排除 web/data、缓存、demo-video、密钥文件，含 outro 修复＋Screening 接入代码＋AUP 条款新版），待传 pitchreel 私有仓；RapidAPI 修复快照已备（477,590 B），待传 rapidapi-sources 私有仓；fashionwalk-site 建仓备料齐（README.md 新写、10 个文本文件清单），待浏览器建仓＋单传。
- 待传（浏览器窗口进行中，传完 API 核验）：factory-hub 五文件（ATLAS.md、PROGRESS.md、DAILY-OPS.md、ASSET-MAP.md、ASSET-INDEX.md）、nano-daily-growth daily/2026-11-07.md。
- 还缺：html-slides-template-pack 17 套增量（约 300 文件，manifest v2 已备，分多夜传）；skills-backup 缺口（lemo 瘦身方案、clone-website/motionsites 入库）；B/C 类集合仓与 nano-memory 未建（按 ASSET-MAP 执行口径分批，不一夜全搬）；free-ai-gateway、terra/genie4/kling4、sku-ops-landing 等行的本地对照未核。
