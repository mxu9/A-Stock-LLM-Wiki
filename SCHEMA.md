# Wiki Schema

## Domain
A股投研知识库 — 覆盖A股上市公司分析、行业产业链研究、估值模型、事件驱动分析及市场动态。

## Conventions
- File names: lowercase, hyphens, no spaces (e.g., `hualu-hengsheng.md`)
- 中文标题在 frontmatter `title` 中体现，文件名用拼音/英文简写
- Every wiki page starts with YAML frontmatter (see below)
- Use `[[wikilinks]]` to link between pages (minimum 2 outbound links per page)
- When updating a page, always bump the `updated` date
- Every new page must be added to `index.md` under the correct section
- Every action must be appended to `log.md`
- **Provenance markers:** On pages that synthesize 3+ sources, append `^[raw/reports/report-name.md]`
  at the end of paragraphs whose claims come from a specific source.

## Frontmatter
```yaml
---
title: 页面标题
created: YYYY-MM-DD
updated: YYYY-MM-DD
type: entity | concept | comparison | query | summary
tags: [from taxonomy below]
sources: [raw/reports/report-name.md]
# Optional quality signals:
confidence: high | medium | low
contested: true
contradictions: [other-page-slug]
---
```

## Stock Code Convention
个股 entity 页面的文件名使用股票代码，如 `002819.md`（东方中科）、`600426.md`（华鲁恒升）。
frontmatter 中 `stock_code` 字段标注代码，`title` 标注简称。

## raw/ Frontmatter
报告源文件 frontmatter：
```yaml
---
source_path: reports/260617/华鲁恒升_全面分析_260617.md
ingested: YYYY-MM-DD
report_type: 全面分析 | 行业分析 | 估值分析 | PEG分析 | 事件分析 | 行情分析 | 星球追踪 | 摘要 | 对比
---
```

## Tag Taxonomy
- **个股标签:** 个股, 化工, 电力设备, 银行, 电子, 汽车, 机械, 有色, 医药, 农业, 新能源, 人形机器人, 金融, 半导体, MLCC, MLCC上游, MLCC涨价, 商业航天, 先进封装
- **行业/概念标签:** 行业分析, 产业链, HVDC, 液冷, 固态变压器, 燃气轮机, 碳酸锂, 油运, HBM, 对日替代, AIDC, 军工, 国产替代, 激光光源, 航运, 光通信, 测试设备, 被动元件, 涨价, 商业航天, 卫星互联网, 6G
- **AI/算力标签:** AI
- **分析类型标签:** 全面分析, 估值分析, PEG分析, 事件分析, 行情分析, 对比分析
- **来源标签:** 知识星球, 妙想数据, tushare数据
- **Meta:** 催化剂, 市场动态, 宏观

Rule: every tag on a page must appear in this taxonomy. If a new tag is needed, add it here first.

## Page Thresholds
- **Create entity page** for every A-share stock analyzed in any report
- **Create concept page** for every industry/产业链/概念 that appears in 2+ reports
- **Add to existing page** when a report updates an already-covered stock/concept
- **DON'T create a page** for passing mentions of unrelated stocks
- **Split a page** when it exceeds ~200 lines

## Entity Pages (个股)
One page per stock. Include:
- 公司概况 / what it is
- 核心业务与行业定位
- 关键财务数据（latest from reports）
- 估值分析摘要
- 催化剂与风险
- 相关行业 [[wikilinks]]
- Report references

## Concept Pages (行业/概念)
One page per industry or concept. Include:
- 定义与范围
- 产业链结构
- 主要标的与对比
- 行业催化剂与趋势
- 相关概念 [[wikilinks]]

## Comparison Pages
Side-by-side analyses of 2+ stocks or industries. Include:
- 对比维度与表格
- 核心差异点
- Verdict or synthesis

## Query Pages
Filed valuable research answers that would be painful to re-derive.

## Update Policy
When new report conflicts with existing knowledge:
1. Check report dates — newer reports generally supersede
2. If genuinely contradictory, note both positions with dates and sources
3. Mark `contested: true` + list contradictions
4. Flag for review
