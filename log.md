# Wiki Log — A股投研

> Chronological record of all wiki actions. Append-only.

## [2026-06-17] create | Wiki initialized
- 41 reports imported, 19 entities + 9 concepts + 1 comparison = 29 pages

## [2026-06-17] ingest | 对日替代五大方向
- 12 new entities, total → 31 entities, 41 pages

## [2026-06-17] ingest | AIDC供电产业链 mx-search补充 + 光通信测试设备 + 源杰/华工/东山精密
- Total → 39 entities + 11 concepts + 1 comparison = 51 pages

## [2026-06-17] lint | Wiki 健康检查
- 0 broken links, 0 orphans, all pages ≥2 outlinks

## [2026-06-20] lint-fix | index.md 计数修正
- 51→54 total, 39→42 entities, 9→11 concepts

## [2026-06-20] create | 应流股份(603308) + 万泽股份(000534) 全面分析
- 44 entities + 11 concepts + 1 comparison = 56 pages

## [2026-06-21] ingest | 海外燃机PDF → gas-turbine更新
- GEV/西门子/卡特/贝克休斯/三菱 Q1数据, 燃气内燃机, 零部件深度数据
- 3份PDF归档 (会议纪要): 海外燃机/猪周期/燃机零部件

## [2026-06-21] create | 猪周期 concept + 银轮股份 entity
- concepts/pig-cycle.md: 去供给初期, PSY 16→22, 政治局点名
- entities/002126.md: 转债不赎回+套保3.5亿$+燃机10亿利润终局
- 45 entities + 12 concepts + 1 comparison = 58 pages

## [2026-06-21] sync | 四份事件分析报告 → wiki
- 良信(002706): Q1-45%利润底+固态断路器+SSCB必选项
- 可立克(002782): Q1-64%利润底+定增转向AI磁件战略跃迁
- 银轮(002126): 转债不赎回+套保3.5亿$+燃机10亿终局

## [2026-06-21] archive | 移除智光电气(002169) — 虚假信息过多
- Deleted: entities/002169.md
- Cleaned all references from concepts: 800v-hvdc, solid-state-transformer, hbm-supply-chain
- Cleaned index.md
- Raw reports retained (raw/ is immutable)
- Wiki: 44 entities + 12 concepts + 1 comparison = 57 pages

## [2026-06-21] ingest | SST四标全面分析（可立克/金盘/四方/西电）
- 4份全面分析报告 → raw/reports/260621/
- 创建 entity: 688676金盘 + 601126四方 + 601179西电
- 更新 entity: 002782可立克（PE修正+新报告）
- SST concept: 添加4个wiki实体链接 + 4条新source
- Wiki: 44→47 entities, 57→60 总页

## [2026-06-21] update | 良信股份(002706) 补充订单情报
- mx-search 两路搜索: 订单合同 + 最新公告
- 新增 ## 📋 订单与合同 章节（8条订单/合同数据）
- 关键: 北美唯一中国断路器供应商 / 近百款UL认证 / 株洲中车中标 / 合同负债+14.5%
- 更新 frontmatter sources + log

## [2026-06-21] update | solid-state-transformer concept 加入良信股份
- 3.2 上游供应链：新增固态断路器(SSCB)行 → [[002706|良信股份]]
- 6.2 A股SST标的速查：新增良信股份行
- 理由：SSCB是SST必选保护器件（微秒级切除），良信已发布纯固+混固产品
- 更新 frontmatter updated + sources

## [2026-06-21] sync | HVDC 7标订单信息全量同步
- 存量更新：中恒电气(002364) + 麦格米特(002851) + 安科瑞(300286) → 新增 📦 订单追踪章节
- 新建 entity：科华数据(002335) + 科士达(002518) + 中熔电气(301031)
- 良信股份(002706) 此前已更新
- index.md: 47→50 entities, 60→63 总页
- 数据源: mx-search 2026-06-21 批量搜索

## [2026-06-21] analyze + sync | 露笑科技(002617) 全面分析
- comprehensive-stock-analysis: mx-search + mx-data + 知识星球三路并行
- 创建 entity: 002617 露笑科技 (SiC衬底/8英寸量产/12英寸突破)
- 报告保存: reports/260621/露笑科技_全面分析_260621.md → 已微信发送
## [2026-06-22] create | sic-supply-chain 碳化硅产业链概念页
- mx-search 全产业链扫描 → 15只SiC标的（衬底4+设备3+器件5+测试1+外延2未上市）
- 6步标准结构：市场概览/竞争格局/估值背景/投资含义
- 关键催化：AIDC SiC需求CAGR 120% + 英伟达先进封装CAGR 176%
- 交叉引用：关联 800v-hvdc + solid-state-transformer + 露笑科技 entity
- index.md: 12→13 concepts, 64→65 总页

