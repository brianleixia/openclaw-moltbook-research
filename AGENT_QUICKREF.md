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

## 工作模式

### Daily Cycle（自动，每天6次）
```
04:00 Researcher → daily/YYYY-MM-DD.md
08:00 Researcher → daily/YYYY-MM-DD.md
12:00 Researcher → daily/YYYY-MM-DD.md
16:00 Researcher → daily/YYYY-MM-DD.md
20:00 Researcher → daily/YYYY-MM-DD.md
00:00 Librarian  → memory/librarian-reports/YYYY-MM-DD.md
```

### Iteration Cycle（手动触发）
用户启动 → Full Agent Swarm → 产出 `iterations/v{N}/`

## 文件夹职责矩阵

| 文件夹 | 谁写 | 内容 |
|--------|------|------|
| `daily/` | Researcher | 每日调研发现 |
| `papers/references.md` | Researcher | 论文记录 |
| `memory/insights.md` | Librarian | 索引（链接到daily） |
| `memory/librarian-reports/` | Librarian | 结构检查报告 |
| `memory/update-log.md` | 用户 | 版本历史 |
| `iterations/v2-refined/` | Full Swarm | 当前研究框架 |
| `iterations/v1-initial/` | Full Swarm | 历史版本 |
| `skills/` | 用户 | Agent技能定义 |

## 关键文件路径（必须遵守）

```
✅ daily/2026-02-19.md
❌ 2026-02-19-daily.md
❌ memory/daily-2026-02-19.md

✅ iterations/v2-refined/ideas.md  (当前版本)
❌ iterations/v1-initial/ideas.md  (旧版本，不更新)

✅ memory/insights.md
❌ memory-insights.md

✅ AGENT_QUICKREF.md
❌ 不存在
```

## Agent启动必读清单

### Researcher Agent启动时：
1. **读取** `AGENT_QUICKREF.md`（本文件）
2. **读取** `skills/research-swarm.md`
3. **读取** `iterations/v2-refined/ideas.md`（注意是v2不是v1）
4. **读取** 今日 `daily/YYYY-MM-DD.md`
5. 搜索 → 写入 `daily/YYYY-MM-DD.md`
6. 如有新论文，追加到 `papers/references.md`

### Librarian Agent启动时：
1. **读取** `AGENT_QUICKREF.md`
2. **读取** `skills/librarian-agent.md`
3. **读取** `skills/research-swarm.md`
4. 检查今日daily是否完整
5. 检查是否有文件在错误位置
6. 更新 `memory/insights.md` 索引
7. 写入 `memory/librarian-reports/YYYY-MM-DD.md`

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

- **当前迭代**: `iterations/v2-refined/ideas.md`
- **历史版本**: `iterations/v1-initial/ideas.md`
- **今日日志**: `daily/YYYY-MM-DD.md`
- **论文记录**: `papers/references.md`
- **项目结构**: `skills/research-swarm.md`

## 上次更新记录
- 2026-02-19: 对齐所有文件到v2-refined框架
- 2026-02-19: 创建AGENT_QUICKREF.md
- 2026-02-18: v2-refined迭代完成
- 2026-02-17: v1-initial项目初始化
