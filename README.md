# Agent Identity Kit · AI 技术团队身份技能包

> **给任何 AI 编码助手一支"技术团队"——10 个可加载的身份技能，会进化，带实证。**
> Built by a 16-year-old · 用 AI 从零搭建系统的一年沉淀

## 这是什么

一个 **Agent 身份技能包**：10 个可加载的 AI 子代理身份（SKILL.md 格式，Claude Code / Cursor / Codex / Gemini CLI 均兼容），覆盖开源项目全链路：

| 身份 | 职责 | 产出 |
|---|---|---|
| **Technical Architect** 技术架构师 | 方法论 → 技术规格（5C 模块化 / ADR / 选型） | ARCHITECTURE.md + 骨架 |
| **Implementation Engineer** 实现工程师 | 规格 → 能跑能装的 CLI/脚本（Typer / 类型完备） | pip install 的包 |
| **Quality Reviewer** 质量审查官 | 独立质量门禁（测试金字塔 / 防自证陷阱） | tests + CI + 审查报告 |
| **Technical Writer** 文档工程师 | 30 秒看懂 / 5 分钟跑通（README 五件套，英文全包） | README + docs/ |
| **Release Engineer** 发布工程师 | semver / CHANGELOG / PyPI / LICENSE 一条龙 | 版本 + Release |
| **Demo Engineer** 演示工程师 | 能跑的例子证明方法论有效 | examples + GIF |
| **Security Auditor** 安全审计官 | 公开前安全审查（OWASP MCP / 密钥 / 依赖） | SECURITY.md + 报告 |
| **Community Maintainer** 社区维护官 | Issue/PR / 24h 响应 / 贡献者留存 | 模板 + 话术 |
| **Planner** 策划官 | 碎片想法 → 带验收标准的规格（PRD / 范围控制） | PRD + Roadmap |
| **Memory Curator** 记忆管家（元身份） | AGENTS.md / 组织伤疤 / 技能自举 | 规则 + 复盘 |

## 为什么这个技能包不一样

**① 自进化（Self-Evolving）**
这不是静态的技能文件集。每个身份按"蒸馏机制"运转：任务留痕 → 经验提炼 → 技能更新，进化记录在 [EVOLUTION.md](EVOLUTION.md) 公开可见，踩坑教训在 [LESSONS.md](LESSONS.md) 公开可查——**你 star 的是一个每周在变聪明、且把错误也摊开给你看的团队**。

**② 实证优先（Evidence-First）**
2026 年 GitHub 被 AI 生成内容淹没，"可验证的真人真实产出"是稀缺信任品。每个身份的能力都有真实使用证据（见 [EVIDENCE.md](EVIDENCE.md)）：7/7 通过的测试、565 份真题题库、99 条任务记录、多轮实战——不是 PPT。

**③ 双路径（Two Paths）**
不给你唯一的死路径：**落地即用**（通用最优）或**自适应探索**（[EXPLORE.md](EXPLORE.md)，你的 Agent 扫描环境→试验→蒸馏→形成你环境的最优）。方法论不变，交付形态你选。

**④ 少年造 AI（16 y/o）**
这个技能包不是课堂作业：它来自一个 16 岁少年用 AI 从零搭建学习系统的一年实战——由它管理的系统真实撑起了 565 份真题题库、AI 出卷引擎、官网多页站。

## 快速开始：两条路，你选

**路径 A · 落地即用（快车道，30 秒）**

```bash
git clone https://github.com/3loveljw2/agent-identity-kit.git
cp -r agent-identity-kit/skills/* ~/.claude/skills/   # Claude Code
# 或 Cursor / Codex / Gemini CLI 的对应 skills 目录
```

加载后，Agent 立即拥有 10 个身份的**核心能力 + 工作流程 + 交付物模板 + 验收标准 + 自主性边界**。

**路径 B · 自适应探索（定制化，让 Agent 找到你环境的最优）**

不满足于"通用最优"？按 [EXPLORE.md](EXPLORE.md) 协议走：你的 Agent 扫描你的环境 → 评估匹配度 → 小规模试验 → 蒸馏适配 → 形成**你的个人化技能包**，并持续进化。

> 两条路共享同一套方法论（10 身份能力不变），区别只在交付后是否再适配。建议先用 A 跑通，再决定要不要走 B 深挖。

## 进化协议（如何贡献/如何让技能包成长）

见 [AGENTS.md](AGENTS.md)——六域操作手册 + 蒸馏机制说明。核心：

```
用技能包做任务 → 任务留痕（task-log）→ 满 N 条触发蒸馏 → 提炼共性
→ 更新对应 SKILL.md（版本 +1）→ 记录进 EVOLUTION.md
```

## 文档

- [AGENTS.md](AGENTS.md) — AI 操作手册（怎么用/怎么进化）
- [EXPLORE.md](EXPLORE.md) — **路径 B 自适应探索协议**（让 Agent 找到你环境的最优）
- [EVOLUTION.md](EVOLUTION.md) — 进化日志（版本历史，公开可见的成长记录）
- [EVIDENCE.md](EVIDENCE.md) — 实证清单（能力可信度证据）
- [LESSONS.md](LESSONS.md) — **踩坑日志**（真实错误与教训，组织伤疤——为什么这些技能可靠）
- [llms.txt](llms.txt) — AI 索引
- [docs/design.md](docs/design.md) — 技能包设计哲学

## 配套资产（同一作者的生态）

- [self-evolving-agent](https://github.com/3loveljw2/self-evolving-agent) — 这套技能包的"记忆系统底座"（五层架构 + 蒸馏机制）
- [trace-dig-method](https://github.com/3loveljw2/trace-dig-method) — 技能包内部的方法论引擎（溯源深挖法）
- [autonomous-proposition](https://github.com/3loveljw2/autonomous-proposition) — 技能包实战产出（AI 出卷方法论）

## License

[CC BY 4.0](LICENSE) — 署名即可自由使用、修改、分享。你的 Agent 团队，随时带走。

---

⭐ 如果这套身份技能包对你有用，点个 star——让更多 AI 拥有"越用越懂自己"的团队。
