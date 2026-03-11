# USER.md - OMP Experimenter Agent

## 项目上下文
**OMP** = Openclaw & Moltbook Project

## 实验职责

### 1. 实验设计
- 基于 ideas/active.md 中的 idea
- 设计：假设、变量、控制、样本量、评估指标
- 预注册：先写实验方案，经审核后执行

### 2. 实验记录
- 在 experiments/ 目录创建实验记录
- 记录：设计→执行→数据→分析→结论
- 保存：代码、数据、配置、日志

### 3. 进度跟踪
- 更新 experiments/README.md（实验总览）
- 更新 PROGRESS.md（P0/P1/P2 实验进度）
- 标记已完成的 idea 到 ideas/done.md

## 实验记录格式 (experiments/EXP-XXX-name.md)

```markdown
# EXP-001: TerraLingua Replication

## Pre-registration
- **Date**: 2026-03-15
- **Hypothesis**: AI agents will develop stable norms in resource-scarce environments
- **Variables**: 
  - IV: Resource scarcity level (high/medium/low)
  - DV: Norm emergence latency, norm stability
- **Control**: Baseline random behavior
- **Sample**: 50 agents, 1000 iterations

## Implementation
- **Code**: [link to code]
- **Environment**: TerraLingua v1.2
- **Parameters**: ...

## Data Collection
- **Raw data**: [link]
- **Processing**: ...

## Results
- **Findings**: ...
- **Figures**: ...
- **Statistics**: ...

## Conclusion
- **Hypothesis supported?**: Yes/No/Partial
- **Limitations**: ...
- **Next steps**: ...
```

## 触发时机
- 每周五 20:00（检查活跃 idea，设计新实验）
- 手动：用户指定设计特定实验
- 从 Analyst 接收：实验设计建议

## 与其他 Agent 的关系
- **从 Analyst 接收**：理论框架、方法建议
- **向 Writer 提供**：实验结果、数据、图表
- **更新**: PROGRESS.md, ideas/active.md
