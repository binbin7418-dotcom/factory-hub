# 产品注册表（PRODUCTS）

状态口径：在售 = 公开页可购买且经亲自核验；建成待上架 = 仓库/构建/落地页全部完成，只差最后上架动作。收入一律以真实到账为准，当前全部为 0。

## 一、Gumroad 工具线（目标 100，当前 17 个条目：在售 15、不卖 2）

统一形态：本地运行（数据不出本机）→ 检查/修复 → 复检出报告；Windows 一键包；$29 一次性（DateShift $9、MetaScrub $19 例外）。落地页统一在 binbin7418-dotcom.github.io/<产品名小写>/，源码仓 github.com/binbin7418-dotcom/<产品名小写>。

| # | 产品 | 一句话 | 状态 | Gumroad / 种子验收摘要 |
|---|---|---|---|---|
| 0 | SheetFix（样板） | Excel 审计修复 | 在售 | binbinster.gumroad.com/l/sheetfix-excel-audit；13 条缺陷修 5、连带消除共 8、剩 5 判断级、新引入 0 |
| 1 | FeedFix | Google Shopping Feed 修复 | 在售 | /l/feedfix-google-shopping-feed-repair；12 商品 21 问题修 10、剩 11（5 阻断）、新引入 0 |
| 2 | EPUBFix | EPUB 发布前检查修复 | 已决定不卖（从未成功上架） | 2026-10-25 核查：Gumroad 公开页 404、后台无此商品——建厂当日「已上架」回执不实；竞品复盘判定付费证据最弱，用户 2026-10-25 拍板下架（无架可下）；仓库与落地页保留，落地页已标停售 |
| 3 | AudioFix | 播客响度标准化+剪静音 | 在售 | /l/audiofix-podcast-loudness；-29.9→-15.9 LUFS、剪静音 4.2s、PASS |
| 4 | ShopifyCsvFix | Shopify 商品 CSV 修复 | 在售 | /l/shopifycsvfix-product-csv-repair；5 行 14 问题修 11、剩 3 阻断 |
| 5 | ListClean | 邮箱列表本地清洗 | 在售 | /l/listclean-local-email-list-cleaner；12 行→干净 7、去重 1、无效拒 2、一次性域名 1 |
| 6 | SilenceCut | 口播视频剪静音/气口 | 在售 | /l/silencecut-talking-head-silence-remover；9s→6.5s、静音 3.0→0.4s（边界：删口水词需转写，文案已明示） |
| 7 | SubtitleFix | SRT/VTT 字幕修复 | 已下架（2026-10-25） | /l/subtitlefix-srt-vtt-repair 已 Unpublish（未删除）；竞品复盘判定付费证据最弱，用户拍板下架；引擎保留，日后可作视频工具包附赠 |
| 8 | PrintReady | KDP 印刷 PDF 预检修复 | 在售 | /l/printready-kdp-pdf-precheck；5 页种子书 2 处结构修复、复检如实报 3 阻断；2026-10-27 晚经公开页核验在售 |
| 9 | ImageBatch | 卖家图片批量预处理 | 在售 | 2026-10-25 复盘改定位 Etsy-first，/l/etsy-listing-photo-prep；EXIF 摆正/限尺寸/剥元数据/整夹小 67%；2026-10-27 晚经公开页核验在售 |
| 10 | QRBatch | CSV 批量二维码+打印版 | 在售 | /l/qrbatch-bulk-qr-print-sheets；5 行→4 码、2 警告、A4 300dpi 打印版；2026-10-27 晚经公开页核验在售 |
| 11 | PageSmith PDF | PDF 拆分/合并/旋转/提取/文字水印+复检 | 在售 | 第二批；/l/pagesmith-pdf-batch-tools；种子验收 20/20；仓 pagesmith-pdf、Actions 构建 success 均经主会话 GitHub API 核验（2026-10-26）；2026-10-27 经公开页核验在售 |
| 12 | StampBatch | 批量照片水印+平台预设+复检 | 在售 | 第二批；/l/stampbatch-batch-photo-watermark；种子验收 24/24；仓 stampbatch、构建 success 已 API 核验（2026-10-26）；2026-10-27 经公开页核验在售 |
| 13 | DupeLens | 重复/相似照片查找+隔离区（绝不删除） | 在售 | 第二批；/l/dupelens-duplicate-photo-finder；种子验收 27/27、误报 0；仓 dupelens、构建 success 已 API 核验（2026-10-26）；2026-10-27 经公开页核验在售 |
| 14 | ContactFix | vCard 联系人去重合并 | 在售 | /l/contactfix-vcard-duplicate-merge；2026-10-27 经公开页核验在售 |
| 15 | DateShift | 照片日期批量修正 | 在售 | $9；/l/dateshift-photo-date-fixer；2026-10-27 晚第四批上架并经公开页核验 |
| 16 | MetaScrub | 照片元数据清理+报告 | 在售 | $19；/l/metascrub-metadata-scrub-report；2026-10-27 晚第四批上架并经公开页核验 |

