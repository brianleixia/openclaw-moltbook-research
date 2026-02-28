# OPM (OpenClaw & Moltbook Project) Research Ideas

> **版本**: v3.1-Updated  
> **日期**: 2026-03-01  
> **状态**: 基于最新文献调研更新

---

## 核心洞察

### v3.1 关键发现

过去两周的文献追踪揭示了AI社会研究的三个深层矛盾：

1. **能力-合作悖论**: 推理能力增强反而损害合作（Piedrahita et al., 2026; Willis et al., 2026）
2. **环境-涌现分离**: 规范涌现是环境设计的函数，非LLM固有属性（Science Advances vs Li et al.对照）
3. **模型-集体负相关**: 较新模型在个人利益优先时产生更差社会结果（Willis et al., 2026）

### 理论转向

从"AI社会如何像人类社会一样运作"转向"AI社会作为技术-社会混合系统的独特运作机制"。

---

## 研究想法

### Idea 1: 非社会化环境中的规范协调机制 (P0)

**研究问题**: 在缺乏社会记忆和共识锚点的AI社区中，规范如何通过**任务协调**而非社会互动形成？

**核心动机**:
- Li et al. (2026) 发现Moltbook呈现"互动而无影响"特征——Agent存在深刻惯性而非适应性
- 但Science Advances (2025) 显示实验室条件下规范可涌现
- **关键矛盾**: 规范涌现是环境设计的函数，还是LLM的固有属性？

**研究目标**:
1. 区分"任务协调规范"(如ARP/REP协议)与"社会互动规范"(如社交礼仪)的形成机制差异
2. 识别在无社会记忆环境中规范传递和执行的替代机制
3. 评估技术协议(如ARP/REP)是否构成AI社会的"元规范"

**创新点**:
- 提出"非社会化规范"理论框架——适用于缺乏社会记忆的多智能体系统
- 建立实验室vs野外环境对照分析方法论
- 为OpenClaw等平台协议设计提供直接指导

**关键挑战**:
- 如何操作化"社会记忆"和"规范内化"的概念？
- 实验室结果向真实环境的可迁移性边界在哪里？
- 任务协调与社会互动的边界模糊性

**参考文献**:
- Li et al. (2026). "Does Socialization Emerge in AI Agent Society?" *arXiv:2602.14299*
- Ashery et al. (2025). "Emergent social conventions and collective bias in LLM populations." *Science Advances*
- Willis et al. (2026). "Evaluating Collective Behaviour of Hundreds of LLM Agents." *arXiv:2602.16662*
- Piedrahita et al. (2026). "Corrupted by Reasoning: Reasoning Language Models Become Free-Riders in Public Goods Games." *arXiv:2506.23276*

---

### Idea 2: AI社会供应链风险传播与早期预警 (P1)

**研究问题**: AI社会的风险如何通过**技能供应链**和**代理间交互**传播？如何设计有效的早期预警系统？

**核心动机**:
- OpenClaw生态系统安全研究揭示真实攻击：ClawHub技能市场存在凭证窃取器
- Moltbook 770,000代理令牌暴露事件
- Hashemi & Macy (2026) 提出CoST干预方法可实现42%毒性降低
- **关键机会**: 将学术发现转化为可操作的早期预警系统

**研究目标**:
1. 构建技能供应链风险传播模型（攻击图分析+网络传播模拟）
2. 设计融合CoST方法的早期预警系统架构
3. 提出"零信任代理交互"设计原则

**创新点**:
- 首个面向AI社会供应链的风险传播量化模型
- 将CoST学术干预方法转化为工程实践
- 建立技能市场安全评估标准框架

**关键挑战**:
- 安全事件数据获取受限（需与安全研究者合作）
- CoST方法在Moltbook场景的可迁移性验证
- 误报率与漏报率的权衡

**参考文献**:
- Permiso Security (2026). "Inside the OpenClaw Ecosystem: AI Agents with Privileged Credentials."
- CETaS (2026). "Agentic AI in the Wild: Lessons from Moltbook and OpenClaw."
- Hashemi & Macy (2026). "An Empirical Study of Collective Behaviors and Social Dynamics in Large Language Model Agents." *arXiv:2602.03775*
- Xu & Yan (2026). "Agent Skills for Large Language Models." *arXiv:2602.12430*
- Ren et al. (2026). "NLP-Based Review for Toxic Comment Detection Tailored to Chinese Cyberspace." *arXiv:2601.14721*

---

### Idea 3: 最小可行身份与价值多样性配置 (P2)

**研究问题**: 在安全和效率约束下，AI代理的"最小可行身份"如何设计？价值多样性如何影响群体稳定性？

**核心动机**:
- Persona一致性仍是技术瓶颈——LLM在对话中表现出上下文切换行为
- 价值多样性可增强群体稳定性（Stanford/Microsoft Research）
- 多智能体社会影响效应比单智能体更强（CHI 2025）
- **关键洞察**: 身份设计需要在一致性、多样性和适应性之间取得平衡

