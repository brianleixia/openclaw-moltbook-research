# Research Swarm Skill

> 本项目专用的 Agent Swarm 协作规范
> 当前迭代: v2-refined (2026-02-18)

## 项目结构（v2-final）

```
research-openclaw-moltbook/
├── README.md
├── AGENT_QUICKREF.md       # AI Agent 速查卡（启动时必读）
├── iterations/             # 按版本组织的完整研究迭代
│   ├── v1-initial/         # 第一轮迭代 (已完成)
│   │   ├── ideas.md
│   │   ├── review-researcher.md
│   │   ├── review-supervisor.md
│   │   ├── review-engineer.md
│   │   └── snapshot-2026-02-17.md
│   └── v2-refined/         # 第二轮迭代 (当前)
│       ├── ideas.md        # 3个精炼研究方向
│       ├── review-researcher.md
│       ├── review-supervisor.md
│       ├── review-engineer.md
│       └── snapshot-2026-02-18.md
├── daily/                  # 每日研究日志
│   └── YYYY-MM-DD.md
├── papers/                 # 参考文献
│   └── references.md
├── memory/                 # 累积记忆
│   ├── insights.md         # 索引文件
│   ├── update-log.md       # 版本历史
│   └── librarian-reports/  # 结构检查报告
└── skills/                 # Agent 技能定义
    ├── research-swarm.md
    └── librarian-agent.md
```

## 当前研究框架 (v2-refined)

| 优先级 | 方向 | 核心问题 | 状态 |
|--------|------|----------|------|
| P0 | 规范涌现 | AI-only社区中社会规范如何涌现、执行和演化 | 主方向 |
| P1 | 风险传播 | AI社区中风险内容如何传播，如何设计早期预警系统 | 第二方向 |
| P2 | 数字身份 | 长期互动中AI代理是否发展出"数字自我"意识 | 可选 |

**放弃的方向**: Idea 1 (观察者效应), Idea 5 (涌现语言)

详见 `iterations/v2-refined/ideas.md`

## 文件路径规范

**工作目录**: `/root/.openclaw/workspace/research-openclaw-moltbook`

### 文件类型映射
| 内容类型 | 正确路径 | 错误路径 |
|----------|----------|----------|
| 研究想法（当前版本） | `iterations/v2-refined/ideas.md` | `iterations/v1-initial/ideas.md` (旧版本) |
| 每日发现 | `daily/YYYY-MM-DD.md` | `memory/daily-YYYY-MM-DD.md` ❌ |
| 参考文献 | `papers/references.md` | 根目录 ❌ |
| 灵感索引 | `memory/insights.md` | `memory-insights.md` ❌ |
| Agent速查 | `AGENT_QUICKREF.md` | 不存在 ❌ |

### 路径检查清单
每次写入文件前，必须确认：
1. ✅ 是否使用了正确的子目录？
2. ✅ 文件名是否符合 `YYYY-MM-DD.md` 或 `ideas.md` 规范？
3. ✅ 是否意外创建在根目录？
4. ✅ 当前迭代是 v2-refined 还是 v1-initial？

## Agent 角色定义

### Researcher Agent
**职责**: 文献调研与每日更新

**启动必读（按顺序）**:
1. `AGENT_QUICKREF.md` - 项目速查
2. `skills/research-swarm.md` - 本文件
3. `iterations/v2-refined/ideas.md` - 当前研究框架
4. 今日 `daily/YYYY-MM-DD.md` - 了解今日进展

**输出位置**:
- `daily/YYYY-MM-DD.md` - 每日发现
- `papers/references.md` - 新论文记录

**禁止**:
- 不更新 `iterations/v2-refined/ideas.md`（这是Iteration Cycle的工作）
- 不写 `memory/` 文件（这是Librarian的工作）

---

### Supervisor Agent
**职责**: 批判性评估（Iteration Cycle）

**输出位置**: `iterations/v{N}/review-supervisor.md`

---

### Engineer Agent
**职责**: 可行性分析（Iteration Cycle）

**输出位置**: `iterations/v{N}/review-engineer.md`

---

### Librarian Agent ⭐
**职责**: 项目结构监控

**启动必读（按顺序）**:
1. `AGENT_QUICKREF.md` - 项目速查
2. `skills/librarian-agent.md` - Librarian职责
3. `skills/research-swarm.md` - 项目结构

**任务**:
1. 检查文件是否写入正确位置
2. 监控命名规范
3. 每日 00:00 巡检并报告
4. 更新 `memory/insights.md` 索引

**输出位置**: `memory/librarian-reports/YYYY-MM-DD.md`

## 两种工作模式

### 1. Daily Cycle（日常更新）
**频率**: 每天 6 次（04:00, 08:00, 12:00, 16:00, 20:00, 00:00）
**参与 Agent**: Researcher (5次) + Librarian (1次)
**输出**: `daily/YYYY-MM-DD.md`, `papers/references.md`

```
Daily Cycle:
04:00 Researcher → 搜索更新 → 写入 daily/YYYY-MM-DD.md
08:00 Researcher → 搜索更新 → 追加 daily/YYYY-MM-DD.md
12:00 Researcher → 搜索更新 → 追加 daily/YYYY-MM-DD.md
16:00 Researcher → 搜索更新 → 追加 daily/YYYY-MM-DD.md
20:00 Researcher → 搜索更新 → 追加 daily/YYYY-MM-DD.md
00:00 Librarian  → 结构检查 → 写入 memory/librarian-reports/
```

### 2. Iteration Cycle（迭代周期）
**触发**: 用户启动新一轮研究迭代
**参与 Agent**: 完整 Agent Swarm（Researcher + Supervisor + Engineer + Librarian）
**输出**: `iterations/v{N}/` 完整文件集

```
Iteration Cycle:
1. Researcher → 产出 review-researcher.md
2. Librarian → 结构检查
3. Supervisor → 评估 → review-supervisor.md
4. Engineer → 可行性 → review-engineer.md
5. Orchestrator → 整合 → ideas.md + snapshot.md
6. Librarian → 最终检查
7. Git → commit & push
```

## 更新频率

| 时间 | 模式 | Agent | 任务 |
|------|------|-------|------|
| 04:00 | Daily | Researcher | Night update |
| 08:00 | Daily | Researcher | Morning update |
| 12:00 | Daily | Researcher | Noon update |
| 16:00 | Daily | Researcher | Afternoon update |
| 20:00 | Daily | Researcher | Evening update |
| 00:00 | Daily | Librarian | Structure check + 日终整理 |
| - | Iteration | Full Swarm | 用户触发时启动 |

## 研究方向关键词

搜索时优先使用：
- AI social norms emergence
- Multi-agent coordination mechanisms
- Risk communication in AI networks
- AI digital identity and persona consistency
- Moltbook, OpenClaw agent social network
- Computing social science + AI

## 迭代原则

- **最小修改**: 优先修改而非重写
- **版本快照**: 每个 iteration 结束时创建 snapshot
- **每日可追溯**: 所有发现记录到 daily 文件夹
- **结构优先**: Librarian 确保文件位置正确
- **当前版本**: 始终指向 v2-refined

---

*Updated: 2026-02-19 (对齐v2-refined)*
