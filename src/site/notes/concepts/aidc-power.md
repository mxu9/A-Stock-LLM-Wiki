---
{"dg-publish":true,"permalink":"/concepts/aidc-power/","title":"AIDC电源","tags":["AIDC","AI电源","电力设备","HVDC","固态变压器","燃气轮机"],"dg-note-properties":{"title":"AIDC电源","slug":"aidc-power","created":"2026-08-16","updated":"2026-08-16","type":"concept","tags":["AIDC","AI电源","电力设备","HVDC","固态变压器","燃气轮机"],"sources":["concepts/800v-hvdc.md","concepts/solid-state-transformer.md","concepts/byte-ai-power.md","concepts/aidc-supply-chain.md","concepts/gas-turbine.md","concepts/power-semiconductor.md","comparisons/ai-power-three-stocks.md","comparisons/hvdc-three-stocks.md","reports/260701/AIDC产业链_行业分析_260701.md","reports/260616/800V HVDC_行业分析_260616.md","reports/260617/HVDC_最新投研动态_260617.md","reports/260613/固态变压器_行业分析_260613.md","reports/260710/阳光电源_全面分析_260710.md","reports/ZSXQ/知识星球_摘要_260815.md","events.md"]}}
---


# AIDC电源

> 🔥 核心标签：AI 数据中心供电革命 | 800V HVDC | SST 固态变压器 | 供电架构三阶段演进（UPS→HVDC→SST）| 2026-2028 黄金窗口

## 定义与范围

AIDC（AI 数据中心）电源指数据中心供电/配电链路，电气系统占新建数据中心总投资 **40-45%**。^[concepts/aidc-supply-chain.md]

本页聚焦**供电链路**（严格口径）：
- **一次电源**：电网/中压 → 800V 高压直流（HVDC），含 HVDC 电源柜、巴拿马电源
- **二次电源**：800V/400V → 中间母线（PSU、IBC）
- **三次电源**：中间母线 → GPU 核心（<1V，占供电半导体投入约 60%，"最后一厘米"）
- **SST 固态变压器**：中压 AC → 低压 DC 一步转换，终极方案
- **备电/发电**：柴发（备电）、燃气轮机/气发（主电）
- **保护与监测**：熔断器、固态断路器（SSCB）、母线/配电监测
- **上游元器件**：磁性元件、电容、SiC/GaN 功率半导体

> ⚠️ 液冷/散热不在本页范围，见 [[concepts/aidc-liquid-cooling\|aidc-liquid-cooling]]；整机柜/服务器/光模块等见 [[concepts/aidc-supply-chain\|aidc-supply-chain]]。

## 产业链结构（供电链路）

```
中压10kV电网
   │
   ├─ SST整机 ──────────── 阳光电源(EnerNeo) / 四方股份(量产) / 中国西电(出海) / 金盘科技 / 伊戈尔 / 新风光
   │
   ├─ 800V HVDC 直流母线
   │     ├─ HVDC电源柜 ─── 中恒电气(31%市占第一) / 科华数据 / 科士达 / 维谛(海外)
   │     ├─ PSU/服务器电源 ─ 麦格米特(NV唯一大陆供应商) / 欧陆通 / 台达(海外)
   │     └─ 保护/监测 ──── 良信股份(SSCB) / 泰永长征(SSCB) / 中熔电气(800V熔断器) / 安科瑞(母线监测)
   │
   └─ 三次电源(最后一厘米) ─ 麦格米特 / 台达 / Vicor(海外) / 磁性元件(可立克/京泉华/麦捷科技) / 电容(法拉/江海)
   │
   备电/发电 ─ 柴发(潍柴系) / 燃机·气发(见 [[concepts/gas-turbine\|gas-turbine]]) / 超级电容(合众汇能) / 储能(阳光电源 iPowerCore)
```

### 供电架构三阶段演进

| 阶段 | 方案 | 单柜功率 | 效率 | 时点 |
|------|------|:--:|:--:|------|
| 现状主流 | UPS | <200kW | 90-92% | 当前 |
| **黄金窗口** | 800V HVDC | 600kW→1MW | 98%+ | **2026-2028** |
| 终局 | SST | 1MW+ | 98.5%+ | 2028+ |

^[concepts/800v-hvdc.md]

