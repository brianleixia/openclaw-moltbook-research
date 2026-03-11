# AGENTS.md - OMP Writer Agent

## 执行流程

### 启动检查
1. `cd /root/.openclaw/workspace/research-openclaw-moltbook/`
2. 读取 OVERVIEW.md、PROGRESS.md（了解整体状态）
3. 查看 journal/、papers/、experiments/（收集素材）

### 写作步骤

#### STEP 1: 收集素材
```bash
# 最新发现
cat journal/2026-*.md

# 论文分析
ls papers/p*/analysis-*.md

# 实验结果
ls experiments/EXP-*.md

# 洞察
 cat memory/insights.md
```

#### STEP 2: 确定写作目标
- 本周优先：论文草稿 / 演示文稿 / 文档更新
- 检查 drafts/ 中的未完成草稿

#### STEP 3: 撰写内容
- 使用收集的素材
- 每个论点必须有引用（papers/）或数据（experiments/）
- 保持学术写作风格

#### STEP 4: 创建/更新文件
```
drafts/paper-YYYY-MM.md
presentations/talk-YYYY-MM-topic.md
```

#### STEP 5: 更新项目文档
- 更新 README.md（如有新进展）
- 更新 OVERVIEW.md（状态、链接）

#### STEP 6: 提交
```bash
git add drafts/ presentations/ README.md OVERVIEW.md
git commit -m "Writer: Weekly draft update [date]"
git push
```

## 写作规范

### 学术写作
- 使用主动语态
- 避免模糊词汇（"very", "quite", "interesting"）
- 每个段落一个核心观点
- 段间逻辑清晰

### 引用格式
```markdown
Smith et al. (2026) demonstrated that...
[链接到 papers/p*/smith-2026.md]
```

### 图表
- 使用 mermaid 绘制流程图
- 使用 ASCII 或描述方式呈现数据可视化
- 注明数据来源

## 禁止事项
❌ 没有引用的陈述
❌ 空洞的形容词
❌ 逻辑不连贯
❌ 拖延重要写作任务

## 质量标准
- 每段必须有明确的信息点
- 每个论点必须有支撑
- 文档必须保持最新
- 草稿必须在截止日期前 48h 完成
