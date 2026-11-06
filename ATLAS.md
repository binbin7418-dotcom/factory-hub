# 总图 ATLAS（仓库 · 文件夹 · Skills 导航）

> 2026-11-02 建立。用途：任何东西「在哪、是干嘛的、找什么看哪里」先查这张图。规则：新建仓/新项目/新 skill 当天补进本图；项目每次更新连同 GitHub 备份一起更新（2026-11-02 用户下令）。
> 数字口径：公开仓清单 2026-11-07 GitHub API 实查为 64 个（2026-11-02 为 39 个）；在售数以 PROGRESS.md 与各线状态文件为准（PRODUCTS.md 停在 2026-10-29，不可信）；资产总表见 ASSET-INDEX.md（2026-11-07 首版）。

## 一、GitHub 仓库地图（binbin7418-dotcom）

### 中枢与门户（先看这里）
| 仓 | 是什么 | 找什么看哪 |
|---|---|---|
| factory-hub | 全线中枢：产品注册表、每日运营清单、总图、资产总表 | PRODUCTS.md（注册表，2026-10-29 停更）、DAILY-OPS.md（每日清单）、ATLAS.md（本图）、ASSET-INDEX.md（资产总表，2026-11-07 首版） |
| binbin7418-dotcom.github.io | 根集合站：全部工具落地页门户 + GSC 验证文件 | 根目录 sitemap；验证文件 google313065ad0232e20b.html 勿删 |
| sku-ops-landing | SKU Operations Copilot 落地页（sku.vn-node.cc.cd） | index.html |

### 产品工具仓（每个 = 一个 Gumroad $29 工具：源码 + Actions 云构建 + docs/ 落地页）
在售 42（工具类；店铺合计 72＝工具类 42＋n8n 包 20＋PitchReel 2＋体检 0（Site Index 已于 2026-11-05 Unpublish 下架）＋新词卖货站包 3（Terra/Genie/Kling 各 $9.99，2026-11-04 晚均经公开页验活）＋新站四线 5（SnapDuo 解锁包 $9.99、Tip SnapDuo、故事书 $19.99、PaperStage $12.99/$19.99、时尚 $12.99，2026-11-06 晚均经公开页验活），2026-11-03 晚主会话逐页活页实测 56 为基数，2026-11-05 第八批 5 个＋n8n 第三批 4 包依次上架，2026-11-06 晚新站四线 5 个上架）：sheetfix、feedfix、audiofix、shopifycsvfix、listclean、silencecut、pagesmith-pdf、stampbatch、dupelens、contactfix、printready、imagebatch、qrbatch、dateshift、metascrub、audiobookspecfix、invoicebatch、statementsift、puzzlepress、mailmend、ledgerlink、deckshrink、stitchchart、codewordforge、redactready、formfillbatch、crosswordpress、logicgridpress、sudokupress、qifsift、woocsvfix（第六批 5 个，2026-11-03 凌晨上架，店铺 45→50）、mathsheetpress、iifsift、calcudokupress、futoshikipress、mosaiccolorpress（第七批 5 个，店铺 50→55）。第八批 5 个（shikakupress、cryptogrampress、queenspress、binairopress、mazepress，验收 41/41）已于 2026-11-05 全部上架（均 $29，公开页 curl 逐个验活）。
不卖（仓保留）：epubfix（从未上架）、subtitlefix（已下架，引擎保留）。
找构建产物：仓内 Actions 的 build 工作流 artifact（双层 zip）；找落地页文案：docs/index.html。