## 市场空间

| 指标 | 数据 | 来源 |
|------|------|------|
| 2026 HVDC 市场 | ~100 亿元（+180% YoY） | 科智咨询 ^[concepts/800v-hvdc.md] |
| 2027 HVDC 市场 | ~177 亿元 | 科智咨询 |
| HVDC 渗透率(新建) | 2026:20% → 2027:40% → 2030:70% | 国盛证券 |
| 2028 SST 市场 | 562.8 亿元 | 中国银河 |
| 2030 SST 全球市场 | 500-1,000 亿元（数据中心） | 东北证券 |
| 全球 HVDC CR3 | 中恒+台达+维谛 = 95% | 东方财富研究中心 |

^[concepts/800v-hvdc.md] ^[concepts/solid-state-transformer.md]

### 英伟达路线图（供电需求）

| 平台 | 时间 | 单柜功率 | 供电需求 |
|------|------|:--:|------|
| H200 | 2025 | <100kW | 48V/400V |
| GB300/VR200 | 2026-2027 | 200-400kW | 800V HVDC 启动 |
| Rubin Ultra | 2027 | 600kW | 800V HVDC 放量 |
| Feynman | 2028 | 1MW+ | SST 唯一解 |

^[concepts/800v-hvdc.md]

## 主要标的（按环节）

### 🔌 一次电源 / 800V HVDC

| 代码 | 名称 | 一句话逻辑 |
|------|------|-----------|
| [[entities/002364\|002364]] | 中恒电气 | HVDC 国内市占率第一(31%)，800V 直流方舱/Panama，宁德 41 亿增资+员工持股 |
| [[entities/002335\|002335]] | 科华数据 | 高端 UPS 国内第一→HVDC 转型，全球首款 200kW UPS（已澄清未与英伟达合作 ⚠️） |
| [[entities/002518\|002518]] | 科士达 | UPS 国内第二，2026Q2-Q3 推 800V HVDC，UPS 全年指引+30% 间接供谷歌 300MW |

### 🔋 二次电源 / PSU

| 代码 | 名称 | 一句话逻辑 |
|------|------|-----------|
| [[entities/002851\|002851]] | 麦格米特 | 英伟达大陆唯一 AI 电源供应商，Rubin 800V 全系认证，PSU→HVDC→SST 全链路，超容柜获谷歌 V8 标配 |
| [[entities/300870\|300870]] | 欧陆通 | A 股服务器电源营收第一，CRPS→OCP→GPU ATS 三线，800V IBC/DC-DC 新变量 |

### ⚡ SST 固态变压器

| 代码 | 名称 | 一句话逻辑 |
|------|------|-----------|
| [[entities/300274\|300274]] | 阳光电源 | SST 首发龙头 EnerNeo(3MW/98.5%)，光储双龙头，与东阳光/中联数据签 130MW 框架，首家过 NV 储能认证 |
| [[entities/601126\|601126]] | 四方股份 | SST 唯一量产（10kV→800V，2.4MW，年产能 200+台），先发优势最强 |
| [[entities/601179\|601179]] | 中国西电 | 国产 SST 出海第一单（4 台 13.8kV/800V），年内已交付 8 台，2027 批量交付窗口 |
| [[entities/688676\|688676]] | 金盘科技 | 干式变压器全球龙头+「元神ONE」SST 样机，海外 CSP 直连+800V 供电架构受益，在手订单 90 亿+ |
| [[entities/002922\|002922]] | 伊戈尔 | 工业控制变压器+SST 新品发布，美国市场/海外渠道布局 |
| [[entities/688663\|688663]] | 新风光 | SVG 电能质量龙头，2.5MW SST 样机（10kV/800V/2500kW 全栈），9-10 月交付海外 S 厂样机 |

### 🛡️ 保护 / 配电 / 监测

| 代码 | 名称 | 一句话逻辑 |
|------|------|-----------|
| [[entities/002706\|002706]] | 良信股份 | 固态断路器 SSCB 龙头（HVDC/SST 必选保护），英伟达白皮书明确 SSCB 路线 |
| [[entities/002927\|002927]] | 泰永长征 ⚠️ | SSCB 固态断路器先行者，DC800V 落地头部运营商 ⚠️示范落地但业绩变脸 |
| [[entities/301031\|301031]] | 中熔电气 | 800V 熔断器独家龙头，单机柜价值量 5×传统，已批量配套英伟达链 |
| [[entities/300286\|300286]] | 安科瑞 | AIDC 配电/母线监测「卖水人」（3.2 万/柜），发布 SST 全链路监测方案 |

