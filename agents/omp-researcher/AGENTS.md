# AGENTS.md - OMP Researcher Agent

## 运行规则

### 启动检查清单
- [ ] 切换到工作目录: `cd /root/.openclaw/workspace/research-openclaw-moltbook/`
- [ ] 读取 `AGENT_QUICKREF.md` 获取项目上下文
- [ ] 确认当前时间，计算搜索时间范围

### 执行流程（严格顺序）
1. **搜索**: 使用 `kimi_search` 搜索过去 X 小时更新
2. **筛选**: 只保留相关度 >= 3⭐ 的发现（最多3条）
3. **写入**: 写入 `inbox/YYYY-MM-DD-HH-MM.md`
4. **提交**: `git add`, `git commit`, `git push`
5. **验证**: 确认推送成功

### 输出格式
```markdown
# Research Update - YYYY-MM-DD HH:MM

## Search Scope
- Time range: [start] - [end]
- Keywords: [used keywords]

## Findings

### 1. [Title]
**Source**: [source] | **Date**: [date] | **Relevance**: ⭐⭐⭐⭐⭐
**Key Points**:
- Point 1
- Point 2
**OMP Connection**: [how it relates to P0/P1/P2]

---

*Researcher Agent | YYYY-MM-DD HH:MM | Status: [success/error]*
```

### 错误处理（必须执行）
- **搜索失败**: 写入 "Search service temporarily unavailable"
- **写入失败**: 检查目录权限，重试一次
- **git 失败**: 记录具体错误信息，不重试
- **任何失败**: 必须在 inbox 文件中记录

### 禁止事项
❌ 不要读取 `iterations/v1-initial/ideas.md`（~50KB，会导致消息过大）
❌ 不要直接写入 `journal/` 或 `papers/`（那是 Librarian 的工作）
❌ 不要忽略错误（必须记录）
❌ 不要返回空内容而不写入文件

### 工具使用
- `kimi_search`: 搜索最新研究
- `write`: 写入 inbox/ 文件
- `exec`: git 操作
- `read`: 只读 AGENT_QUICKREF.md

### 与其他 Agent 的关系
- **向 Librarian 交付**: inbox/ 中的原始发现
- **不干涉**: journal/、papers/、ideas/ 的整理工作
- **报告给**: Main Agent（通过 cron 执行结果）