### 新站四线（2026-11-06 晚全部上线，同套架构：EC2＋Caddy 分路径＋Gumroad 许可证校验＋Muse 逐单生产，48 小时交付）
| 站 | 入口 | Gumroad 产品 | GitHub 仓 | 备注 |
|---|---|---|---|---|
| SnapDuo 趋势梗合照 | https://api.newkwlab.com/duo/ | SnapDuo HD Unlock Pack $9.99（一码解锁 3 张）＋Tip SnapDuo（打赏，最低 $1） | snapduo（公开，9 文件已核一致） | 引擎 Kie Nano Banana 2.1（3 credits ≈ $0.015/张）；孤儿任务自愈已上线；热梗侦察 cron 每周一/四 |
| Starlight Stories 个性化故事书 | https://api.newkwlab.com/book/ | Personalized Christmas Storybook $19.99（ennflz） | storybook-site（公开，7 文件已核一致） | 锚点图锁脸＋版式铁律（全书统一方版）；英文朗读定版 Gemini TTS Sulafat；30 天首单观察自 2026-11-06 |
| PaperStage 纸片动画 | https://api.newkwlab.com/clip/ | Personalized Christmas Paper-Cutout Animation Solo $12.99 / Duo $19.99（jibnek） | paperstage-site（公开，6 文件已核一致） | 圣诞版已上线静挂不推（他令先推时尚）；六场景贴纸包在 ~/workspace/paperstage-scenes/ |
| Fashion Citywalk 纸片时尚 | https://api.newkwlab.com/walk/ | Personalized Fashion Citywalk Paper-Cutout Animation $12.99（okgucl） | fashionwalk-site（待建，今晚首批欠账第 1 笔） | 六款在售模板（Fashion/东京/上海 Café/Off Duty 拼贴/伦敦 Duo/香港 Market）；IG＋FB 首发帖已发 2026-11-07 02:12，TikTok 他叫停等他定 |

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
| fashion-film-factory | 服装线资产（模特库 43 张 + README） | 2026-11-02 已落仓核验；knowledge+蓝图备份包 fashion-knowledge-20261102.zip 与 BACKUP-NOTE.md 已于 2026-11-03 凌晨核验在仓，资产备份齐全 |
| comedy-line | 搞笑动画线资产（cast/概念/EP01 生产/文档/skill-run 共 5 包，39 条废片全排除） | 2026-11-03 凌晨仓库根目录列表亲核，5 包在列（本地备份源在 ip-animation/comedy-line/backup-20261103/）；EP01《抢大福》2026-11-04 00:24 收官（7 拍全过逐拍验收闸，EP01-full.mp4 45.4 秒，夜复盘 ffprobe 实测 1216×672/24fps 一致）；导播台工作台实例 2026-11-04 01:44 遭攻击已停机、永不复用；新站 cpod-1xa9hxnr4nez（4090，¥2.15/时）2026-11-04 夜–11-05 凌晨跑完 EP02：6/6 镜全过逐拍验收闸，拼合 EP02-full.mp4（61.46s/1216×672/24fps，夜复盘 ffprobe 实测一致），实例已停机；2026-11-05 01:04 用户看完成片判定「没声音、没故事」下令放弃，此路线（Director＋H3 无声逐镜拼接）就此结案，EP03 不按此路线开工；EP02 成片＋状态文件已于 2026-11-05 09:28 补传私有仓（API 复核：仓内 10 文件/10 提交，EP02-full.mp4 21.2MB 与本地字节一致），动画线资产备份关账；2026-11-05 02:26 用户定调动画线整体停下、2026-11-06 00:11 视频克隆/生成线亦推翻停掉，不再投入，资产留档不动 |
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
| goals/seo | 新词出海 SEO 站（引擎线） | site/（newkw.pages.dev 源码，18 页已上线，2026-11-03 凌晨 dist/sitemap 18 条核验） |
| rapidapi-batch* | RapidAPI 各批源站与 worker | batch3/geoip 含城市版 v2 worker 与数据暂存 |
| custom-skills | 自有 skills（9 个） | INDEX.md 总索引（触发场景+负样本） |
| external-skills | 外部 skills 实物库 | INDEX.md 逐卡登记（用途/许可/状态/路径） |
| research_notes | 全部调研报告存档 | 按日期目录：search-demand-20261101（选品）、history-sample-scout-20261101（选题）等 |
| cf-node | 自建 CF 代理节点 | .secrets.json（凭证级勿外传）；subscription-url.txt |
| user/files | 他发来的原始材料 | 小程序全套、图包原图（归档后以各项目目录为准） |
| trend-photo-station | SnapDuo 站源码＋运营 | web/（站点与服务）、agent/、TREND-WATCH.md 热梗侦察日志 |
| storybook-site | Starlight Stories 站源码 | web/、SPEC.md、BUILD-REPORT.md |
| paperstage-site | PaperStage 站源码 | web/、SPEC.md、BUILD-REPORT.md；贴纸包在 ~/workspace/paperstage-scenes/ |
| fashionwalk-site | Fashion Citywalk 站源码 | web/、SPEC.md、BUILD-REPORT.md、REDESIGN.md、SWAP-REPORT.md |
| ppt-template-product | HTML 演示模板包 20 套 | templates/（20 套×EN/ZH）、html-slides-template-pack.zip（最终包） |
| muse-bf | Muse 黑五线（fastucp 底座调研） | research_notes/muse-blackfriday-github-bases-20261106.md、shopify-bfcm-demand-20261106.md |
| backups-staging | 各线备份暂存 | rapidapi/（batch1–15）、pitchreel-src-20261107.zip（新快照）、rapidapi-repair-20261106.zip |
| growth-log/daily | 每日修炼汇总 | 2026-11-05/06/07 三篇；同步仓 nano-daily-growth（私有） |

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
6. lemo-opuscar 技术深学（2026-11-02 他定调：不试它的风格样片、不跟在别人后面；学它的知识——动效、风格、布局、音效——学好技巧后自创风格）：✅ 深学完成，STUDY.md 五章 + OUR-STYLE-TEMPLATE.md 在 research_notes/lemo-opuscar-study-20261102/。待落地（报告附录优先级）：①阅读时长检查器并入 spotcheck——✅ 代码已落地（tools/spotcheck.py，--reading-time 独立 WARN 模式，CJK/4.5+其他/15+1.5s，2026-11-02 夜复盘实测 SRT/JSON/缺文件三例全过；未接入成片硬闸）②timeline 单一真源 + cue 偏差表验收（仍待做）③ASR 逐行复检规则补进故事线 QA——✅ 等价形已落地（asr_numbers：中文位值/逐字/小数均归一为 canonical value 再比对，夜复盘实测一千九百零三→1903、三点五→3.5）。原「ink-wash 并入 FORMAT-STANDARD」口径作废。