### 🔧 上游元器件

| 代码 | 名称 | 一句话逻辑 |
|------|------|-----------|
| [[entities/002782\|002782]] | 可立克 | SST 高频变压器纯正标的，台达链核心（外购 50-60%），定增扩产 AI 电源磁性元件 |
| [[entities/002885\|002885]] | 京泉华 | SST-MFT 高频变压器卡位最好（伊顿主供+台达配套），单瓦价值量 8-10 倍升级 |
| [[entities/300319\|300319]] | 麦捷科技 ⚠️ | TLVR 电感国产突破，直供英伟达（首个进 GPU 原厂 BOM 的国产 TLVR）⚠️AVL资质未取得 |
| [[entities/002617\|002617]] | 露笑科技 | SiC 衬底（8 英寸稳定量产），SST/SSCB 基石材料 |
| [[entities/688469\|688469]] | 芯联集成 | 3300V SiC MOSFET 填补 SST 核心功率级国产空白（BOM 降 20-35%） |
| 600563 | 法拉电子 | 薄膜电容龙头，SST 用量 3-5 倍（暂无独立实体页） |

### 🏭 备电 / 发电（关联 [[concepts/gas-turbine\|gas-turbine]]）

| 代码 | 名称 | 一句话逻辑 |
|------|------|-----------|
| 000338 | 潍柴动力 | 数据中心柴发+气发双主线，2.5MW 产品 UL 认证提前至 8 月上旬 |
| 000880 | 潍柴重机 | 5.38 亿扩产 6-7MW 天然气发电机组（北美数据中心），柴发景气延续 |
| [[entities/600673\|600673]] | 东阳光 | 与阳光电源签 30MW SST 框架采购，电子材料+算电协同 |

### 🔬 测试设备

| 代码 | 名称 | 一句话逻辑 |
|------|------|-----------|
| [[entities/688551\|688551]] | 科威尔 | 测试电源装备，AI 服务器电源测试设备核心受益 |

> 💡 以上一句话逻辑均来自工作区实体页/概念页/对比页（如 [[entities/002364\|中恒电气]]）；个股深挖见各实体页。

## 🔧 国产替代属性（工作区证据）

> 依据工作区实体页/概念页检索整理，按证据强度分三档；标注来源文件。

### 🟢 第一档：明确"国产替代"表述（14 只）