## [2026-06-22] ingest | GPU供电深度文章 → wiki 全链路同步
- 来源：知乎「电源大能」《离 GPU 最近的最后一厘米》
- 归档：raw/articles/
- 800v-hvdc concept: 新增 3.2.5 三级供电体系（PDN/VPD/IVR演进+TLVR电感）
- 新建 entity: 顺络电子(002138) + 麦捷科技(300319) — TLVR耦合电感国产突破
- 麦捷科技: 2026.5首次国产TLVR写入GPU原厂BOM
- index.md: 51→53 entities, 65→67 总页

## [2026-06-22] ingest | 800V HVDC 砖块电源深度文章 → wiki 全链路同步
- 来源：知乎「电源大能」《800V HVDC 砖块电源技术深度解析》
- 归档：raw/articles/
- 800v-hvdc concept: 新增 IBC砖块电源章节（物理定律/四级电压轨/四维约束/玩家矩阵/SSCB）
- 关键节点：800V HVDC批量出货提前到2026Q3（TrendForce），台达Q4大规模投产
- 新建 entity: 欧陆通(300870) + 深南电路(002916) + 兴森科技(002436) + 横店东磁(002056)
- IBC玩家矩阵：台达/Infineon/Vicor/英诺赛科/麦格米特/欧陆通/MPS/Navitas
- index.md: 53→57 entities, 67→71 总页

## [2026-06-22] ingest | SST产业链全景深度文章 → wiki 全链路同步
- 来源：知乎「电源大能」《SST产业链全景：从功率半导体到系统集成》(26KB)
- 归档：raw/articles/
- SST concept: 新增2.6节（四种拓扑+三级架构+核心元器件+七重壁垒+AIDC经济性+全球市场+五条投资主线）
- 关键数据：SST全球市场2024~5亿$→2030~60亿$(6年12倍)，AIDC占比15%→55%
- 关键拐点：SST TCO 2028年打平传统方案
- 新建 entity: 安泰科技(000969) + 法拉电子(600563) + 许继电气(000400)
- 新增材料板块
- index.md: 57→60 entities, 71→74 总页

## [2026-06-25] ingest | 知识星球每日摘要 6/24 → wiki 全链同步
- 来源：知识星球每日摘要 6/24（401条主题，15页）
- 归档：raw/reports/ZSXQ/知识星球_摘要_260625.md
- 新建 concept: semiconductor-price-cycle（半导体涨价周期）+ mlcc-capacitor（MLCC/被动元件）
- 更新 concept: aidc-liquid-cooling（新增冰轮环境/英维克动态）+ gas-turbine（新增AIDC共振动态）
- 更新 entity: 应流股份(603308) + 法拉电子(600563) + 三环集团(300408) + 国瓷材料(300285)
- SCHEMA.md: 新增标签 半导体/MLCC/MLCC上游/MLCC涨价/被动元件/涨价
- index.md: 13→15 concepts, 74→76 总页

## [2026-06-28] create | 商业航天 concept + 11 entity stubs
- 来源：mx-search 长征十号乙火箭+商业航天（15条研报/新闻）+ 知识星球 中信建投/中泰机械 研报
- 新建 concept: commercial-space（商业航天产业链，含火箭制造/卫星载荷/特种配套三层标的，均经 mx-search 主业验证）
- 新建 entity: 广联航空(300900) + 超捷股份(301005) + 斯瑞新材(688102) + 飞沃科技(301232) + 航天工程(603698) + 上海瀚讯(300762) + 中国卫星(600118) + 信科移动(688387) + 国博电子(688375) + 珠海冠宇(688772) + 海兰信(300065)
- 验证结果：7只高置信度（主业高度相关），3只中置信度（逻辑成立但非纯主业），1只低置信度（国博电子Q1利润-98%）
- SCHEMA.md: 新增标签 商业航天
- index.md: 60→71 entities, 15→16 concepts, 76→88 总页

## [2026-06-28] create | 信维通信(300136) entity + 更新 commercial-space
- mx-search验证：SpaceX卫星地面终端独家供应商（2021起），60亿定增加码商业卫星通信，26Q1扣非+104%
- 新建 entity: 300136.md
- 更新 concept: commercial-space（新增SpaceX/海外链板块，含信维/迈为/钧达/东方日升）
- index.md: 71→72 entities, 88→89 总页

## [2026-06-28] create | 千帆星座 + GW星座 concept 页
- mx-search 双星座产业链深挖（各15条），知识星球 华泰/建投/ZX等机构研报
- 新建 concept: qianfan-constellation（千帆/G60，>1.5万颗，200在轨，垣信运营）
- 新建 concept: gw-constellation（中国星网，1.3万颗，171在轨，6G空天一体）
- 双页含：核心数据/产业链标的/发射节奏/技术特点/频轨资源/对比表
- SCHEMA.md: 新增标签 卫星互联网/6G
- index.md: 16→18 concepts, 89→91 总页

