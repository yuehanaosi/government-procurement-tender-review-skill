# 政府采购与招投标响应文件审核
# Government Procurement and Tender Response Review

面向政府采购及招投标业务的中英双语 Codex Skill。适用于供应商递交前自查、采购人或代理机构材料核对，以及同一项目多家供应商响应文件的逐家复核。审核以项目条款、正式政策来源和文件证据为基础。每项问题可追溯到具体表格、页码和依据，便于修改、复核与归档。

A bilingual Codex skill for government procurement and tendering. It supports supplier pre-submission checks, document verification by purchasers or agents, and separate reviews of multiple submissions for one project. Findings are grounded in project clauses, official policy sources and documentary evidence. Each finding identifies its form, page and governing requirement for correction, verification and recordkeeping.

## 适用范围 / Scope

适用于中国大陆政府采购货物、服务和工程等项目，覆盖政府采购招标、竞争性磋商、竞争性谈判、询价及适用招标投标法的工程建设项目。政策索引覆盖大陆31个省级行政区，并列明计划单列市及新疆生产建设兵团查询路径。香港、澳门另列官方入口，按各自制度核验。涉及国企或其他招标采购时，先确定适用制度和监管范围。

Designed for goods, services and works procurement in mainland China, including government procurement tendering, competitive consultation, negotiation, quotation requests and construction projects governed by bidding legislation. The source index covers all 31 provincial-level jurisdictions in mainland China, with separate lookup paths for cities with independent planning status and the Xinjiang Production and Construction Corps. Hong Kong and Macao official portals are listed for independent verification under their respective rules. For state-owned enterprise or other procurement, establish the governing regime and regulator first.

## 主要能力 / Review capabilities

- **政策适用与项目依据 / Applicable policy and project documents.** 确认采购方式、项目类别及监管范围，核实中央和地方现行及项目适用规则，检查项目公告、采购文件和补遗。 / Identify the procedure, subject matter and regulator, verify national and local rules applicable to the project, and check notices, solicitation documents and addenda.
- **资格、授权与签章 / Eligibility, authority, signatures and seals.** 核对营业执照、资格声明、法定代表人证明、授权委托书、生效日期及签章位置。分别记录 PDF 可见签章和电子签章验证状态。 / Verify business licenses, eligibility declarations, legal representative identification, powers of attorney, effective dates and execution fields. Record visible marks and digital validation status separately.
- **报价、保证金和期限 / Pricing, bid security and timing.** 复算分项与总价，核对限价、大小写、保证金、提交方式、有效期和履约期限。 / Recalculate unit-price extensions and totals. Check ceilings, numeric and written amounts, bid security, submission method, validity and performance dates.
- **技术商务与评分 / Technical and commercial responsiveness and scoring.** 对照设备参数、供货范围、交付与验收、评分证据和价格优惠声明，报告确有依据的差异及待核验事项。 / Cross-check specifications, supply scope, delivery and acceptance, scoring evidence and preference declarations. Report supported discrepancies and open verification items.
- **文字与证据定位 / Editorial review and evidence location.** 查错字、错年份、错文号、模板残留和前后冲突。逐家出具问题清单，注明 PDF 页码、条款、影响和处理动作。 / Spot typos, incorrect years, citation errors, template remnants and inconsistencies. Deliver a separate issue list for each supplier, including the page, clause, impact and corrective action.

## 安装和使用 / Installation and usage

将本仓库完整复制到 Codex 的技能目录 `~/.codex/skills/government-procurement-tender-review`，并在 Codex 中调用 `$government-procurement-tender-review`。提交采购文件、补遗及响应文件，说明需要核对的版本。已上传的项目可一并提供交易回执及最终电子签章文件。

Copy this repository to `~/.codex/skills/government-procurement-tender-review` and invoke `$government-procurement-tender-review` in Codex. Supply the procurement documents, addenda and responses, and identify the intended versions. For submitted projects, include the receipt and final electronically signed documents when available.

> 使用该 Skill 核对各供应商响应文件，按公司列出问题，标注 PDF 阅读器页码、采购依据及处理意见，输出中英双语。  
> Use this skill to review each supplier’s response. Report exceptions by supplier, with PDF viewer pages, the basis for each finding and the action required. Deliver the findings in Chinese and English.

## 文件索引 / Repository contents

| 文件 / File | 内容 / Purpose |
|---|---|
| [SKILL.md](SKILL.md) | 审核入口及执行指令 / Skill entry point and instructions |
| [agents/openai.yaml](agents/openai.yaml) | 双语显示名称及调用提示 / Bilingual display name and invocation prompt |
| [政策来源 / Policy sources](references/policy-sources.md) | 全国法规、地方检索入口和适用性核验 / National law, local lookup routes and applicability checks |
| [审核程序 / Review procedure](references/review-procedure.md) | 审核要点、证据要求和双语输出范例 / Review checks, evidence requirements and bilingual example |

具体项目的结论取决于当时适用的政策、有效采购文件和实际提交的版本。资格、否决和得分由有权主体依法判断。英文译文用于业务理解，法规及项目文件以官方文本为准。

Project conclusions depend on the applicable rules, operative procurement documents and submitted versions. The responsible body determines eligibility, rejection and scoring. English translations support business use; consult official texts for the controlling wording.