| 代码 | 名称 | 环节 | 国产替代逻辑 | 来源 |
|------|------|------|------|------|
| [[entities/002851\|002851]] | 麦格米特 | PSU/HVDC | 英伟达大陆唯一 AI 电源供应商，全球仅台达+麦格米特两家过 NV 认证（替代台达垄断） | entities/002851.md |
| [[entities/002364\|002364]] | 中恒电气 | HVDC | 国内市占率 31% 第一 vs 外资维谛 22%，牵头国标+工信部单项冠军（替代维谛） | entities/002364.md |
| [[entities/002706\|002706]] | 良信股份 | 固态断路器/配电 | 明写「AIDC 配电国产替代+海外高毛利」双轮驱动，维谛采购需求 15 亿/年替代空间 | entities/002706.md |
| [[entities/688551\|688551]] | 科威尔 | 电源测试 | AI 服务器电源测试国产替代卡位，外资/台系 Chroma 致茂占主要份额 | entities/688551.md |
| [[entities/300870\|300870]] | 欧陆通 | PSU/IBC | 明写「国产替代：麦格米特之外大陆第二家布局 800V IBC」 | entities/300870.md |
| [[entities/300319\|300319]] | 麦捷科技 ⚠️ | 电感 | TLVR 电感首个进 GPU 原厂 BOM 的国产供应商，替代乾坤(台达)>40% 份额 ⚠️AVL资质未取得 | entities/300319.md |
| [[entities/002617\|002617]] | 露笑科技 | SiC 衬底 | 晶体生长 90% 国产化+12 英寸填补国内空白；英伟达 800V 拉动 SiC 国产化紧迫性 | entities/002617.md、concepts/800v-hvdc.md |
| [[entities/688469\|688469]] | 芯联集成 | SiC 器件 | 3300V SiC MOSFET 填补 SST 核心功率级国产空白（BOM 降 20-35%），8 英寸 SiC 国内首条量产线 | concepts/800v-hvdc.md、entities/688469.md |
| [[entities/002885\|002885]] | 京泉华 | 磁性元件 | 伊顿 SST-MFT 独家配套+BE 全球 90% 磁性元器件主供（国产件打进海外龙头供应链） | entities/002885.md |
| [[entities/002782\|002782]] | 可立克 | 磁性元件 | 台达 SST 链核心供应商（外购 50-60%），AI 电源磁性元件"卖铲人" | entities/002782.md |
| [[entities/002056\|002056]] | 横店东磁 | 磁芯 | 800V IBC 高频磁芯：日系垄断（TDK/FDK/日立），国产替代空间大 | entities/002056.md |
| [[entities/000969\|000969]] | 安泰科技 ⚠️ | 纳米晶磁芯 | 国内纳米晶市占率第一，SST 高频变压器刚需，国产化率 60%→2028E 80% ⚠️SST暂无订单 | entities/000969.md |
| [[entities/601179\|601179]] | 中国西电 | SST | 国产 SST 出海第一单（4 台 13.8kV/800V），vs 台达/伊顿"国产替代逻辑，成本优势" | entities/601179.md |
| [[entities/688676\|688676]] | 金盘科技 | 变压器/SST | 干式变压器全球龙头，美国 69kV 变压器进口禁令豁免（本地化产能+JST 品牌），替代北美进口 | entities/688676.md |

### 🟡 第二档：国产龙头地位明确（隐含替代外资，6 只）

| 代码 | 名称 | 环节 | 依据 |
|------|------|------|------|
| [[entities/002335\|002335]] | 科华数据 | UPS→HVDC | 高端 UPS 国内第一、全球首款 200kW UPS（外资 UPS 传统主导） |
| [[entities/002518\|002518]] | 科士达 | UPS→HVDC | UPS 国内第二（外资艾默生/施耐德主导格局下的国产主力） |
| [[entities/301031\|301031]] | 中熔电气 | 熔断器 | 800V 熔断器独家龙头，已批量配套英伟达链（替代海外熔断器供应） |
| [[entities/601126\|601126]] | 四方股份 | SST | SST 唯一量产（10kV→800V 2.4MW，年产能 200+台） |
| [[entities/688663\|688663]] | 新风光 | SVG/SST | 高压 SVG 国内龙头，2.5MW SST 全栈样机 |
| [[entities/002927\|002927]] | 泰永长征 | SSCB | 国内 SSCB 先行者（概念页标注"国内暂时空白，追赶窗口 18-24 月"） |

### 🔵 第三档：所在环节国产化率低 → 替代空间大

| 环节 | 国产化率 | 受益/相关标的 | 来源 |
|------|:--:|------|------|
| 数据中心柴发 | 17% | 潍柴动力(000338)/潍柴重机(000880) | concepts/gas-turbine.md |
| SiC 器件 | <15% | [[entities/688469\|芯联集成]]/斯达/宏微 | concepts/sic-supply-chain.md |
| 功率半导体整体 | MOSFET 35% / IGBT 25% / SiC <10% | [[entities/603290\|斯达半导]]/[[entities/600460\|士兰微]]/[[entities/688396\|华润微]] | concepts/power-semiconductor.md |
| SST 控制芯片 | 仅 10% | （全链国产化率最低卡点） | concepts/solid-state-transformer.md |
| 燃机整机/零部件 | <5% / ~20% | [[entities/603308\|应流股份]]/[[entities/688239\|航宇科技]]/[[entities/002353\|杰瑞股份]] | concepts/gas-turbine.md |
| 薄膜电容 | 70%→85% | [[entities/600563\|法拉电子]] | entities/600563.md |

