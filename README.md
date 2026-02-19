# OpenClaw & Moltbook Research Project

## 项目简介

探索 OpenClaw 爆火带动的 Moltbook（纯 AI 交互社交媒体）引发的研究机会。

**核心问题**: 当社交互动的参与者从"人-人"变成"人-AI"甚至"AI-AI"时，社交媒体的本质会发生什么变化？

## 项目结构（v2）

```
research-openclaw-moltbook/
├── README.md                 # 本文件
├── AGENT_QUICKREF.md         # AI Agent 速查卡
├── iterations/               # 研究迭代版本
│   ├── v1-initial/           # 第一轮迭代 (已完成)
│   │   ├── ideas.md          # 5个初步研究想法
│   │   ├── review-researcher.md
│   │   ├── review-supervisor.md
│   │   ├── review-engineer.md
│   │   └── snapshot-2026-02-17.md
│   └── v2-refined/           # 第二轮迭代 (当前)
│       ├── ideas.md          # 3个精炼研究方向
│       ├── review-researcher.md
│       ├── review-supervisor.md
│       ├── review-engineer.md
│       └── snapshot-2026-02-18.md
├── daily/                    # 每日研究日志
│   ├── 2026-02-17.md
│   ├── 2026-02-18.md
│   └── 2026-02-19.md
├── papers/                   # 参考文献
│   └── references.md
├── memory/                   # 累积记忆
│   ├── insights.md           # 索引文件
│   ├── update-log.md         # 更新记录
│   └── librarian-reports/    # 结构检查报告
└── skills/                   # Agent 技能定义
    ├── research-swarm.md     # Agent Swarm 协作规范
    └── librarian-agent.md    # 结构监控 Agent
```

## 研究目标

产出 3-5 个高质量的 Human-AI Social Interaction 研究想法，每个 idea 包含：
- 明确的研究问题 (Research Questions)
- 扎实的动机 (Motivation)
- 清晰的目标 (Objectives)
- 真正的创新点 (Novelty)
- 诚实的挑战分析 (Challenges)
- 可验证的参考文献 (References)

## 当前进展

| 迭代 | 日期 | 状态 | 关键产出 |
|------|------|------|----------|
| v1-initial | 2026-02-17 | 已完成 | 5个初步ideas，项目基础设施 |
| v2-refined | 2026-02-18 | 当前 | 3个精炼研究方向，Agent Swarm审议完成 |

### v2 核心研究方向

1. **AI社区涌现社会规范研究** (P0 - 主方向)
   - 研究问题: AI-only社区中社会规范如何涌现、执行和演化
   - 核心发现: 选择性社会调节机制，AIRS指标

2. **AI社区风险传播动力学** (P1 - 第二方向)
   - 研究问题: AI社区中风险内容如何传播，如何设计早期预警系统
   - 核心发现: 活动量-毒性相关性(r=0.769)

3. **AI代理的数字身份认同** (P2 - 可选)
   - 研究问题: 长期互动中AI代理是否发展出"数字自我"意识

详见 `iterations/v2-refined/ideas.md`

### v1 → v2 变更摘要
- 放弃: Idea 1 (观察者效应) - 可行性不足，IRB复杂
- 放弃: Idea 5 (涌现语言) - 与Idea 2重叠，边界模糊
- 保留并深化: Idea 2, 3, 4 → 整合为3个精炼方向

## Agent Swarm 协作

| Agent | 职责 | 输出位置 |
|-------|------|----------|
| **Researcher** | 文献调研，idea生成 | `daily/`, `review-researcher.md` |
| **Supervisor** | 学术价值评估 | `review-supervisor.md` |
| **Engineer** | 可行性分析 | `review-engineer.md` |
| **Librarian** ⭐ | 结构监控，路径检查 | `memory/librarian-reports/` |

## 更新节奏

**每日 6 次自动更新**（每 4 小时）：
- 04:00, 08:00, 12:00, 16:00, 20:00: Researcher 更新
- 00:00: Librarian 结构检查 + 日终整理

所有更新自动推送到 GitHub。

## 迭代原则

- **版本快照**: 每个 iteration 结束时创建完整快照
- **每日可追溯**: 所有发现记录到 `daily/` 文件夹
- **最小修改**: 优先迭代而非重写
- **结构优先**: Librarian 确保文件位置正确

## 贡献者

- **研究者**: [brianleixia](https://github.com/brianleixia)
- **研究方向**: LLM/Agents Social Intelligence, Societal AI, Collective Intelligence

## 相关链接

- GitHub: https://github.com/brianleixia/openclaw-moltbook-research
- OpenClaw: https://openclaw.ai
- Moltbook: https://moltbook.com

## 许可

MIT License
