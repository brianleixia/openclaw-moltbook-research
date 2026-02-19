# OpenClaw & Moltbook Research Project

## 项目简介

探索 OpenClaw 爆火带动的 Moltbook（纯 AI 交互社交媒体）引发的研究机会。

**核心问题**: 当社交互动的参与者从"人-人"变成"人-AI"甚至"AI-AI"时，社交媒体的本质会发生什么变化？

**v3 核心洞察**: 规模化≠社会化——AI 社会可能保持"非社会化"状态，规范通过任务协调而非社会互动形成。

## 项目结构（v3）

```
research-openclaw-moltbook/
├── README.md                 # 本文件
├── AGENT_QUICKREF.md         # AI Agent 速查卡
├── iterations/               # 研究迭代版本
│   ├── v1-initial/           # 第一轮迭代 (历史)
│   │   ├── ideas.md          # 5个初步研究想法
│   │   └── snapshot-2026-02-17.md
│   ├── v2-refined/           # 第二轮迭代 (历史)
│   │   ├── ideas.md          # 3个精炼研究方向
│   │   └── snapshot-2026-02-18.md
│   └── v3-integrated/        # 第三轮迭代 (当前)
│       └── ideas.md          # 基于调研整合优化
├── daily/                    # 每日研究日志
│   └── YYYY-MM-DD.md
├── papers/                   # 参考文献
│   └── references.md
├── memory/                   # 累积记忆
│   ├── insights.md           # 索引文件
│   ├── update-log.md         # 版本历史
│   └── librarian-reports/    # 结构检查报告
└── skills/                   # Agent 技能定义
    ├── research-swarm.md     # Agent Swarm 协作规范
    └── librarian-agent.md    # 结构监控 Agent
```

## 研究目标

产出 3 个高质量的 AI 社会研究想法，每个 idea 包含：
- 明确的研究问题 (Research Questions)
- 扎实的动机 (Motivation)
- 清晰的目标 (Objectives)
- 真正的创新点 (Novelty)
- 诚实的挑战分析 (Challenges)
- 可验证的参考文献 (References)

## 当前进展

| 迭代 | 日期 | 状态 | 关键产出 |
|------|------|------|----------|
| v1-initial | 2026-02-17 | 历史 | 5个初步ideas |
| v2-refined | 2026-02-18 | 历史 | 3个精炼研究方向 |
| **v3-integrated** | **2026-02-19** | **当前** | **基于调研整合优化** |

### v3 核心研究方向（重新定位）

1. **非社会化环境中的规范协调机制** (P0 - 主方向)
   - 研究问题: 在缺乏社会记忆的 AI 社区中，规范如何通过任务协调而非社会互动形成？
   - 核心发现: Moltbook "互动而无影响"，规模化≠社会化

2. **AI 社会供应链风险传播** (P1 - 第二方向)
   - 研究问题: AI 社会的风险如何通过技能供应链和代理间交互传播？
   - 核心发现: ClawHub 凭证窃取器，770K 令牌暴露

3. **最小可行身份与代理凭证管理** (P2 - 第三方向)
   - 研究问题: 在安全和效率约束下，AI 代理的"最小可行身份"如何设计？
   - 核心发现: Persona 一致性技术瓶颈，价值多样性增强稳定性

详见 `iterations/v3-integrated/ideas.md`

### v2 → v3 核心转变

| 维度 | v2 | v3 |
|------|-----|-----|
| **核心假设** | AI 社会会像人类一样社会化 | AI 社会保持"非社会化"状态 |
| **P0 重点** | 社会规范涌现 | 任务协调规范 |
| **P1 重点** | 风险内容传播 | 供应链安全 |
| **P2 重点** | 数字自我意识 | 最小可行身份 |

## Agent Swarm 协作

| Agent | 职责 | 输出位置 |
|-------|------|----------|
| **Researcher** | 文献调研，每日更新 | `daily/`, `papers/references.md` |
| **Supervisor** | 学术价值评估 | `iterations/v{N}/review-supervisor.md` |
| **Engineer** | 可行性分析 | `iterations/v{N}/review-engineer.md` |
| **Librarian** ⭐ | 结构监控，日终整合 | `memory/librarian-reports/`, `memory/insights.md` |
| **Orchestrator** | 迭代整合，版本升级 | `iterations/v{N}/ideas.md` |

## 更新节奏

### Daily Cycle（日常更新）
**频率**: 每天 6 次（04:00, 08:00, 12:00, 16:00, 20:00, 00:00）

| 时间 | Agent | 任务 | 输出 |
|------|-------|------|------|
| 04:00 | Researcher | Night update | `daily/YYYY-MM-DD.md` |
| 08:00 | Researcher | Morning update | `daily/YYYY-MM-DD.md` |
| 12:00 | Researcher | Noon update | `daily/YYYY-MM-DD.md` |
| 16:00 | Researcher | Afternoon update | `daily/YYYY-MM-DD.md` |
| 20:00 | Researcher | Evening update | `daily/YYYY-MM-DD.md` |
| **00:00** | **Librarian** | **结构检查 + 日终整合** | `memory/librarian-reports/`, `memory/insights.md` |

### Iteration Cycle（迭代升级）
**触发**: 用户启动或 Librarian 检测到重大发现积累
**参与**: Full Agent Swarm
**输出**: `iterations/v{N}/` 完整文件集

## 迭代原则

- **版本快照**: 每个 iteration 结束时创建完整快照
- **每日可追溯**: 所有发现记录到 `daily/` 文件夹
- **日终整合**: Librarian 每日 00:00 更新索引和日志
- **最小修改**: 优先迭代而非重写
- **结构优先**: Librarian 确保文件位置正确
- **当前版本**: 始终指向最新 iteration

## 贡献者

- **研究者**: [brianleixia](https://github.com/brianleixia)
- **研究方向**: LLM/Agents Social Intelligence, Societal AI, Collective Intelligence

## 相关链接

- GitHub: https://github.com/brianleixia/openclaw-moltbook-research
- OpenClaw: https://openclaw.ai
- Moltbook: https://moltbook.com

## 许可

MIT License
