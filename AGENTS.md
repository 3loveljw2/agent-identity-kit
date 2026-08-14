# AGENTS.md · Agent Identity Kit 操作手册

> 给 AI 编码代理看的手册（也给人看）。回答：这个仓库是什么、怎么用、怎么进化、边界在哪。

## 一、仓库是什么

10 个可加载的 Agent 身份技能（SKILL.md），每个身份 = 一个"子代理角色定义"（身份声明 / 核心能力 / 工作流程 / 交付物模板 / 验收标准 / 自主性设计）。

## 二、常用命令

```bash
# 查看全部身份
ls skills/
# 查看某个身份的完整定义
cat skills/technical-architect/SKILL.md
# 加载单个身份（复制给 Agent）
# 快速开始见 README.md
```

无构建、无依赖、纯 Markdown——**这个仓库不需要运行，只需要读取**。

## 三、结构

```
skills/{identity}/SKILL.md    # 10 个身份技能
EVOLUTION.md                  # 进化日志（版本 + 每次更新的原因）
EVIDENCE.md                   # 实证清单（每个身份的可信度证据）
AGENTS.md                     # 本文件
llms.txt                      # AI 索引
docs/design.md                # 设计哲学
```

## 四、内容规范（写/改 skill 时）

1. 每个 SKILL.md 必须含：frontmatter（name/description 三要素）+ 身份声明 + 核心能力模型 + 工作流程 + 交付物模板 + 验收标准 + 自主性设计
2. description 三要素：功能 + 触发关键词 + 边界/负向场景（防误触发）
3. 身份型 skill 高自主性（给原则+边界，允许动态调整）；流程型低自主性（固定脚本）
4. 引用事实必须有证据（实证优先原则）：能力描述落到 EVIDENCE.md 可查

## 五、进化协议（核心机制）

```
1. 用技能包完成真实任务 → 写 task-log 留痕（日期/任务/产出/踩坑）
2. 经验累积（约每 10 条任务）→ 触发蒸馏：
   a. 聚类：哪些经验是共性规律？
   b. 提炼：写进哪个身份的 SKILL.md？新增还是修改？
   c. 版本 +1：SKILL.md 版本号递增
3. 每次进化记录进 EVOLUTION.md（版本/日期/改了什么/为什么）
4. 实证同步：EVIDENCE.md 更新（新的任务证据）
```

**铁律**：
- 蒸馏结果写入长期知识必须经过确认（防记忆污染）
- 只追加不覆盖：旧版本信息保留在 EVOLUTION.md 历史区
- 不记录敏感信息（密钥/隐私）

## 六、边界（永不触碰）

- 不把技能包用于生成恶意/违法内容
- 不删除或改写他人贡献的 SKILL.md 核心方法论（只做版本演进）
- 敏感信息（API key / 个人隐私）绝不写入本仓库任何文件
- 身份技能只做"角色能力定义"，不做"用户决策"——决策权永远在人

## 七、贡献指南

1. 新增身份：先查 EVOLUTION.md 确认无重复 → 按"内容规范"写 SKILL.md → 更新 README 表格 + llms.txt + EVOLUTION.md
2. 改进身份：版本 +1 → 记录变更原因到 EVOLUTION.md → 同步 EVIDENCE.md
3. 提交信息遵循 Conventional Commits（feat/fix/docs）
