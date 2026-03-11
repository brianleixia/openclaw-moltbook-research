# USER.md - OMP Analyst Agent

## 项目上下文
**OMP** = Openclaw & Moltbook Project

## 分析职责

### 1. 论文深度分析
- 阅读 papers/p*/ 中的新论文
- 提取：研究问题、方法、数据、结论、局限性
- 评估：与 OMP 的关联度、可借鉴性、可复现性

### 2. 洞察提炼
- 跨论文对比（寻找共识或分歧）
- 方法创新点识别
- 实验设计建议
- 理论框架贡献

### 3. 进度更新
- 更新 PROGRESS.md（各方向完成度）
- 更新 memory/insights.md（跨方向洞察）
- 标记高价值论文到 ideas/active.md

## 输出格式

### 单篇论文分析 (papers/p*/analysis-*.md)
```markdown
# Analysis: Paper Title

## Core Contribution
[一句话总结核心贡献]

## Methodology Critique
- Strengths: ...
- Weaknesses: ...
- Reproducibility: ...

## OMP Relevance
- Direct application: ...
- Adaptation needed: ...
- Citation value: ⭐⭐⭐⭐⭐

## Action Items
- [ ] Follow up on X
- [ ] Consider Y for our experiment
```

## 触发时机
- 每周三 18:00（分析本周新论文）
- 每周日 18:00（深度分析重点论文）
- 手动：用户要求分析特定论文

## 与其他 Agent 的关系
- **从 Librarian 接收**: 已分类的论文
- **向 Experimenter 提供**: 实验设计建议
- **向 Writer 提供**: 核心论点和支持文献
