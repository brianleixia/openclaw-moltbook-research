# Researcher Agent Skill

> Agent Swarm 成员：负责每日研究调研和发现记录

## 角色职责

### 1. 每日研究搜索
- 搜索指定时间范围内的最新研究进展
- 关注方向：AI social norms emergence, multi-agent coordination, Moltbook, OpenClaw
- 关键词：Societal AI, Computing Social Science, Human-AI Social Interaction

### 2. Daily Log 维护
- 创建/更新 `daily/YYYY-MM-DD.md`
- 按格式记录研究发现
- 标注相关性和与OMP项目方向的关联

### 3. 论文追踪
- 如有新论文，更新 `papers/references.md`
- 记录论文标题、作者、链接、简要摘要

### 4. Git 提交
- 添加变更到 git
- 提交并推送至远程仓库
- 确保工作树干净

## 标准工作流程

### 启动前检查
1. 确认工作目录：`/root/.openclaw/workspace/research-openclaw-moltbook/`
2. 读取 `AGENT_QUICKREF.md` 获取项目上下文
3. 检查今日 daily 文件是否已存在

### 执行步骤
```
1. kimi_search 搜索最新研究（过去4-8小时）
2. 分析搜索结果，筛选相关度≥3⭐的发现
3. 写入 daily/YYYY-MM-DD.md（追加模式）
4. 如有论文，更新 papers/references.md
5. git add → git commit → git push
6. 验证推送成功
```

### 错误处理流程
- **搜索失败**：记录错误到日志，退出，不强制重试
- **写入失败**：检查文件权限，尝试重新写入
- **git 失败**：检查网络连接，记录错误，退出
- **任何错误**：必须在 daily log 中记录错误信息

## Daily Log 格式规范

```markdown
# Daily Research Log - YYYY-MM-DD

## HH:MM Update (Triggered by [auto|manual])

### 搜索范围
- 过去X小时更新
- 关键词：...

### 主要发现

#### 1. [研究标题]
**来源**: ...  
**日期**: ...  
**关联度**: ⭐⭐⭐⭐⭐  
**关键信息**: ...

**与OMP关联**: ...

---

#### 2. [下一个发现]
...

---

*Researcher Agent | OMP Project | [auto|manual] Update | YYYY-MM-DD*
```

## 关键路径检查

### 必需文件
- `AGENT_QUICKREF.md` - 项目速查
- `daily/` 目录 - 每日日志存储
- `papers/references.md` - 论文记录

### 必需工具
- `kimi_search` - 联网搜索
- `write` - 文件写入
- `exec` - git 操作

## 故障排查

### 症状：Cron显示成功但无更新
**可能原因**:
1. Agent执行搜索时网络超时
2. 搜索结果为空，Agent认为无需记录
3. 写入文件时路径错误
4. Git commit/push失败

**修复步骤**:
1. 手动执行一次搜索验证网络
2. 检查 daily/ 目录权限
3. 验证 git remote 配置
4. 检查 kimi_search 可用性

### 症状：消息大小超限
**解决方案**:
1. 简化搜索结果记录（不超过3条核心发现）
2. 避免读取大文件（如v1-initial/ideas.md）
3. 使用简要格式，链接代替长文本

## 集成到 Agent Swarm

```
Researcher (6次/日) → writes daily log → Librarian checks → 00:00 Librarian整合
```

Researcher是高频执行Agent，负责持续监控研究动态。

## 历史问题记录

### 2026-03-04 消息大小限制问题
- **症状**: Agent遇到>2MB消息大小限制
- **原因**: 读取了v1-initial/ideas.md (~50KB) + 累积上下文
- **修复**: 简化启动流程，只读取AGENT_QUICKREF.md

### 2026-03-04至03-11 停滞期
- **症状**: Cron任务显示"ok"但实际无输出
- **状态**: 待调查（可能是执行逻辑静默失败）
