# Research Swarm Skill

> 本项目专用的 Agent Swarm 协作规范

## 项目结构（v2）

```
research-openclaw-moltbook/
├── README.md
├── iterations/           # 按版本组织的完整研究迭代
│   └── v1-initial/
│       ├── ideas.md              # 该版本的完整想法
│       ├── review-researcher.md  # Researcher 输出
│       ├── review-supervisor.md  # Supervisor 评估
│       ├── review-engineer.md    # Engineer 分析
│       └── snapshot-YYYY-MM-DD.md # 版本快照
├── daily/                # 每日研究日志
│   ├── 2026-02-17.md
│   └── 2026-02-18.md
├── papers/               # 参考文献
│   └── references.md
├── memory/               # 累积记忆
│   ├── insights.md       # 索引文件（链接到每日日志）
│   └── update-log.md     # 更新记录
└── skills/               # Agent 技能定义
    ├── research-swarm.md
    └── librarian-agent.md
```

## 文件路径规范

**工作目录**: `/root/.openclaw/workspace/research-openclaw-moltbook`

### 文件类型映射
| 内容类型 | 正确路径 | 错误路径 |
|----------|----------|----------|
| 研究想法（当前版本） | `iterations/v{N}/ideas.md` | `ideas/ideas-v{N}.md` ❌ |
| 每日发现 | `daily/YYYY-MM-DD.md` | `memory/daily-YYYY-MM-DD.md` ❌ |
| 参考文献 | `papers/references.md` | `papers/paper-notes.md` ❌ |
| 灵感索引 | `memory/insights.md` | `memory-insights.md` ❌ |

### 路径检查清单
每次写入文件前，必须确认：
1. ✅ 是否使用了正确的子目录？
2. ✅ 文件名是否符合 `YYYY-MM-DD.md` 或 `ideas.md` 规范？
3. ✅ 是否意外创建在根目录？

## Agent 角色定义

### Researcher Agent
**职责**: 文献调研与 idea 生成

**输出位置**:
- 新版本: `iterations/v{N}/review-researcher.md`
- 每日更新: `daily/YYYY-MM-DD.md`

---

### Supervisor Agent
**职责**: 批判性评估

**输出位置**: `iterations/v{N}/review-supervisor.md`

---

### Engineer Agent
**职责**: 可行性分析

**输出位置**: `iterations/v{N}/review-engineer.md`

---

### Librarian Agent ⭐ 新增
**职责**: 项目结构监控

**任务**:
1. 检查文件是否写入正确位置
2. 监控命名规范
3. 每日 00:00 巡检并报告
4. 自动修复简单的路径错误

**输出位置**: `memory/librarian-reports/YYYY-MM-DD.md`

## 协作流程（更新）

```
Daily Cycle:
1. Researcher → 搜索更新 → 写入 daily/YYYY-MM-DD.md
2. Librarian → 检查结构 → 修复问题（如有）
3. Git → commit & push

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

| 时间 | Agent | 任务 |
|------|-------|------|
| 04:00 | Researcher | Night update |
| 08:00 | Researcher | Morning update |
| 12:00 | Researcher | Noon update |
| 16:00 | Researcher | Afternoon update |
| 20:00 | Researcher | Evening update |
| 00:00 | Librarian | Structure check + 日终整理 |

## 迭代原则

- **最小修改**: 优先修改而非重写
- **版本快照**: 每个 iteration 结束时创建 snapshot
- **每日可追溯**: 所有发现记录到 daily 文件夹
- **结构优先**: Librarian 确保文件位置正确

---

*Updated: 2026-02-18 (v2 structure)*
