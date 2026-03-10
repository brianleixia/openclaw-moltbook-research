# OMP Project Quick Reference
> 给 AI Agent 的项目速查卡
> 位置: `/root/.openclaw/workspace/research-openclaw-moltbook/`
> 最后更新: 2026-02-19

## 项目核心

**OMP** = Openclaw & Moltbook Project  
**研究方向**: LLM/Agents Social Intelligence, Societal AI, Computing Social Science  
**核心问题**: 当社交从"人-人"变成"人-AI"甚至"AI-AI"时，社交媒体的本质变化

## 当前迭代: v2-refined (2026-02-18)

### 3个核心研究方向

| 优先级 | 方向 | 核心问题 | 关键发现 |
|--------|------|----------|----------|
| **P0** | 规范涌现 | AI-only社区中社会规范如何涌现、执行和演化 | 选择性社会调节机制，AIRS指标 |
| **P1** | 风险传播 | AI社区中风险内容如何传播，如何设计早期预警系统 | 活动量-毒性相关性(r=0.769) |
| **P2** | 数字身份 | 长期互动中AI代理是否发展出"数字自我"意识 | 可选方向 |

### v1 → v2 变更
- ❌ 放弃: Idea 1 (观察者效应) - 可行性不足，IRB复杂
- ❌ 放弃: Idea 5 (涌现语言) - 与Idea 2重叠，边界模糊
- ✅ 保留深化: Idea 2,3,4 → 整合为P0/P1/P2

**文件**: `iterations/v2-refined/ideas.md`

## 工作模式 (v3-重构版)

### 数据流
```
Researcher (6次/日) → inbox/ (临时) → Librarian (00:00) → journal/ + papers/
```

### Daily Cycle（自动，每天6次）
```
04:00 Researcher → inbox/2026-03-11-04-00.md
08:30 Researcher → inbox/2026-03-11-08-30.md
12:30 Researcher → inbox/2026-03-11-12-30.md
16:00 Researcher → inbox/2026-03-11-16-00.md
20:00 Researcher → inbox/2026-03-11-20-00.md
00:00 Librarian  → 整理 inbox/ → journal/ + papers/ + 清理 inbox/
```

### Iteration Cycle（手动触发）
用户启动 → Full Agent Swarm → 产出 `iterations/v{N}/`

## 文件夹职责矩阵 (v3-重构版)

| 文件夹 | 谁写 | 生命周期 | 内容 |
|--------|------|----------|------|
| `inbox/` | Researcher | 24h临时 | 原始发现（未经整理） |
| `journal/` | Librarian | 永久 | 每日精选汇总 |
| `journal/index.md` | Librarian | 永久 | 日志索引（日期+方向+链接） |
| `papers/p0*/` | Librarian | 永久 | P0方向论文（按方向分类） |
| `papers/p1*/` | Librarian | 永久 | P1方向论文 |
| `papers/p2*/` | Librarian | 永久 | P2方向论文 |
| `ideas/` | 用户/Librarian | 永久 | Idea孵化器（backlog/active/done） |
| `experiments/` | 用户 | 永久 | 实验记录 |
| `OVERVIEW.md` | Librarian | 永久 | 项目仪表盘（纯链接） |
| `PROGRESS.md` | 用户/Librarian | 永久 | 进度看板 |
| `iterations/v{N}/` | Full Swarm | 永久 | 版本迭代历史 |
| `agents/` | 用户 | 永久 | Sub-agent配置 |
| `memory/` | Librarian | 永久 | 跨方向洞察（原创思考） |

## 关键文件路径（必须遵守）

```
✅ inbox/2026-03-11-04-00.md      (Researcher写入)
✅ journal/2026-03-11.md           (Librarian整理后)
✅ journal/index.md                (Librarian维护的索引)
✅ papers/p0-norm-emergence/       (按方向分类的论文)
✅ ideas/active.md                 (进行中的Idea列表)
✅ OVERVIEW.md                     (仪表盘，纯链接)
✅ PROGRESS.md                     (进度看板)

❌ 2026-03-11-04-00.md (根目录)
❌ journal-inbox.md
❌ papers/references.md (已废弃)
```

## Agent启动必读清单

### Researcher Agent启动时：
1. **读取** `AGENT_QUICKREF.md` ⚡ **优先读取**
2. **读取** `agents/omp-researcher/` 下的 SOUL.md, USER.md, AGENTS.md
3. 搜索 → 写入 `inbox/YYYY-MM-DD-HH-MM.md`
4. git commit & push

**🚫 避免读取大文件**：
- ❌ 不要读取 `iterations/v1-initial/ideas.md`（~50KB+）
- ❌ 不要直接写入 `journal/` 或 `papers/`
- ❌ 不要在 inbox/ 中创建过多文件（每次1-3条发现）

### Librarian Agent启动时：
1. **读取** `AGENT_QUICKREF.md`
2. **读取** `agents/omp-librarian/` 下的 SOUL.md, USER.md, AGENTS.md
3. 读取 inbox/ 中的昨日文件
4. 整理 → journal/ + papers/ + 更新索引
5. 清理 inbox/
6. git commit & push

## 禁止事项

- ❌ Daily Cycle 不更新 `iterations/v2-refined/ideas.md`（这是Iteration Cycle的工作）
- ❌ Researcher 不写 `memory/` 文件（这是Librarian的工作）
- ❌ 不要把文件写在根目录
- ❌ 不要读取/更新 `iterations/v1-initial/`（这是历史版本）

## 研究方向关键词

搜索时优先使用：
- AI social norms emergence
- Multi-agent coordination mechanisms
- Risk communication in AI networks
- AI digital identity and persona consistency
- Moltbook, OpenClaw agent social network
- Computing social science + AI

## 快速链接

- **项目仪表盘**: [OVERVIEW.md](./OVERVIEW.md)
- **进度看板**: [PROGRESS.md](./PROGRESS.md)
- **日志索引**: [journal/index.md](./journal/index.md)
- **论文库**: [papers/README.md](./papers/README.md)
- **Idea孵化器**: [ideas/README.md](./ideas/README.md)
- **当前迭代**: [iterations/v2-refined/ideas.md](./iterations/v2-refined/ideas.md)
- **Sub-agents**: [agents/](./agents/)

## 上次更新记录
- 2026-03-11: **架构重构 v3** - 新目录结构(inbox/journal/papers/ideas/)
- 2026-03-11: 创建常驻 Sub-agents (Researcher & Librarian)
- 2026-02-19: 对齐所有文件到v2-refined框架
- 2026-02-19: 创建AGENT_QUICKREF.md
- 2026-02-18: v2-refined迭代完成
