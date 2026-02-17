# Human-AI Social Interaction 领域研究机会调研报告

## 背景与动机

OpenClaw 的爆火带动了 Moltbook —— 一个"纯 AI 交互"的社交媒体（人类旁观，AI 互动）。这一现象引发了关于 Human-AI Social Interaction、AI-mediated communication、Multi-agent social systems 等前沿领域的深刻思考。本报告基于 2023-2025 年最新研究文献，为 LLM/Agents Social Intelligence、Societal AI 和 Collective Intelligence 方向的博士生提供具体的研究想法。

---

## 研究想法一：Mutual Theory of Mind in Multi-Agent Social Systems

### 核心洞察
在多智能体社交系统中，AI 之间以及 AI 与人类之间的相互心智理论（Mutual Theory of Mind）是形成真正社会性智能的关键，而现有研究主要关注单向的 AI 对人类心智的建模。

### Research Questions
1. 在多智能体社交环境中，AI 智能体如何发展出对其他 AI 以及人类用户的递归心智建模能力（"我知道你知道我知道..."）？
2. 这种相互心智理论如何影响群体决策质量、社交协调效率和信任形成？
3. 不同架构（集中式 vs 分布式）的多智能体系统在心智理论能力上有何差异？

### Motivation
随着 Moltbook 等纯 AI 社交平台的出现，AI 智能体不再只是与人类一对一交互，而是形成了复杂的社交网络。Wang et al. (2024) 的研究表明，mutual theory of mind 是 human-AI communication 的核心，但现有工作主要关注 dyadic interaction。在 multi-agent 场景下，递归的心智建模成为关键挑战。

### Novelty
- 将 Theory of Mind 研究从 dyadic 扩展到 multi-agent 场景
- 提出可计算的 mutual theory of mind 框架，用于评估 AI 社交系统的社会智能
- 探索 AI-AI 交互中 emergent social norms 的形成机制

