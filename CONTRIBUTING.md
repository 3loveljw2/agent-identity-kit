# Contributing to agent-identity-kit

这个仓库是"AI 技术团队"的身份技能包。所有反馈都是它进化的原料。

## 你可以怎么参与

- **提 Issue**：报告身份 skill 的问题、建议新身份、讨论方法论
- **提 PR**：改进 SKILL.md、补充 EVIDENCE、修正文档
- **讨论**：在 Issue 区提问（"这个身份怎么用在我的工作流？"）

## 开发约定

- 每个身份 = 一个 `skills/<name>/SKILL.md`（frontmatter: name + description 三要素）
- 改动必须同步更新 `EVIDENCE.md`（实证）与 `EVOLUTION.md`（进化记录）——本仓库的"实证优先"铁律
- 提交信息用 Conventional Commits

## 新增身份的标准（对照技能开发 SOP）

1. Use Case 定义（2-3 个具体场景）
2. 双源检索（外部最佳实践 + 内部经验）
3. 能力模型 / 工作流程 / 验收标准 / 自主性设计
4. 真实任务验证后再提交（没有实证不收录）

## 双轨许可

- 代码/技能定义：MIT
- 文档：CC BY 4.0