> 📌 三档口径：第一档=工作区有明确"国产替代/替代XX/填补空白"表述；第二档=国产市占第一/独家龙头（隐含替代外资）；第三档=低国产化率环节，替代空间最大。
>
> 🔍 可信度交叉验证见 [[reports/260816/AIDC电源国产替代_可信度评估_260816\|AIDC电源国产替代 可信度评估]]（妙想 mx-search/mx-data 全量验证，2026-08-16）。⚠️ 麦捷科技(AVL资质存疑)/安泰科技(SST无订单)/泰永长征(业绩变脸)/科士达(HVDC研发中)/京泉华(MFT小试) 等 claim 有下调提示，详见报告。


| 日期 | 类别 | 事件 | 涉及标的 | 来源 |
|------|:--:|------|------|------|
| 08-16 | 技术 | 直流回归主流：SST 产业化元年报道，伊顿/台达/维谛卡位，四方/西电/阳光率先产品化 | 四方/西电/阳光 | [[reports/260816/每日事件更新_260816\|每日事件更新 260816]] |
| 08-15 | 公司 | 中恒电气：宁德 41 亿增资正式签署+三大领域战略合作 | 中恒电气 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 08-15 | 公司 | 金盘科技海外 CSP 直连+800V 供电架构受益，弗吉尼亚工厂投产 | 金盘科技 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 08-15 | 技术 | 安科瑞发布 SST 全链路监测方案（弧光/测温/绝缘/局放） | 安科瑞 | [[concepts/solid-state-transformer\|solid-state-transformer]] |
| 08-15 | 订单 | 中国西电年内已交付 8 台 SST，2027 批量交付窗口 | 中国西电 | [[concepts/solid-state-transformer\|solid-state-transformer]] |
| 08-14 | 技术 | 英伟达 800VDC 白皮书 2.0：PowerRack 落地、SSCB 固态断路器路线明确 | 良信/中恒 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 08-13 | 公司 | 中恒电气 HVDC+巴拿马电源龙头（市占 70%+），员工持股计划落地 | 中恒电气 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 08-12 | 技术 | NVIDIA 推 800VDC：2027 单机架供电上看 2MW，台北 OCP 聚焦 800V IT Racks | 中恒/麦格米特 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 08-12 | 公司 | 飞龙股份获英伟达认可，将供 800V 高集成电子水泵 | 飞龙股份 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 08-12 | 业绩 | 台达 7 月营收+47.7%，电源及零组件+58.9%，全年 Capex 700 亿扩产 | 台达(海外) | [[concepts/800v-hvdc\|800v-hvdc]] |
| 08-12 | 订单 | 京泉华 SST-MFT 高频变预期 40%+ 份额，伊顿主供完成验证 | 京泉华 | [[concepts/solid-state-transformer\|solid-state-transformer]] |
| 08-12 | 技术 | 新风光 2.5MW SST 样机国内最先一批，9 月底交付海外 S 厂 | 新风光 | [[concepts/solid-state-transformer\|solid-state-transformer]] |
| 08-11 | 量产 | 800V HVDC 26Q3 确定量产（通合科技/新雷能）；SST 2030 全球市场 4166 亿 | HVDC 链 | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 08-10 | 资本 | 英伟达拟 30 亿美元入股 Lancium（首期 20 亿/20%股权），首次重金布局电力基础设施 | — | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 08-08 | 认证 | 阳光电源首家通过 NV 储能认证；玉柴国际数据中心柴发 26H1 出货 1800 台 | 阳光电源 | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 08-08 | 资本 | 英伟达拟向星际之门电力公司投最高 30 亿美元 | — | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 08-06 | 配置 | #AIDC电源# 回调后配置窗口：柜内（麦格米特/欧陆通/奥海）柜外（中恒/科士达/盛弘/科华/英威腾）元器件（宏发/中熔/良信/法拉） | 多标的 | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 08-05 | 量产 | 台达 ±400V/800V HVDC Q3 量产、Q4 出货、2027 产量大增 | 台达(海外) | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 08-02 | 研报 | 广发电新：国内数据中心 800V DC 进展有望超预期 | — | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 08-01 | 业绩 | 伊顿 2Q26 电气收入+26.7%，数据中心订单同比高增、上调全年指引 | 伊顿(海外) | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 07-29 | 订单 | Generac Q2 北美柴发 AIDC 订单每两月翻倍，累计 16 亿美元 | 柴发链 | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 07-27 | 周度 | AIDC 电力周度：Rubin 7/21 批量交付；A 股 AI 电源为海外映射/光补涨，无核心一供 | AI电源链 | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 07-25 | 需求 | 美银：美国数据中心电力需求 2035 年激增 253% 达 194GW（占全美 20%） | 电力设备 | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 07-23 | 订单 | 科士达 UPS 全年指引+30%，间接供谷歌 300MW | 科士达 | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 07-21 | 交付 | 英伟达 Rubin 正式批量交付（CoreWeave/谷歌云/Azure/甲骨文采用 Vera Rubin） | NV链 | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 07-18 | 产业 | 江苏 SST 产业联盟 78 家成员成立（南瑞继保理事长）,"1+4+10"路径 | SST链 | [[concepts/solid-state-transformer\|solid-state-transformer]] |
| 07-16 | 技术 | 国电南瑞发布四款 SST（瑞磐/瑞霆/瑞融/瑞枢）；华润微 SiC 获 SST 备货订单 | SST链 | [[concepts/solid-state-transformer\|solid-state-transformer]] |
| 07-15 | 订单 | 麦格米特超容柜获谷歌 V8 标配（市场约 10 亿美元） | 麦格米特 | [[concepts/aidc-supply-chain\|aidc-supply-chain]] |
| 07-13 | 订单 | 阳光电源 EnerNeo 3MW/98.5%，与东阳光(30MW)/中联数据(100MW)签框架，2027 批量交付 | 阳光电源 | [[concepts/solid-state-transformer\|solid-state-transformer]] |
| 07-11 | 技术 | 英伟达与台达合作开发 600kW 级 SST（98.2%，580W/in³） | 台达(海外) | [[concepts/solid-state-transformer\|solid-state-transformer]] |
| 07-10 | 落地 | 字节 AI Rack 3.0：800V HVDC+100% 全液冷，单柜 500kW/双柜 1MW（OCP 峰会） | 中恒/麦格米特/科华 | [[concepts/byte-ai-power\|byte-ai-power]] |
| 07-09 | 发布 | 阳光电源首发全自研 SST EnerNeo，微软/AWS/阿里云/腾讯/字节出席 | 阳光电源 | [[concepts/byte-ai-power\|byte-ai-power]] |
| 07-01 | 政策 | 美国逆变器禁令发酵（影响储能/逆变器出口，非 AIDC 供电主线）⚠️关联事件 | 阳光电源等 | [[zsxq/events/us-inverter-ban/index\|美国逆变器禁令]] |
| 06-30 | 深度 | AIDC 全固态配电生死局：SiC 模块是 SST/SSCB 基石；英伟达 800V 拉动 SiC 国产化 | SiC链 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 06-29 | 研报 | 国盛证券：AI 电源高景气延续，800V HVDC 全球 2031E 608 亿美元 | HVDC链 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 06-29 | 澄清 | 科华数据澄清尚未与英伟达合作，出海是重要战略 ⚠️ | 科华数据 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 06-28 | 量产 | TrendForce：英伟达 800V Power Rack 2026Q3 完成备货，Vera Rubin 客户选用 | NV链 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 06-23 | 器件 | 芯联动力 3300V SiC MOSFET，填补 SST 核心功率级国产空白，BOM 降 20-35% | 芯联集成 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 06-17 | 格局 | 东方财富研究中心：国内 HVDC 格局中恒 31%/维谛 22%/科华 19%/中兴 11% | 中恒/科华 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 06-15 | 订单 | 中国西电斩获海外数据中心 SST 订单（4 台 13.8kV/800V）——国产 SST 出海第一单 | 中国西电 | [[concepts/solid-state-transformer\|solid-state-transformer]] |
| 06-15 | 技术 | 英伟达+谷歌提前推进 800V HVDC，Q3 小批量出货 | NV链 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 06-11 | 研报 | 两大券商分歧：AI 电源龙头普跌，科士达 Q2-Q3 推 800V，麦格米特最早进 NV 认证 | 科士达/麦格米特 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 06-08 | 示范 | 青岛"算电岛"：特来电 HVDC→SST 演进，220kV 直入 800VDC，2027 挂网示范 | SST链 | [[concepts/800v-hvdc\|800v-hvdc]] |
| 06-02 | 生态 | 安森美加入英伟达 MGX 生态，布局 800V DC 电源架构 | — | [[concepts/800v-hvdc\|800v-hvdc]] |