另有旧产品：SKU Operations Copilot（$19，在售，0 销量，binbinster.gumroad.com/l/shopify-sku-ops-copilot，落地页 sku.vn-node.cc.cd）。

## 二、RapidAPI 线（目标 100，当前公开 27 个）

统一：免费层 + PRO/ULTRA 订阅；源站 Cloudflare Pages；网关实测全过；真实订阅 0。2026-10-26 提额已批（工单 144055），每账号 20 个公开上限已移除，可继续上架。

| 批次 | API | 定价 | 源站目录 |
|---|---|---|---|
| 一 | Page2MD、QRGen、MetaExtract、Feed2JSON、MD2HTML、TextLens | $15/$49 档 | rapidapi-batch/、rapidapi-first-api/（page2md） |
| 二 | EmailCheck、CryptoPulse、WeatherNow、PhoneCheck、DomainIntel、FXRates（FXRates 已恢复公开） | PRO $5–10 | rapidapi-batch2/ |
| 三 | HolidayCal、DNSPilot、IBANCheck、UAParse、PostCode | PRO $3–9 | rapidapi-batch3/ |
| 四 | TextAI、ScanText、BookLens、QuakeWatch | PRO $3–9 | rapidapi-batch4/ |
| 补 | GeoIP（IP 国家与 ASN 查询） | $0/$5/$19 | geoip 项目 Pages secret 已设并重部署，国家级通路已通；公开页 rapidapi.com/binbin7418/api/geoip-ip-country-and-asn-lookup |
| 五 | GeoPlaces（地理编码与地址查询） | $0/$7/$17 | geoplaces.pages.dev；公开页 rapidapi.com/binbin7418/api/geoplaces-geocoding-and-address-lookup；2026-10-27 上架并经公开页核验 |
| 六 | MockGen（确定性假数据生成）、SunTimes（日出日落与月相）、WordLens（英语词典同义与例句）、CountryData（国家事实货币与区号） | 统一 $0/$5/$14 | mockgen-49y.pages.dev、suntimes-api.pages.dev、wordlens.pages.dev、countrydata.pages.dev；公开页前缀 rapidapi.com/binbin7418/api/mockgen-deterministic-fake-data-generator、/suntimes-sunrise-sunset-and-twilight-times、/wordlens-english-dictionary-synonyms-and-examples、/countrydata-country-facts-currencies-and-calling-codes；2026-10-27 晚全部上架并经公开页核验 |

计数口径：一至四批 21 个 + GeoIP 1 个 + 第五批 GeoPlaces 1 个 + 第六批 4 个 = 27 个。

二号备选（2026-10-25 注册成功，Wbin7416@gmail.com，账号 ID 12411578，显示名 Bin Wei）：PayPal 关联未完成——PayPal 授权在 hCaptcha 多轮后密码提交报错，已停手防收款账号风控，「同一 PayPal 能否绑二号」仍未测到平台表态，待冷却后重试。WordWeb（Datamuse 从 CF 出口 403）停放。

搜索可见性（2026-10-25）：PhoneCheck 约 39 位、CryptoPulse 约 68 位、WeatherNow 约 81 位，其余暂未进前 100——新列表常态，靠调用量爬升。

## 三、n8n 线（目标 100 个模板/服务资产，当前 10 个产品位：8 个已落地、2 个进行中）

