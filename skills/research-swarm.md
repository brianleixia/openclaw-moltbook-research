# Research Swarm Skill

> 本项目专用的 Agent Swarm 协作规范

## 角色定义

### Researcher Agent
**职责**: 文献调研与 idea 生成

**任务清单**:
1. 搜索相关领域的最新论文
2. 识别研究空白 (research gaps)
3. 提出 3-5 个初步 research ideas
4. 为每个 idea 提供初步的 motivation 和 novelty

**输出格式**:
```markdown
## Idea N: [标题]
**核心洞察**: [一句话概括]
**Research Questions**: [2-3 个具体问题]
**Motivation**: [为什么重要]
**Novelty**: [与现有工作的区别]
**关键文献**: [3-5 篇核心论文]
```

---

### Supervisor Agent
**职责**: 批判性评估

**评估维度**:
1. **学术价值**: 是否解决重要问题？
2. **创新性**: novelty 是否足够？
3. **可行性**: 在博士阶段可完成吗？
4. **影响力**: 潜在引用价值？

**输出格式**:
```markdown
## Idea N 评估: [标题]
**评分**: X/10
**优点**: [列出]
**弱点**: [列出]
**建议**: [如何改进]
**风险**: [潜在问题]
```

---

### Engineer Agent
**职责**: 可行性分析

**评估维度**:
1. **数据获取**: 是否有可用数据？
2. **计算资源**: 需要多少 GPU/存储？
3. **技术依赖**: 依赖哪些工具/平台？
4. **时间估算**: 原型 vs 完整研究的时间

**输出格式**:
```markdown
## Idea N 可行性: [标题]
**数据**: [来源/获取难度]
**资源**: [计算需求]
**技术栈**: [关键工具]
**时间**: [预估]
**阻塞点**: [最大风险]
```

---

## 协作流程

```
Round N:
1. Researcher → 产出 ideas-vN-draft.md
2. Supervisor → 评估 → ideas-vN-reviewed.md
3. Engineer → 可行性 → ideas-vN-feasible.md
4. Orchestrator → 整合 → ideas-vN.md
```

## 迭代原则

- 保留有价值的部分
- 删除或修改被质疑的部分
- 添加新产生的洞察
- 保持文件结构一致

---

*Created: 2026-02-17*
