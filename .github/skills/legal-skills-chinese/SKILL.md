---
name: legal-skills-chinese
description: 为法学论文研究、法律资料归纳、法律解释、论证组织与检查、法条和案例核验选择并读取本仓库的中文法律技能。用户要求梳理文献、比较规范、分析制度、完善法律论证或核对引用时使用；按任务调用已有检索工具并保留来源，未接入数据库时明确标注待查。
---

# 中文法学研究技能导航

阅读[仓库规则](../../../AGENTS.md)，从下列导航选择所需技能，实际打开对应的中文 `SKILL.md` 后执行。所有源文件都位于仓库根目录 `skills/`；相对链接从本文件所在目录解析。参照[项目说明及许可](../../../README.md)，保留原始技能内容与署名。

## 执行顺序

1. 从用户请求和材料中确定研究问题、法域、适用时间及材料范围。沿用用户已经明确的条件；缺失信息影响结论时说明假设或询问关键问题。涉及香港、澳门或域外法时，明确采用相应法域的前提，不直接套用中国大陆法源及解释规则。
2. 选择最贴合任务的一个主导技能，完整读取其步骤与能力边界，再按需读取关联技能。论文研究优先考虑多源文档归纳、概念理解、法律解释和论证评估；仅在用户提出对应实务任务时使用判决预测、文书生成或案件管理技能。不要一次加载全部技能，也不要仅凭导航标题执行。
3. 需要核对法条、案例、学术观点或事实数据时，实际调用已连接的检索工具或读取用户提供的原文。记录出处、版本或日期及支持具体结论的位置；检索不足时保留问题，明确标注未核实部分。
4. 按用户要求的格式输出结论、依据、论证过程、相关反对意见与不确定处。清楚区分原材料内容、作者或机构的观点以及本次分析的推断。

## 引用与材料使用

- 不编造法律名称、条号、条文、案号、裁判要旨、效力状态、作者、题名、DOI、引文或页码。按适用时点核对规范版本，避免以今天的版本代替历史版本。
- 保留来源链接和必要的出处信息，引用到能够支持相应主张的位置。沿用用户指定的引注规范；已有准确引用无需改写。
- 仅读过摘要、检索片段或二手转述时，如实说明材料范围；不要把摘要当作全文，不要把转引写成直接阅读，不补写未经核对的原文页码。
- 资料不足仍可提供研究问题、分析框架与检索计划；将需要后续核实的具体内容标注为 `[待检索]` 或 `[待查]`，不要据此形成确定性结论。

## 已连接工具的使用

本导航和源技能本身不提供数据库访问权限。先查看当前环境实际可用的工具，再按工具说明选择与执行；下列名称是服务器配置名，不是可以臆造调用的函数名。

| 服务器配置名 | 选择的工具用途 |
|---|---|
| `pkulaw-law-search` | 检索法规与法条 |
| `pkulaw-case-search` | 检索司法案例 |
| `pkulaw-citation-validator` | 核对法条引用与原文 |

仅在连接可用且调用成功后依据返回结果引用。未连接、调用失败或结果不足时明确告知并标注待查；不能以模型记忆冒充已完成的数据库核验。实际服务地址、参数和工具能力以[北大法宝官方接入文档](https://mcp.pkulaw.com/docs)及已连接接口为准；[仓库接入说明](../../../MCP-PKULAW.md)用于查找背景与相关技能说明。不要将 Token 或其他凭证写入仓库。

## 技能导航

### 1. 信息检索

- [案例检索](../../../skills/case-retrieval/SKILL.md)
- [法条检索](../../../skills/legal-article-retrieval/SKILL.md)
- [其他法律资料检索](../../../skills/other-legal-retrieval/SKILL.md)
- [法律规范效力检查](../../../skills/legal-norm-validity-check/SKILL.md)
- [法律概念理解](../../../skills/legal-concept-comprehension/SKILL.md)

### 2. 事实与要素处理

- [法律要素提取](../../../skills/legal-element-extraction/SKILL.md)
- [结构化要素提取](../../../skills/structured-element-extraction/SKILL.md)
- [争议焦点识别](../../../skills/dispute-issue-identification/SKILL.md)
- [证据评估](../../../skills/evidence-evaluation/SKILL.md)

### 3. 法律解释

- [法律解释论证](../../../skills/legal-interpretation-argument/SKILL.md)
- [体系解释](../../../skills/systematic-interpretation/SKILL.md)
- [目的解释](../../../skills/teleological-interpretation/SKILL.md)
- [规范意义论证](../../../skills/Normative-Meaning-Argumentation/SKILL.md)

### 4. 法律推理

- [演绎推理](../../../skills/deductive-reasoning/SKILL.md)
- [归纳推理](../../../skills/inductive-reasoning/SKILL.md)
- [类比推理](../../../skills/analogical-reasoning/SKILL.md)
- [法律溯因推理](../../../skills/Legal-Abductive-Reasoning/SKILL.md)
- [反事实推理](../../../skills/counterfactual-reasoning/SKILL.md)
- [法律后果推导](../../../skills/formal-legal-consequence/SKILL.md)
- [冲突解决](../../../skills/conflict-resolution/SKILL.md)

### 5. 论证组织与评估

- [论证链构建](../../../skills/argument-chain-construction/SKILL.md)
- [论证强度评估](../../../skills/argument-strength-evaluation/SKILL.md)
- [证据论证链](../../../skills/evidence-argument-chain/SKILL.md)
- [风险优先级排序](../../../skills/strategic-risk-prioritization/SKILL.md)

### 6. 风险评估与价值判断

- [争议与履约风险](../../../skills/dispute-and-performance-risk/SKILL.md)
- [内部合规风险识别](../../../skills/internal-compliance-risk-identification/SKILL.md)
- [法律风险评估](../../../skills/legal-risk-assessment/SKILL.md)
- [司法价值判断](../../../skills/judicial-value-judgment/SKILL.md)
- [行政价值判断](../../../skills/administrative-value-judgment/SKILL.md)
- [法律判决预测](../../../skills/legal-judgment-prediction/SKILL.md)

### 7. 文书与事务管理

- [多源文档归纳](../../../skills/multi-document-summarization/SKILL.md)
- [法律文书摘要](../../../skills/legal-document-summarization/SKILL.md)
- [法律术语规范](../../../skills/legal-terminology/SKILL.md)
- [法律文书格式适用](../../../skills/legal-document-formatting/SKILL.md)
- [裁判文书生成](../../../skills/judgment-document-generation/SKILL.md)
- [案件流程规划](../../../skills/case-lifecycle-planning/SKILL.md)
- [审理排期与期限监测](../../../skills/trial-scheduling-and-deadline-monitoring/SKILL.md)
- [工时与诉讼预算](../../../skills/billing-and-litigation-budget/SKILL.md)