> 📌 时间线仅收录 2026-05-15 之后事件；更早背景见"历史报告与背景资料"。美国逆变器禁令为关联事件（储能/逆变器），非 AIDC 供电主线。

## 历史报告与背景资料

- `reports/260701/AIDC产业链_行业分析_260701.md` — AIDC 全产业链（供电+液冷+元器件）
- `reports/260616/800V HVDC_行业分析_260616.md` — 800V HVDC 行业分析
- `reports/260617/HVDC_最新投研动态_260617.md` — HVDC 最新投研动态
- `reports/260613/固态变压器_行业分析_260613.md` — 固态变压器行业分析
- `reports/260710/阳光电源_全面分析_260710.md` — 阳光电源全面分析
- `reports/250618/AIDC液冷产业链_行业分析_250618.md` — AIDC 液冷（背景）
- `raw/articles/800V HVDC 砖块电源技术深度解析…` — 三次电源/砖块电源技术深文
- `raw/articles/离 GPU 最近的最后一厘米…` — 供电成为芯片终极瓶颈
- `raw/articles/SST产业链全景…` — SST 产业链全景
- `raw/papers/800V_HVDC_SST_20260413.md` — 800V HVDC/SST 研报 OCR

## 相关概念

- [[concepts/800v-hvdc\|800v-hvdc]] — 800V HVDC 高压直流供电（细分概念）
- [[concepts/solid-state-transformer\|solid-state-transformer]] — 固态变压器 SST（细分概念）
- [[concepts/byte-ai-power\|byte-ai-power]] — 字节 AI 电源（800V 落地标杆）
- [[concepts/aidc-supply-chain\|aidc-supply-chain]] — AIDC 全产业链（上位概念）
- [[concepts/aidc-liquid-cooling\|aidc-liquid-cooling]] — AIDC 液冷（关联，不在本页范围）
- [[concepts/power-semiconductor\|power-semiconductor]] — 功率半导体（上游器件）
- [[concepts/sic-supply-chain\|sic-supply-chain]] — 碳化硅产业链（上游材料）
- [[concepts/gas-turbine\|gas-turbine]] — 燃气轮机（发电/备电）
- [[concepts/virtual-power-plant\|virtual-power-plant]] — 虚拟电厂（算电协同）
- [[concepts/nvidia-rubin\|nvidia-rubin]] — NVIDIA Rubin 产业链（需求驱动）