## 五、排查清单（未关的问题，关一个划一个）
- [x] GeoIP 数据仓余 277 文件上传 + v3 worker 部署 + 线上 5 条验真。（2026-11-02 02:12 完工，见 memory/2026-11-02.md）
- [x] newkw 站 GSC 提交 + IndexNow（2026-11-02：IndexNow 202 受理；GSC 所有权验证通过，验证文件 google7e2e7b06294a1b5d.html 勿删）。残项：sitemap 已提交但 GSC 显示「无法抓取」——盒侧以 Googlebot UA 实测 200/application/xml、robots 全放行，判为新属性首次抓取的常见暂态，不删不重提，数日后复查状态。
- [x] factory-hub 的 PRODUCTS.md 同步 GitHub（2026-11-02 02:26 同步；03:4x 夜复盘 API 实查：远端 ATLAS.md 10685B、PRODUCTS.md 11181B，均与本地字节数一致，03:36「本地已更新、GitHub 尚未跟上」担忧已消除）。
- [ ] 根集合站 sitemap 补入新工具落地页。
- [ ] video-mcp 新快照刷新（video-product 仓已过期，改走 pitchreel 私有仓）：pitchreel-src-20261107.zip 已打好（49MB、229 文件，排除 web/data、缓存、demo-video、密钥，含 outro 修复＋Screening 接入代码＋AUP 条款新版），今晚上传，传完 API/浏览器核验。
- [ ] PRODUCTS.md 注册表全量补齐（仍停在 2026-10-29，未含第四批后全部产品与 72 店铺现状；勿以注册表为准报数）。
- [ ] n8n 社区登录会话 2026-11-03 起丢失，私信箱未直查（心跳多次记为覆盖缺口，非无新增），待白天恢复会话后补查。
- [x] Gumroad n8n 第三批滚动 24h 上限三连拦（04:27、09:52、23:52 均 0/3）——2026-11-05 晚第三批兽医/旅行社/除虫＋水暖 HVAC 四包全部上架（公开页 curl 验活），仅剩花店包按他 2026-11-03 决定继续压着。
- [x] 导播台安全重建＋EP02 生产（2026-11-05 凌晨 6/6 镜收官；同日 01:04 用户否决整条无声逐镜路线而结案，EP03 不按此路线开工——不是成功上线，是生产完成＋用户否决结案）。
- [x] RapidAPI 在售 100（2026-11-04 第 100 个 CardCheck 公开：https://rapidapi.com/binbin7418/api/cardcheck ，Finance，BASIC 免费 500/月、PRO $5/10,000、ULTRA $19/50,000；Studio 项目列表实数 100；LondonTransit 仍挂起、由 CardCheck 补位，不再复测排队）；CF Pages 已满 100/100，再扩品须先并项目或清位；图标 99/99 已补齐；第一梯队 v2（EmailCheck 批量＋RDAP 域名年龄、PhoneCheck 批量体检、LyricLine 缓存提速、Shopify 整店档案 /store-report＋/compare）均已部署并经 Studio 应用，EmailCheck 免费档维持 500/月不降（用户 11-04 16:00 拍板，诊断 200 方案作废）。——2026-11-05 复盘执行：C 档 17 个唯一品全部改 Private 下架（在售唯一品 99→82），FlightScope 上架（在售 82→83）；B 档补批量 6 品代码侧＋Studio 侧全部完成，全线真批量端点 4→10；稳定性周测首份 96/99（3 失败均为上游）；定价以后台实价为准（EmailCheck PRO $9/ULTRA $29/BASIC 100 次，公开页 $5/$14 口径作废）。
- [x] newkwlab.com 实名同步：模板 25377735 已实名成功，域名本体 client hold 于 2026-11-05 13:20 解除；三站自定义域名已绑（terra/genie4/kling4.newkwlab.com，Enforce HTTPS 已开，curl https 均 200 且标题正确）；api.newkwlab.com HTTPS 已通（Caddy＋Let's Encrypt）；pitchreel.newkwlab.com 已由用户本人改 A 记录指 EC2、证书已签、https 全 200。
- [ ] 新词三站待办：Bing 已做（11-06：5 站验证、4 份 sitemap Success）；GSC newkwlab.com 域名属性已验证（11-06 13:27）、binbin7418 已加为完整用户，数据待 1–3 天（复查 11-07 11:07，11-09 仍无数据报异常）；30 天首单观察期自 2026-11-04 起计，首单未出前不扩站；GEO 审计【直接改】三站已落地（Terra 静态价目/预设、Kling 景别运镜下拉、Genie 静态输出），PitchReel 法律页＋定价页规格透明已上线。
- [x] EP02 成片与状态文件私有仓 comedy-line 备份（2026-11-05 09:28 已传并 API 复核，见上）。
- [ ] RapidAPI 100 品功能审计修复：TrialFinder 文档与生产不符（审计 72 过/26 部分/1 挂）修复状态未见回执，勿记完成。
- [x] story-koubo 备份仓已建并经第二窗口复核（2026-11-02）。
- [ ] custom-skills、external-skills 备份仓待补（skills-backup 已建，但 lemo-opuscar 112MB 全仓未入，待瘦身方案，不记为已备份；2026-11-05 新入库 clone-website、motionsites-web-builder 亦未进备份；缺口已登记进 ASSET-INDEX.md）。
- [ ] PitchReel Standard 时长文案口径（实测 83s vs 标称 ≈60s）微调。
- [x] spotcheck 的 asr_numbers 补阿拉伯数字等价形（2026-11-02 夜复盘实测：中文位值/逐字/小数归一比对已落地，34 条断言全过）。
- [ ] 邀请码 samseah 池计数读不到、夜影小窝 DNS 间歇不可达（监测缺口，非下架证据）。
- [ ] Danish_Koul_14 客户对话静默（等回复，不主动追第二封）。
- [x] PitchReel 迁移 48 小时回滚观察已提前终结——他 2026-11-06 09:05 令删旧 InstaBox 入口（「旧的insabox 就删掉吧。没用了」），回滚点已毁；生产只在 EC2，健康只看公网 /health。残项：EC2 生产管理员新密码只存 EC2 本机 .admin-env，待攒批存保险库。
- [ ] 出口代理断连——定版（2026-11-06 03:40）：proxy.conf 只写裸地址 http://hatch-egress-proxy:3128；但运行时每次重启后约 50 秒会把两份 proxy.conf 重写为当次现签 token（裸地址活不过一次重启）；断连主因是出口路径突发性丢包（约 30% 失败率），与 token/主机/接口无关。重启后先查 drop-in 是否被重写；断连先看失败率与时间分布。VM 第 18 次重启 2026-11-07 02:10，agent 自愈约 1 分钟、重启后零 error（见 PROGRESS 2026-11-07）。
- [ ] SEO 工作台：GSC sc-domain:newkwlab.com 已验证（2026-11-06 13:27），binbin7418 已加为完整用户；数据待 1–3 天（复查 11-07 11:07，11-09 仍无数据报异常）；Bing 5 站验证、4 份 sitemap Success；Clarity 4 站 21 页；SOP-01 找词日报 2026-11-06 起连跑 3 天，首跑回执未见待核查；SOP-02 已定版；GEO 审计【待拍板】项攒批报 Vision；newkw 首份按页数据（点击 0/展示 2/排名 22.5）实为 newkw.pages.dev 口径（非 newkwlab.com），太薄不触发配包，继续观察。
- [ ] 自然流平台扩展：api.market 开店 5/5 完成（出款信息已填 PayPal 1060207169@qq.com）；8 品：已上线 2（EmailCheck 11-06 05:29、PhoneCheck 11-06 14:01 批准）、在审 5（FXRates 已修 spec 重新提交、VinScope、IBANCheck、WeatherNow、HolidayCal）、草稿 1（HostIntel：Shodan 免费版非商业授权问题，RapidAPI 侧已改回 Public）；AlternativeTo 账号 visionwei 已确认，约 2026-11-12 解锁提交，届时实测；Zyla 待启动。
- [ ] 22016 模板重提挂起，等他本人用 wbin7419 登录上传，不催（重提包已修好复核，行业字段仍写 realestate，上传前须改）；Kie API key 已于 2026-11-06 13:10 到手并验活（custom.kie-ai，余额 916.5 credits 起），本项旧口径作废。
- [ ] PPT 模板包 20 套：最终打包已完成（zip 16.3MB/410 文件，11-06 14:43），定价方案与 Gumroad 上架待他拍板；备份仓 html-slides-template-pack 仅 3 套（44 文件），17 套增量约 300 文件待分多夜上传（manifest v2 已备）。
- [ ] Waffo 整改：部署验证（terms.html §5 AUP 上 EC2＋本机接 Screening 跑真接口）待他点头，之后重提审核；生产/测试 Key 私钥已存本机（0600）。
- [ ] RapidAPI 修复快照补传：rapidapi-repair-20261106.zip（477,590 B）今晚传 rapidapi-sources 私有仓。
- [ ] fashionwalk-site 建仓：今晚首批欠账第 1 笔（公开仓，10 个文本文件；媒体不进仓）。注：另有口径称「fashionwalk-site 已建」，GitHub API 两次查无（11-07 03:05 与 03:2x，64 公开仓清单内无此仓、直接查 404），该口径降级为未完成，以 API 为准。
- [ ] n8n 试用 2026-11-08 到期，3 天宽限后工作流暂停；n8n 线已转低功耗（2026-11-06 13:21 定调），gigs 与行业包只挂着。
- [ ] 全线作战计划（~/workspace/goals/goal/files/全线作战计划-20261107.md）待他确认，未批准。
- [ ] Claude Code 审计脑首轮（全站触达/小程序读仓/RapidAPI A 档一致性）待他点头；它不碰主分支/线上/账号。
- [ ] Mika 公开仓（2026-11-04 建，50MB，Android AI agent 描述）不在 ATLAS 内，来源/归属待主会话确认。
- [ ] VM 主机稳定性评估（白天待办）：11-06 一天 5 次重启（13–17 次），11-07 02:10 第 18 次；agent 自愈正常，但重启频率异常须白天评估。

## 六、找东西速查
- 某个产品在没在卖、卖多少钱 → factory-hub/PRODUCTS.md
- 今天该干什么 → factory-hub/DAILY-OPS.md
- 仓在哪、文件在哪 → 本图一、二节
- 某个能力怎么做 → custom-skills/INDEX.md（自有）或 external-skills/INDEX.md（外部）
- 某个结论的证据 → research_notes/ 对应日期报告
- 某条线的规矩 → ~/AGENTS.md + 对应 GOAL.md