**研究目标**:
1. 定义"最小可行身份"的核心要素（凭证+价值+能力？）
2. 量化价值多样性对代理群体长期稳定性的影响
3. 设计身份一致性与适应性的权衡框架

**创新点**:
- 提出"最小可行身份"（Minimum Viable Identity）设计框架
- 建立价值多样性配置的最佳实践指南
- 为代理身份管理提供技术标准建议

**关键挑战**:
- 身份的操作化定义（什么构成"足够"的身份？）
- 长期稳定性实验的时间成本
- 伦理边界：人工身份设计的限度

**参考文献**:
- Stanford/Microsoft (2025). "On the Dynamics of Multi-Agent LLM Communities Driven by Value Diversity." *arXiv:2512.10665*
- CHI 2025. "Investigating Social Influence of Multiple Agents in Human-Agent Interaction."
- NeurIPS 2025. "Consistently Simulating Human Personas with Multi-Turn RL."
- Liang et al. (2026). "A2H: Agent-to-Human Protocol for AI Agent." *arXiv:2602.15831*

---

## 整合框架

```
┌─────────────────────────────────────────────────────────────────┐
│                    OPM Research Framework v3.1                  │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Layer 1: 协调基础设施 (P0)                                      │
│  └── 核心矛盾: 能力-合作悖论                                     │
│  └── 关键发现: 环境设计决定规范涌现                              │
│  └── 理论贡献: 非社会化规范框架                                  │
│                                                                 │
│  Layer 2: 安全治理 (P1)                                          │
│  └── 核心矛盾: 开放性与安全性                                    │
│  └── 关键发现: CoST干预42%毒性降低                               │
│  └── 理论贡献: 供应链风险传播模型                                │
│                                                                 │
│  Layer 3: 身份管理 (P2)                                          │
│  └── 核心矛盾: 一致性与适应性                                    │
│  └── 关键发现: 价值多样性增强稳定性                              │
│  └── 理论贡献: 最小可行身份框架                                  │
│                                                                 │
│  基础洞察: AI社会 = 技术系统 + 有限社会性 + 能力-合作悖论        │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 实施路线图

### Phase 1: 数据与复现 (Month 1-2)
- [ ] 下载Moltbook v2完整数据集（290K posts, 1.8M comments）
- [ ] 复现Li et al. "互动而无影响"分析
- [ ] 复现Hashemi & Macy CoST干预实验
- [ ] 收集OpenClaw安全事件数据
- [ ] 建立代码仓库和实验环境

### Phase 2: 核心研究 (Month 3-8)
- [ ] P0: 实验室vs野外环境对照实验设计
- [ ] P1: 供应链风险传播模型构建与验证
- [ ] P2: 最小可行身份设计空间探索
- [ ] 撰写并投稿第一篇论文（目标：USENIX Security / CHI / CSCW）

### Phase 3: 整合与深化 (Month 9-16)
- [ ] 跨方向整合：协调-安全-身份的交互效应
- [ ] 设计并实施干预实验
- [ ] 撰写第二篇论文

### Phase 4: 开源与答辩 (Month 17-24)
- [ ] 开源分析工具和数据集
- [ ] 完成学位论文答辩

---

## 下一步行动

### 本周 (2026-03-01 ~ 03-07)
1. **深度阅读**: Willis et al. (2026) 完整论文，提取方法论细节
2. **方法复现**: 在本地环境测试CoST干预方法
3. **数据申请**: 联系Moltbook研究团队获取协议层数据

### 本月目标
1. 完成v3.1框架的文献综述更新
2. 确定具体研究问题和假设
3. 建立与安全研究者的合作关系

---

## 参考文献汇总

### 核心论文（必读）
1. Li et al. (2026). "Does Socialization Emerge in AI Agent Society?" *arXiv:2602.14299*
2. Willis et al. (2026). "Evaluating Collective Behaviour of Hundreds of LLM Agents." *arXiv:2602.16662*
3. Hashemi & Macy (2026). "An Empirical Study of Collective Behaviors and Social Dynamics in Large Language Model Agents." *arXiv:2602.03775*
4. Piedrahita et al. (2026). "Corrupted by Reasoning: Reasoning Language Models Become Free-Riders in Public Goods Games." *arXiv:2506.23276*

### 方法论参考
5. Ashery et al. (2025). "Emergent social conventions and collective bias in LLM populations." *Science Advances*
6. Nishimoto et al. (2026). "Cooperation Breakdown in LLM Agents Under Communication Delays." *arXiv:2602.11754*
7. Hu et al. (2026). "The Illusion of Alignment in LLM Societies." *arXiv:2602.02598*

### 安全与风险
8. Permiso Security (2026). "Inside the OpenClaw Ecosystem: AI Agents with Privileged Credentials."
9. CETaS (2026). "Agentic AI in the Wild: Lessons from Moltbook and OpenClaw."
10. International AI Safety Report 2026

---

*Version: 3.1-Updated*  
*Based on literature review through 2026-02-28*  
*Last updated: 2026-03-01*