## 对比页

- [[comparisons/ai-power-three-stocks\|ai-power-three-stocks]] — 阳光电源 vs 麦格米特 vs 中恒电气
- [[comparisons/hvdc-three-stocks\|hvdc-three-stocks]] — 锐明 vs 中熔 vs 明阳（HVDC 三股）

## 核心结论

> 🔥 **AIDC 供电架构正经历 UPS→800V HVDC→SST 三阶段确定性演进**：英伟达 800V 白皮书 2.0 + 字节 AI Rack 3.0 落地，2026-2028 是 HVDC 黄金窗口，SST 2028+ 终局。A 股核心标的按环节卡位：HVDC 看中恒电气，PSU 看麦格米特，SST 看阳光电源/四方/西电/金盘，保护器件看良信/泰永/中熔，元器件看可立克/京泉华/麦捷。
>
> ⚠️ 板块处于 0→1 早期，PE 普遍偏高（HVDC 龙头 ~100x，NV 链 400x+），2026H2-2027 是业绩验证期，注意订单节奏与技术路线（800V vs ±400V）风险。

## 📝 更新日志

| 日期 | 更新内容 | 来源 |
|------|------|------|
| 2026-08-16 | 追加：国产替代可信度评估报告链接（妙想 mx-search/mx-data 全量验证），麦捷/安泰/泰永加注⚠️ | 妙想验证 |
| 2026-08-16 | 追加：国产替代属性三档清单（明确表述14只/龙头6只/低国产化率环节） | 工作区整合 |
| 2026-08-16 | 新建：AIDC 电源总览页（概念/标的/近3个月新闻时间线），严格供电链路口径 | 工作区整合 |