- Fiverr gig 在架 4 个：主 gig（n8n 自动化代建 $90/$140/$290）、WhatsApp 自动回复+线索打分（$90/$190/$390）、修复/诊断、Looker Studio 报表；均 3 图满库。卖家 @visionwei。
- 待发 2 个（被新卖家 4 个上限挡住）：AI 客服智能体（$90/$240/$490）、线索获取+打分（$90/$190/$390）；文案与图在 ~/workspace/接单雷达/ 对应目录。
- Gumroad 行业包 6 个（$49 一次性，含设置答疑；引擎与 Fiverr/社区样品同一套，出厂文件逐字提取验收，每包 7/7 全过；本地 ~/workspace/product-factory/n8n-packs/），2026-10-27 全部经公开页核验在售：
  - 地产版 WhatsApp Lead Receptionist for Real Estate Agents：在售 binbinster.gumroad.com/l/whatsapp-receptionist-real-estate（热线索实测 100 分）
  - 汽修版 WhatsApp Lead Receptionist for Auto Repair Shops：在售 /l/whatsapp-receptionist-auto-repair（热线索实测 85 分）
  - 美容版 WhatsApp Lead Receptionist for Beauty Salons & Spas：在售 /l/whatsapp-receptionist-beauty-salon（热线索实测 95 分）
  - 牙科版 WhatsApp Lead Receptionist for Dental Clinics：在售 /l/whatsapp-receptionist-dental-clinic（热线索实测 100 分）
  - 健身版 WhatsApp Lead Receptionist for Fitness Studios：在售 /l/whatsapp-receptionist-fitness-studio（热线索实测 100 分）
  - 宠物版 WhatsApp Lead Receptionist for Pet Services：在售 /l/whatsapp-receptionist-pet-services（热线索实测 100 分）
- n8n 官方模板库：第 10 个产品位。提交路径已摸清（creators.n8n.io）；卡点为保险库内该站点登录的用户名存成了实例地址而非邮箱，已停手不再弹卡，记入攒批清单（用户顺手重存后补交）。云实例活样板已建成：weib.app.n8n.cloud 内「WhatsApp Lead Receptionist — Live Demo」（12 节点，样例实测 85 分/Hot，未激活），试用约至 2026-11-08。
- 样品资产：WhatsApp Lead Receptionist 工作流（仓 github.com/binbin7418-dotcom/whatsapp-lead-receptionist；社区展示帖待平台审批）；线索打分 demo 实测版（11 用例全过，Hot ≥70 / Warm ≥45）。
- 社区应征：累计 6 封（邮箱/私信），截至 2026-10-25 暂无回复，巡检持续盯。

## 维护记录

- 2026-10-25：中枢仓建立；11 个落地页全部上线核验；3 个产品等安装包回传后由 cron `gumroad-final3-watch` 自动上架。
- 2026-10-25 下午：n8n 线扩到 10 个产品位——Gumroad 行业包 3 个建成并逐包验收（地产/汽修已在售，美容待次日补上架）；n8n 模板库提交卡在创作者门户登录，路径已记录待办。
- 2026-10-25 傍晚：竞品拆解复盘完成——SubtitleFix 下架、EPUBFix 确认从未上架并决定不卖（在售工具实为 6 个，逐个公开页核验）；待上架 3 个产品文案按复盘修订（ImageBatch Etsy-first / QRBatch 印刷标签 / PrintReady 拒审钩子+退款保证）。
- 2026-10-25 晚：RapidAPI 第三、四批上架，公开数达 20 撞平台上限；FXRates 切 Private 给 QuakeWatch 腾位；提额工单已提交；二号（Wbin7416）注册成功、PayPal 关联待续。n8n 行业包新增牙科/健身/宠物 3 包建成验收。
- 2026-10-26 凌晨：第二批 3 工具（PageSmith/StampBatch/DupeLens）仓库建成并经 GitHub API 逐仓核验（文件齐全、build-windows 全部 success、落地页已上线）；Gumroad 上架排 10-27。本文件为本地先行更新，GitHub 中枢仓与根集合页待上架完成后一并同步。
- 2026-10-27：分发侧同步定版——Gumroad 在售 15 个（PrintReady/ImageBatch/QRBatch 晚间走重新下载 artifact→本地验包→授权逐个上传路线全部上架并经公开页核验，cron `gumroad-final3-watch` 已停用；第四批 DateShift $9、MetaScrub $19 同晚在售）；n8n 行业包 6 个全部在售；RapidAPI 公开 27 个（提额已批、GeoPlaces 与第六批 4 个经公开页核验）；本文件 2026-10-27 夜同步至 GitHub 中枢仓，根集合页与 sitemap 同步更新为 15 个工具落地页。
