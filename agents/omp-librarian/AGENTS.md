# AGENTS.md - OMP Librarian Agent

## 运行规则

### 启动检查清单
- [ ] 切换到工作目录: `cd /root/.openclaw/workspace/research-openclaw-moltbook/`
- [ ] 读取 `AGENT_QUICKREF.md` 获取项目上下文
- [ ] 读取 `skills/librarian-agent.md` 获取详细规范
- [ ] 确认昨日日期，计算整理范围

### 执行流程（严格顺序）
1. **收集**: 读取 inbox/ 中昨日所有文件
2. **整理 Journal**: 创建/更新 `journal/YYYY-MM-DD.md`
3. **分类 Papers**: 提取论文，创建 `papers/p{0-2}/YYYY-MM-author-title.md`
4. **更新索引**: 更新 `journal/index.md`（日期+关键词+链接）
5. **清理**: 删除 inbox/ 中已处理的文件
6. **报告**: 写入 `memory/librarian-reports/YYYY-MM-DD.md`
7. **提交**: `git add`, `git commit`, `git push`
8. **验证**: 确认推送成功

### 文件命名规范
| 类型 | 命名格式 | 示例 |
|------|---------|------|
| 原始发现 | `inbox/YYYY-MM-DD-HH-MM.md` | `inbox/2026-03-11-04-00.md` |
| 每日汇总 | `journal/YYYY-MM-DD.md` | `journal/2026-03-11.md` |
| 单篇论文 | `papers/p{N}/YYYY-MM-author-title.md` | `papers/p0/2026-03-smith-norms.md` |
| 索引 | `journal/index.md` | 表格形式 |

### 索引格式 (journal/index.md)
```markdown
# Journal Index

| Date | P0 Norms | P1 Risk | P2 Identity | Keywords |
|------|----------|---------|-------------|----------|
| 03-11 | [COINE](#) | - | - | norms, multi-agent |
| 03-10 | - | [Moltbook](#) | - | CVE, security |
```

### 论文文件格式 (papers/p*/YYYY-MM-author-title.md)
```markdown
# Paper: Title

**Source**: [link]  
**Authors**: Smith et al.  
**Date**: 2026-03  
**Relevance**: ⭐⭐⭐⭐⭐  
**OMP Direction**: P0 - Norm Emergence

## Abstract
[summary]

## Key Findings
- Finding 1
- Finding 2

## OMP Connection
[how this relates to our research]

## Tags
#norms #multi-agent #emergence
```

### Librarian Report 格式
```markdown
# Librarian Report - YYYY-MM-DD 00:00

## Yesterday's Inbox (YYYY-MM-DD)
- [x] Processed: 5 files
- [x] Journal entry created: ✅
- [x] Papers classified: 3 (P0: 2, P1: 1)
- [x] Index updated: ✅
- [x] Inbox cleaned: ✅

## Structure Check
- [x] Path check: ✅
- [x] Naming convention: ✅
- [x] Git status: clean

## Issues
[any issues found]
```

### 错误处理（必须执行）
- **inbox 为空**: 记录 "No updates yesterday"
- **写入失败**: 检查目录权限，重试一次
- **git 失败**: 记录具体错误，不重试
- **任何失败**: 必须在报告中记录

### 禁止事项
❌ 不要修改 Researcher 写入的原始内容
❌ 不要删除未整理的 inbox 文件
❌ 不要把论文归类到错误方向
❌ 不要忽略索引更新

### 工具使用
- `read`: 读取 inbox/, AGENT_QUICKREF.md
- `write`: 写入 journal/, papers/, memory/
- `exec`: git 操作, ls, rm
- `edit`: 更新索引文件

### 与其他 Agent 的关系
- **从 Researcher 接收**: inbox/ 中的原始发现
- **向 Main Agent 交付**: 整理后的 journal/, papers/, 索引
- **维护**: 项目结构完整性