## [2026-06-28] update | 商业航天六只高置信度核心 → 补充订单信息
- mx-search 逐只搜寻订单/合同/中标公告，6只全部更新
- 广联航空(300900): 蓝箭10亿长单+天龙三号单箭>2000万+年产40发
- 超捷股份(301005): 2025航天收入6696万(+355%)+产能10发/年
- 斯瑞新材(688102): 朱雀三号独家供应+待交付3.62亿+26Q1商业航天+300%
- 飞沃科技(301232): ⚠️航天收入仅123万(<1%)，三次并购切入但未获大批量订单
- 上海瀚讯(300762): 垣信信关站4994万+载荷中标入围
- 信维通信(300136): SpaceX独家6年+星网12.6亿+银河航天>18亿+8481万套在手

## [2026-06-28] update | 五只高置信度核心全面分析 → wiki
- mx-search + 研报深挖 超捷/斯瑞/上海瀚讯/中国卫星/信维通信，全部升级为完整分析页
- 超捷股份(301005): 25年营收8.79亿(+39.5%), 航空航天6696万(+355%), 浙商"买入"
- 斯瑞新材(688102): 25年营收15.72亿(+18%), 26Q1扣非+46%, 华泰26E净利2.04亿, PE 149x
- 上海瀚讯(300762): ⚠️连续三年亏损, 25年营收5.03亿, 商业航天1.2亿, 定增7.46亿已获批
- 中国卫星(600118): 25年营收61亿但净利仅3556万(PE 2497x), 毛利率8.84%, 卫星制造国家队
- 信维通信(300136): SpaceX独家6年, 华创"强推", 26E净利12.87亿, 目标价50.05元

## [2026-06-29] create | 先进封装 concept + 4 entity stubs
- mx-search主业验证：甬矽电子(688362)/长电科技(600584)/汇成股份(688403)/晶方科技(603005)全部通过
- 剔除芯碁微装（设备商非封测），剔除盛合晶微（非A股）
- 新建 concept: advanced-packaging（先进封装，280亿+集体扩产，甬矽103亿/长电78亿）
- 新建 entity: 688362.md, 600584.md, 688403.md, 603005.md
- index.md: 91→96 总页（72→76 entities, 18→19 concepts）
- SCHEMA.md: 新增标签 先进封装
### 2026-07-01 | 功率半导体板块同步
- 新建 concept: power-semiconductor（功率半导体）
- 新建 entity x8: 603290/688187/600460/688396/300373/605111/688261/688711
- 新增报告: reports/260701/功率半导体_行业分析_260701.md
- 更新 index.md: entity +8, concept +1
### 2026-07-01 | ZSXQ 6/30每日摘要同步
- 同步 concept: semiconductor-price-cycle, advanced-packaging, humanoid-robot, commercial-space
- 新增报告: reports/ZSXQ/知识星球_摘要_260630.md (8页240条)
### 2026-07-01 | 时代电气全面分析
- 更新 entity: 688187.md（全面分析增强）
- 新增报告: reports/260701/时代电气_全面分析_260701.md

## [2026-08-16] create | AIDC电源 总览概念页
- 新建 concepts/aidc-power.md：AIDC 电源总览（严格供电链路口径：HVDC/SST/PSU/保护器件/元器件/备电）
- 整合来源：800v-hvdc / solid-state-transformer / byte-ai-power / aidc-supply-chain / gas-turbine / power-semiconductor + comparisons + reports + events
- 标的按环节表格（约 29 只），新闻时间线 2026-05-15 至今（近3个月，倒序）
- index.md: concepts 48→49, total 268→269
- SCHEMA.md: 新增标签 AI电源

## [2026-08-16] update | AIDC电源 追加国产替代属性
- concepts/aidc-power.md 新增「🔧 国产替代属性」三档清单
- 第一档 明确表述 14 只 / 第二档 国产龙头 6 只 / 第三档 低国产化率环节 6 项
- 来源：实体页+概念页检索，逐条标注来源文件
- 同步更新页面更新日志

## [2026-08-16] verify | AIDC电源国产替代 可信度评估（妙想全量验证）
- 新建 reports/260816/AIDC电源国产替代_可信度评估_260816.md（20只评级：S/A/B/C × 强度）
- mx-search 全量验证 20 只 + mx-data 抽查 8 只（数据落 queries/mx_verify/）
- 证实 7 条 / 降级标注 9 条 / 存疑证伪 3 条（麦捷AVL、安泰SST无订单、四方-维谛传闻）
- aidc-power.md 加报告链接+麦捷/安泰/泰永⚠️；reports.md 加目录条目