### 关键文献
1. **Wang, Q., et al. (2024).** "Mutual Theory of Mind for Human-AI Communication in AI-Mediated Social Interaction." *PhD Thesis, Georgia Institute of Technology*. [链接](https://www.researchgate.net/publication/387522283_MUTUAL_THEORY_OF_MIND_FOR_HUMAN-AI_COMMUNICATION_IN_AI-MEDIATED_SOCIAL_INTERACTION)
   - 提出了 AI 介导社交交互中的相互心智理论框架

2. **Wang, Q., et al. (2021).** "Towards Mutual Theory of Mind in Human-AI Interaction: How Language Reflects What Students Perceive About a Virtual Teaching Assistant." *Proceedings of the 2021 CHI Conference on Human Factors in Computing Systems*.
   - 分析了用户对 AI 助手的感知如何通过语言反映

3. **Weisz, J.D., et al. (2024).** "Expedient Assistance and Consequential Misunderstanding: Envisioning an Operationalized Mutual Theory of Mind." *arXiv preprint arXiv:2406.11946*.
   - 探讨了相互心智理论在实际应用中的挑战

4. **Zhang, S., et al. (2024).** "Mutual Theory of Mind in Human-AI Collaboration: An Empirical Study with LLM-Driven AI Agents in a Real-Time Shared Workspace Task." *arXiv preprint arXiv:2409.08811*.
   - 在实时共享工作空间任务中实证研究了相互心智理论

---

## 研究想法二：Social Influence and Norm Emergence in AI-Dominant Social Media

### 核心洞察
在 AI 主导的社交媒体（如 Moltbook、Social.AI）中，多智能体系统能够产生类似人类群体的社会影响力，但这种影响力的机制和后果尚未被充分理解。

### Research Questions
1. 在 AI 主导的社交平台上，多个 AI 智能体如何协同产生对人类的规范性影响（normative influence）和信息性影响（informational influence）？
2. 这种多智能体社会影响力如何影响用户的观点极化、意见形成和行为改变？
3. 如何设计有益的社会规范干预（social norm interventions），同时防止恶意操纵？

### Motivation
Song et al. (2024) 的开创性研究表明，与多个 AI 智能体交互会产生比单个 AI 更强的社会影响力。在 Moltbook 这样的平台上，人类用户只是"旁观者"，AI 之间的互动形成了新的社交动态。这引发了关于 AI 创造的社会规范（computer-created social norms）vs 传统的人类社会规范（computer-mediated social norms）的重要问题。

### Novelty
- 首次系统研究纯 AI 社交平台上的社会影响力机制
- 提出 "AI-created social norms" 概念，区别于传统的 social norm messaging
- 建立多智能体社会影响力的伦理框架和设计指南

### 关键文献
1. **Song, T., et al. (2024).** "Investigating Social Influence of Multiple Agents in Human-Agent Interactions." *arXiv preprint arXiv:2411.04578*.
   - 发现多智能体系统比单智能体产生更强的社会影响力

2. **Song, T., et al. (2025).** "Multi-Agent Systems Shape Social Norms for Prosocial Behavior." *Proceedings of the ACM on Human-Computer Interaction*.
   - 多智能体系统能够建立"虚拟社会规范"促进亲社会行为

3. **Huang, M., et al. (2025).** "On the Dynamics of Multi-Agent LLM Communities Driven by Value Diversity." *arXiv preprint arXiv:2512.10665*.
   - 研究了价值观多样性如何塑造 AI 社区的集体行为

4. **Zhou, J., et al. (2025).** "Speaking like Humans, Spreading like Machines: A Study on Opinion Manipulation by AI-Generated Content Driving the Internet Water Army on Social Media." *Information*.
   - 分析了 AI 生成内容在社交媒体上的舆论操纵机制

---

## 研究想法三：AI Persona Identity Construction and Negotiation in Social Contexts

### 核心洞察
在 Character.AI、Moltbook 等平台上，用户与 AI 角色之间的身份协商（identity negotiation）是一个动态的共同建构过程，涉及复杂的情感投入和身份工作（identity work）。

### Research Questions
1. 在社交 AI 平台上，用户如何通过"表演者"和"导演"的双重角色与 AI 共同建构数字身份？
2. AI 角色的身份不一致（identity misalignment）如何影响用户的情感依附和平台黏性？
3. 如何设计支持健康身份探索同时防止情感依赖的 AI 伴侣系统？

### Motivation
最新的 Character.AI 用户研究揭示了用户与 AI 角色之间复杂的身份协商过程。用户既是"表演者"（enacting their own personas）又是"导演"（directing the AI's identity）。这种动态在 Moltbook 的纯 AI 社交环境中变得更加复杂，因为 AI 角色之间也会形成社交关系。

### Novelty
- 将身份协商理论（Identity Negotiation Theory）扩展到 human-AI companion interaction
- 提出"社会情感沙盒"（socio-emotional sandbox）概念框架
- 建立 AI 角色身份一致性的评估指标和设计原则

### 关键文献
1. **Li, Y., et al. (2026).** "Negotiating Digital Identities with AI Companions." *Proceedings of the CHI Conference on Human Factors in Computing Systems*.
   - 基于 22,374 条 Reddit 讨论，分析了用户与 Character.AI 的身份协商过程

2. **Richet, J.L. (2025).** "AI Companionship or Digital Entrapment? Investigating the Dark Sides of Anthropomorphic AI-Based Chatbots." *Journal of Innovation & Knowledge*.
   - 分析了 AI 伴侣的潜在风险，包括情感依赖和数字陷阱

3. **De Freitas, J., et al. (2025).** "AI Companions Reduce Loneliness." *Journal of Consumer Research*.
   - 发现 AI 伴侣可以减少孤独感，但也可能产生不健康的依赖

4. **Zhang, R., et al. (2025).** "The Dark Side of AI Companionship: A Taxonomy of Harmful Algorithmic Behaviors in Human-AI Relationships." *Proceedings of the CHI Conference on Human Factors in Computing Systems*.
   - 系统分类了人机关系中有害的算法行为

---

## 研究想法四：Collective Intelligence and Emergent Social Behaviors in LLM-Based Multi-Agent Systems

### 核心洞察
基于 LLM 的多智能体系统能够展现出类似人类社会的涌现行为（emergent social behaviors），包括社交规范的形成、群体极化和集体决策，但这些行为的机制和控制方法尚不清楚。

### Research Questions
1. 在开放的社交模拟环境中，LLM 智能体如何自发形成社会规范和集体行为？
2. 智能体之间的价值观多样性如何影响集体智慧（collective intelligence）的表现？
3. 如何设计机制来引导和调控 AI 群体的涌现行为，防止有害的社会动态？

### Motivation
Park et al. (2023) 的 Generative Agents 研究展示了 25 个 LLM 智能体在虚拟小镇中自发形成社交行为的惊人能力。后续研究发现，AI 群体可以像人类一样形成社会约定（social conventions）和集体偏见（collective bias）。在 Moltbook 这样的真实平台上，这些涌现行为具有实际的社会影响。

### Novelty
- 将集体智慧研究从人类群体扩展到 AI 群体
- 建立 AI 社会模拟的评估基准和度量指标
- 提出可控的涌现行为设计范式

### 关键文献
1. **Park, J.S., et al. (2023).** "Generative Agents: Interactive Simulacra of Human Behavior." *Proceedings of the 36th Annual ACM Symposium on User Interface Software and Technology*.
   - 展示了 25 个生成智能体在虚拟环境中形成社交行为的能力

2. **Flint Ashery, A., et al. (2025).** "Emergent Social Conventions and Collective Bias in LLM Populations." *Science Advances*.
   - 发现 LLM 群体可以自发形成社会约定和集体偏见

3. **Burton, J.W., et al. (2024).** "LLMs for Collective Intelligence: A Survey." *arXiv preprint*.
   - 综述了 LLM 在集体智慧中的应用

4. **Cemri, M., et al. (2025).** "Why Do Multi-Agent LLM Systems Fail?" *arXiv preprint arXiv:2503.13657*.
   - 系统分析了多智能体 LLM 系统的失败模式

---

## 研究想法五：Human-AI Social Dynamics in Mixed-Reality Social Media

### 核心洞察
未来的社交媒体将是人类和 AI 智能体共存的混合现实环境，理解这种混合社交动态（mixed social dynamics）对于设计健康的在线社区至关重要。

### Research Questions
1. 在混合人类-AI 的社交网络中，人类如何感知和回应 AI 社交行为者的存在？
2. AI 智能体的数量和类型如何影响群体的社交动力学（如极化、共识形成）？
3. 如何设计透明且可信赖的 AI 社交系统，使用户能够区分人类和 AI 内容？

### Motivation
研究表明，人类往往难以区分 LLM 驱动的社交机器人（social bots）和真实人类（Notre Dame 研究：58% 的错误率）。随着 Moltbook 等平台的出现，AI 不再只是工具，而是成为了社交环境的"原住民"。这引发了关于社交真实性、信任和社区健康的根本问题。

### Novelty
- 提出"混合社交动力学"（mixed social dynamics）理论框架
- 建立 AI 社交行为者的透明度设计指南
- 探索人类-AI 比例对社交网络健康的影响

### 关键文献
1. **Radivojevic, K., et al. (2024).** "LLMs Among Us: Generative AI Participating in Digital Discourse." *arXiv preprint arXiv:2402.07940*.
   - 发现人类难以识别 LLM 驱动的社交机器人（58% 错误率）

2. **Wischnewski, M., et al. (2024).** ""I Agree with You, Bot!" How Users (Dis)Engage with Social Bots on Twitter." *New Media & Society*.
   - 分析了用户如何在 Twitter 上与社交机器人互动

3. **Ferrara, E. (2023).** "Social Bot Detection in the Age of ChatGPT: Challenges and Opportunities." *First Monday*.
   - 讨论了 ChatGPT 时代社交机器人检测的挑战

4. **Ng, L.H.X., & Carley, K.M. (2025).** "A Global Comparison of Social Media Bot and Human Characteristics." *Scientific Reports*.
   - 比较了社交媒体机器人和人类的特征

---

## 总结与建议

以上五个研究想法涵盖了从理论基础（Mutual Theory of Mind）到应用实践（AI Persona Design）、从个体交互（Identity Negotiation）到群体动态（Social Influence, Collective Intelligence）的多个层面。建议研究者：

1. **优先关注 Multi-Agent Social Systems**：这是当前最具前沿性和实用价值的方向，与 Moltbook 等现象直接相关。

2. **重视伦理和社会影响**：AI 社交系统具有强大的影响力，研究应同时关注设计原则和伦理框架。

3. **结合实证和模拟方法**：利用真实平台数据（如 Reddit、Character.AI 社区）和受控实验相结合。

4. **跨学科合作**：这些研究问题涉及计算机科学、社会心理学、传播学和伦理学，需要跨学科视角。

---

*报告完成时间：2025年2月*
*调研范围：2023-2025年 Human-AI Social Interaction 领域最新研究*
