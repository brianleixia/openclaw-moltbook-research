# OMP Agent Swarm 架构

**版本**: v3.1 | **最后更新**: 2026-03-11

## 🏗️ Agent 组织架构

```
┌─────────────────────────────────────────────────────────────┐
│                      Main Agent (You)                        │
│                   监督、决策、最终审核                        │
└─────────────────────────────────────────────────────────────┘
                              │
        ┌─────────────────────┼─────────────────────┐
        │                     │                     │
        ▼                     ▼                     ▼
┌──────────────┐    ┌──────────────┐    ┌──────────────┐
│  Researcher  │    │   Analyst    │    │ Experimenter │
│   (Daily)    │    │  (Weekly)    │    │   (Weekly)   │
└──────────────┘    └──────────────┘    └──────────────┘
        │                     │                     │
        └─────────────────────┼─────────────────────┘
                              │
                              ▼
                    ┌─────────────────┐
                    │  Librarian      │
                    │  (Daily 00:00)  │
                    └─────────────────┘
                              │
                              ▼
                    ┌─────────────────┐
                    │     Writer      │
                    │   (Weekly)      │
                    └─────────────────┘
```

## 👥 Agent 职责矩阵

| Agent | 核心职责 | 输出 | 频率 | 权限 |
|-------|---------|------|------|------|
| **Researcher** | 发现最新研究 | inbox/*.md | 每日6次 | 只写 inbox/ |
| **Librarian** | 整理、分类、索引 | journal/, papers/ | 每日00:00 | 读 inbox/, 写 journal/papers |
| **Analyst** | 深度分析论文 | analysis-*.md, insights/ | 每周2次 | 读 papers/, 写 analysis/ |
| **Experimenter** | 设计、执行实验 | experiments/EXP-*.md | 每周1次+按需 | 写 experiments/, 更新 PROGRESS |
| **Writer** | 撰写论文、文档 | drafts/, presentations/ | 每周1次 | 读全库, 写 drafts/ |

## 🔄 数据流

```
Day 1-6 (Research Phase):
    Researcher ──► inbox/ ──► Librarian ──► journal/ + papers/
                                    │
                                    ▼
    Day 7 (Analysis Phase):
    Analyst ◄──── papers/ ────► analysis/ ────► insights/
                                    │
                                    ▼
    (Execution Phase):
    Experimenter ◄── ideas/ ────► experiments/ ────► results
                                    │
                                    ▼
    (Writing Phase):
    Writer ◄──── journal/ + papers/ + experiments/ ────► drafts/
```

## 📅 执行时间表

| 时间 | Agent | 任务 | 输出检查 |
|------|-------|------|---------|
| 04:00 | Researcher | 搜索更新 | inbox/ 新文件 |
| 08:30 | Researcher | 搜索更新 | inbox/ 新文件 |
| 12:30 | Researcher | 搜索更新 | inbox/ 新文件 |
| 16:00 | Researcher | 搜索更新 | inbox/ 新文件 |
| 20:00 | Researcher | 搜索更新 | inbox/ 新文件 |
| 00:00 | Librarian | 整理 inbox/ | journal/ + papers/ 更新 |
| 周三 18:00 | Analyst | 分析新论文 | analysis-*.md |
| 周五 20:00 | Experimenter | 设计实验 | EXP-*.md (预注册) |
| 周日 18:00 | Analyst | 深度分析 | insights/ 更新 |
| 周日 21:00 | Writer | 撰写草稿 | drafts/ 更新 |

## 🔒 权限控制

### 写入权限矩阵

| Agent | inbox/ | journal/ | papers/ | analysis/ | experiments/ | drafts/ | ideas/ |
|-------|--------|----------|---------|-----------|--------------|---------|--------|
| Researcher | ✅ 写 | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| Librarian | ✅ 读/删 | ✅ 写 | ✅ 写 | ❌ | ❌ | ❌ | ❌ |
| Analyst | ❌ | ❌ | ✅ 读 | ✅ 写 | ❌ | ❌ | ❌ |
| Experimenter | ❌ | ❌ | ❌ | ❌ | ✅ 写 | ❌ | ✅ 更新 |
| Writer | ❌ | ❌ | ✅ 读 | ✅ 读 | ✅ 读 | ✅ 写 | ❌ |

## 🚨 冲突解决

### 1. 文件位置冲突
- **规则**: 各 Agent 只在自己的目录写入
- **Librarian 负责**: 协调文件命名，避免覆盖

### 2. 内容更新冲突
- **规则**: 使用 git 管理版本
- **Librarian 负责**: 每日 00:00 统一提交

### 3. 任务优先级冲突
- **Main Agent 决策**: 用户（你）指定优先级
- **默认顺序**: Researcher > Librarian > Analyst > Experimenter > Writer

## 📊 质量保证

### 每个 Agent 的产出标准

| Agent | 质量标准 |
|-------|---------|
| Researcher | 相关度≥3⭐, 来源可靠, 及时提交 |
| Librarian | 结构正确, 索引更新, 及时清理 |
| Analyst | 批判性分析, 原创洞察, 可操作建议 |
| Experimenter | 可复现, 完整记录, 及时更新 |
| Writer | 清晰, 有证据支撑, 按时完成 |

## 🆘 故障处理

### Agent 未按时执行
1. 检查 cron 状态
2. 检查 Agent session 状态
3. 手动触发: `sessions_send(sessionKey, "执行任务")`

### Agent 输出质量差
1. 检查 Agent 是否读取了正确的上下文文件
2. 更新 Agent 的 SOUL.md/USER.md 澄清期望
3. 手动提供反馈，帮助学习

### Git 提交冲突
1. Librarian 优先处理冲突
2. 如有复杂冲突，通知 Main Agent
3. 避免多个 Agent 同时提交

## 📈 扩展计划

### 未来可能添加的 Agent
- **Reviewer**: 审核论文草稿，提供修改意见
- **Coder**: 专门负责实验代码实现
- **Visualizer**: 生成数据可视化
- **Outreach**: 管理社交媒体、博客、会议投稿

---

*由 Main Agent 维护 | OMP Project v3.1*
