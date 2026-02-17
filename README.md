# OpenClaw & Moltbook Research Project

## 项目简介

探索 OpenClaw 爆火带动的 Moltbook（纯 AI 交互社交媒体）引发的研究机会。

**核心问题**: 当社交互动的参与者从"人-人"变成"人-AI"甚至"AI-AI"时，社交媒体的本质会发生什么变化？

## 研究目标

产出 3-5 个高质量的 Human-AI Social Interaction 研究想法，每个 idea 包含：
- 明确的研究问题 (Research Questions)
- 扎实的动机 (Motivation)
- 清晰的目标 (Objectives)
- 真正的创新点 (Novelty)
- 诚实的挑战分析 (Challenges)
- 可验证的参考文献 (References)

## 文件结构

```
.
├── README.md              # 本文件
├── ideas/                 # 研究想法
│   ├── ideas-v1.md        # 第一轮：5个初步想法
│   └── ...                # 后续迭代
├── papers/                # 相关论文笔记
│   └── paper-notes.md
├── memory/                # 调研过程中的发现
│   ├── insights.md        # 灵感记录
│   └── daily-updates.md   # 每日更新
└── skills/                # 项目专用技能
    └── research-swarm.md  # Agent Swarm 协作规范
```

## 当前进展

| 轮次 | 日期 | 主要产出 | 状态 |
|------|------|----------|------|
| 1 | 2026-02-17 | 初始调研 + 5 个 research ideas | 待 Agent Swarm 评估 |

### 第一轮研究想法概览

1. **观察者效应**: 人类作为旁观者在纯 AI 社交网络中的心理机制
2. **涌现社会规范**: AI 社区中社会规范的自发形成与演化
3. **危机传播**: AI 中介环境中的旁观者效应与有害信息传播
4. **Persona 漂移**: 长期社交中 AI 角色一致性的变化
5. **涌现语言**: AI 代理是否会发展出人类无法理解的语言

详见 [ideas/ideas-v1.md](ideas/ideas-v1.md)

## 研究方法论

采用 **Agent Swarm** 协作模式：
- **Researcher Agent**: 调研文献，提出 ideas
- **Supervisor Agent**: 批判性评估 ideas 的学术价值
- **Engineer Agent**: 评估实现可行性
- **Orchestrator**: 整合输出，统筹迭代

## 迭代原则

- **最小修改原则**: 每次迭代基于上一轮，不推翻重来
- **持续收敛**: 逐步精炼 ideas，而非不断发散
- **证据驱动**: 每个 claim 都要有可追溯的 source

## 自动化

- 每日自动调研最新论文（cron 任务）
- 自动更新参考文献和想法

## 贡献者

- **研究者**: [brianleixia](https://github.com/brianleixia)
- **研究方向**: LLM/Agents Social Intelligence, Societal AI, Collective Intelligence

## 许可

MIT License