## [2026-08-16] fix | 麦捷科技 TLVR「直供英伟达」表述全库修正
- entities/300319.md：TLVR 行补 ⚠️未获 AVL
- concepts/800v-hvdc.md：改「媒体口径」，加注⚠️公司澄清未获AVL、小批量试产
- 已修正页面：aidc-power.md(2处)、800v-hvdc.md、entities/300319.md、可信度评估报告

## [2026-08-17] analysis | 算力租赁 3-6个月投资筛选
- 新增报告：reports/260817/算力租赁_3-6个月投资筛选_260817.md
- 刷新核心6标的8/17行情、H1业绩口径、负债率、质押与PE
- 硬闸结论：智微智能可分批；协创/利通/润泽等验证；宏景/东阳光不参与
- 更新 concepts/suanli-rental.md、comparisons/suanli-rental-six-stocks.md、reports.md

## [2026-08-17] verify | 算力租赁 四维度投资价值验证
- 新增报告：reports/260817/算力租赁_四维度验证_260817.md（真实订单落地/高端算力规模/业绩兑现能力/电力资源 四维度；mx-search 23次 + mx-data 6组，数据落 queries/suanli_rental_dim_verify_0817/）
- 关键新增证据：东阳光 8/17 晚中报落地三笔 5 年期算力订单累计 390-460 亿（H1 算力收入仅 6034 万、设备投入 41.14 亿）；协创 8/17 互动确认多集群交付验收进入计费；智微 H1 经营现金流 +9.68 亿转正、智算收入 10.3 亿(+245%)
- 评级修正：润泽科技上调为「资源禀赋第一候选」（自建110kV变电站/包电模式）；智微智能加注「算力租赁纯度低、无自有电力」风险；东阳光从纯题材升级为「订单兑现跟踪标的」（当期仍不参与）
- 原排序（智微>协创>利通>润泽>宏景/东阳光）四维度下基本成立
- 更新 concepts/suanli-rental.md（四维度结论+更新日志+来源）、reports.md（目录+计数216→217）
## [2026-08-19] create | 高频变压器 概念页
- 新建 concepts/high-frequency-transformer.md：高频变压器厂商全景 + 可立克地位
- 独立搜索（mx-search 3组 + 通用网页）→ mx-data 财务核实 → 知识库对照（entities/002782/002885/002922 + solid-state-transformer），结论一致
- 关键结论：可立克=国内磁性元件龙头+SST高频变压器A股核心标的+台达链卡位（第一梯队）；全球龙头仍为村田/TDK/台达等国际大厂
- 可信度提示：「台达50-60%外购自可立克/独供」为自媒体/纪要口径，权威研报未量化
- index.md: concepts 49→50, total 269→270
## [2026-08-19] analysis | 高频变压器 国产替代 深度分析 + 可信度评估
- 新建报告：reports/260819/高频变压器_国产替代_可信度评估_260819.md（三环节评估 + 13 标的评级矩阵）
- 新建实体页：entities/688190.md（云路股份）、300811.md（铂科新材）、002902.md（铭普光磁）、301120.md（新特电气）
- 更新 concepts/high-frequency-transformer.md：追加国产替代三环节摘要 + 报告链接
- 结论：材料端国产化已兑现（中国产能55%/国内市占58%/云路全球第一）；器件端替代窗口期但订单早期（可立克SST研发测试早期、京泉华MFT小试）；整机端0到1（西电出海首单/四方量产/金盘北美）
- 业绩分化：云路/铂科兑现最好；铭普/茂硕/天通亏损，主题与业绩需区分
- 验证：mx-search 8组 + mx-data 9只财务核实；index.md: entities 216→220, total 270→274; reports.md: 217→218
## [2026-08-19] analysis | 铂科新材 全面分析（深挖）
- 新建报告：reports/260819/铂科新材_全面分析_260819.md（概况/技术壁垒/盈利/订单客户/竞争格局/国产替代/估值风险）
- 增强 entities/300811.md：全面重写（行情/主营构成/技术壁垒/客户/竞争/国产替代/风险）
- 关键结论：全球粉芯第一27.1%+AI芯片电感全球第五7.6%；铜铁共烧工艺全球独创；2026Q1毛利率37.1%创低点、芯片电感增速降至+20%、产能利用率下滑；PE(TTM)77.6x
- 客户：华为/比亚迪/阳光电源/ABB/台达/MPS/伟创力；芯片电感经MPS/伟创力间接供货全球头部GPU/ASIC（招股书口径）
- 验证：mx-search 7组 + mx-data 4组（含顺络/麦捷/东睦对比）+ 网页交叉；reports.md: 218→219；index: 300811 报告数→1
| 2026-08-27 | 创建 [[sugar]] 概念页 + 5个糖业entity（600737中粮糖业/000911广农糖业/000833粤桂股份/600251冠农股份/600191华资实业）| 用户报告摄入 temp/糖.md |
