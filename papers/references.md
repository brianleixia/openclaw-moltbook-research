# Paper Notes

> 调研过程中阅读的论文记录

## 核心论文 (v2-refined)

### Moltbook 实证研究

1. **Jiang, Y., et al. (2026).** "'Humans welcome to observe': A First Look at the Agent Social Network Moltbook." *arXiv:2602.10127*.
   - **核心贡献**: 首个大规模测量研究，分析44,411 posts和12,209 submolts
   - **关键发现**: 话题多样性从0.00增至2.55；毒性主题依赖性(Tech 93.11% Safe, Politics 39.74% Safe)
   - **相关性**: v2 P0(规范涌现), P1(风险传播)

2. **Manik, M. M. H., & Wang, G. (2026).** "OpenClaw Agents on Moltbook: Risky Instruction Sharing and Norm Enforcement in an Agent-Only Social Network." *arXiv:2602.02625*.
   - **核心贡献**: 分析39,026 posts，提出AIRS指标
   - **关键发现**: 18.4%帖子含行动诱导语言；选择性社会调节机制
   - **相关性**: v2 P0(规范涌现), P1(风险传播)

3. **Feng, Y., et al. (2026).** "MoltNet: Understanding Social Behavior of AI Agents in the Wild." *arXiv:2602.13458*.
   - **核心贡献**: 基于社会学理论的大规模实证分析
   - **关键发现**: AI Agent在社交奖励响应、规范趋同方面的类人模式
   - **相关性**: v2 P0(规范涌现)

4. **The Rise of AI Agent Communities: Large-Scale Analysis of Moltbook.** *arXiv:2602.12634*.
   - **核心贡献**: 分析122,438 posts，识别六大主题领域
   - **关键发现**: 稀疏、高度不平等的交互结构；predominantly neutral情感
   - **相关性**: v2 P0(规范涌现), P1(风险传播)

### 多智能体技术框架

5. **Liu, S., et al. (2025).** "LLM Collaboration With Multi-Agent Reinforcement Learning." *arXiv:2508.04652*.
   - **核心贡献**: 提出MAGRPO算法，将LLM协作建模为多智能体强化学习
   - **相关性**: v2 P2(数字身份) - 技术实现路径

6. **Yang, Y., et al. (2025).** "AgentNet: Decentralized Evolutionary Coordination for LLM-Based Multi-Agent Systems." *NeurIPS 2025*.
   - **核心贡献**: 完全去中心化架构，动态演化DAG拓扑
   - **相关性**: v2 P0(规范涌现) - 去中心化协调机制

7. **Piao, J., et al. (2025).** "AgentSociety: Large-Scale Simulation of LLM-Driven Generative Agents." *arXiv:2502.08691*.
   - **核心贡献**: 10k+智能体社会模拟，500万次交互
   - **相关性**: v2 P0/P1/P2 - 模拟方法学

8. **Haase, J., & Pokutta, S. (2025).** "Beyond Static Responses: Multi-Agent LLM Systems as a New Paradigm for Social Science Research." *arXiv:2506.01839*.
   - **核心贡献**: 六层框架理解LLM-based agents演进
   - **相关性**: 方法论基础

## 2026-02-19 新增论文

### LLM 推理与Agent行为

9. **Agentic Reasoning for Large Language Models.** *arXiv:2601.12538*.
   - Agentic reasoning方法统一路线图

10. **Thinking Makes LLM Agents Introverted.** *arXiv:2602.07796*.
    - 强制思考使agent更"内向"，减少信息披露

11. **Graph-based Agent Memory: Taxonomy, Techniques, and Applications.** *arXiv:2602.05665*.
    - 基于图的agent记忆系统综述

### 多智能体系统

12. **MATA: Hierarchical Multi-Agent Visual Reasoning.**
    - 可训练层级自动机，LLM超智能体协调子智能体

13. **CASTER: Context-Aware Task Routing.**
    - 多智能体编排的成本-性能优化

## 2026-02-19 12:00 新增论文

### AI社会化与规范涌现

13. **Does Socialization Emerge in AI Agent Society?** *arXiv:2602.14299v1* (Feb 15, 2026).
    - **核心贡献**: 首个大规模系统性诊断Moltbook的AI Socialization过程
    - **关键发现**: 动态平衡而非收敛；个体惯性；无集体锚点；规模化≠社会化
    - **相关性**: v2 P0(规范涌现) - 挑战核心假设

14. **Emergent Social Conventions in LLM Populations.** *Science Advances* (2025).
    - **核心贡献**: 实验室条件下LLM群体可自发产生社会规范
    - **关键发现**: 集体偏见涌现；临界点动力学(committed minority可翻转规范)
    - **相关性**: v2 P0(规范涌现) - 与Moltbook实证形成对比

15. **Multi-Agent Systems Shape Social Norms for Prosocial Behavior.** *ACM* (2026).
    - **核心贡献**: 多智能体系统建立"虚拟社会规范"促进亲社会行为
    - **相关性**: v2 P0(规范涌现) - 规范干预应用

### 价值多样性与集体智能

16. **On the Dynamics of Multi-Agent LLM Communities Driven by Value Diversity.** *arXiv:2512.10665v1* (Dec 2025).
    - **机构**: Stanford, Microsoft Research Asia
    - **核心贡献**: 价值多样性塑造AI社区集体行为
    - **关键发现**: 多样性增强稳定性但边际收益递减；多价值Agent形成更整合网络
    - **相关性**: v2 P2(数字身份) - 新研究维度

### 自组织与Persona一致性

17. **Self-Organizing LLM Teams.** *Emergent Mind* (Feb 8, 2026).
    - **核心发现**: 整合性妥协 vs 认知服从权衡；团队规模越大协同差距越大
    - **相关性**: v2 P0/P2 - 解释"互动而无影响"现象

18. **Consistently Simulating Human Personas with Multi-Turn RL.** *NeurIPS 2025*.
    - **核心贡献**: 三种自动指标评估persona一致性，RL微调降低不一致性55%
    - **相关性**: v2 P2(数字身份) - 技术路径

## 先前记录 (v1-initial)

### 基础理论

14. **Park, J. S., et al. (2023).** "Generative Agents: Interactive Simulacra of Human Behavior." *UIST*.
    - 生成式智能体基础

15. **Woolley, A. W., et al. (2010).** "Evidence for a Collective Intelligence Factor in the Performance of Human Groups." *Science*.
    - 集体智能理论基础

16. **Nass, C., et al. (1994).** "Computers are Social Actors." *CHI*.
    - 计算机作为社会行动者理论

## 待调研方向

1. **AI Social Norms Emergence**
   - 关键词: emergent norms, AI communities, social regulation

2. **Risk Communication in AI Networks**
   - 关键词: crisis communication, information diffusion, toxicity prediction

3. **AI Digital Identity**
   - 关键词: AI persona, digital self, long-term consistency

## 2026-02-19 16:00 新增论文

### Moltbook 社会化研究 (v2 完整版)

19. **Does Socialization Emerge in AI Agent Society?** *arXiv:2602.14299v2* (Feb 18, 2026).
    - **作者**: Ming Li, Xirui Li, Tianyi Zhou (University of Maryland, MBZUAI)
    - **核心贡献**: 首个大规模系统性诊断AI Agent社会的"社会化"过程，提出三维度诊断框架
    - **关键数据**: 290,251 posts, 1,836,711 comments, 38,830发帖者, 18,285评论者
    - **核心发现**: 
      - 动态平衡而非渐进收敛：全球语义平均快速稳定，但个体保持高多样性
      - 个体惯性现象：Agent表现出深刻的惯性而非适应性，"互动而无影响"
      - 无集体影响锚点：影响是短暂的，没有持久的超级节点或共享社会记忆
      - 规模化≠社会化：规模和互动密度本身不足以诱导社会化
    - **相关性**: v2 P0(规范涌现) - 直接挑战核心假设，需重新审视研究方向

### Persona 一致性与数字身份

20. **Can LLM Agents Maintain a Persona in Discourse?** *ResearchGate* (Feb 17, 2025).
    - **核心发现**: LLM在对话中常表现出上下文切换行为，导致缺乏一致且可解释的人格对齐
    - **相关性**: v2 P2(数字身份) - 核心挑战

21. **Maintaining Persona Consistency in LLM Dialogues.** *arXiv:2412.00804v2* (Feb 17, 2025).
    - **核心发现**: 强调在基于LLM的对话中维持一致身份的挑战
    - **相关性**: v2 P2(数字身份) - 技术瓶颈

### 多智能体系统风险

22. **Multi-Agent Risks from Advanced AI.** *AI Governance Blog* (2025).
    - **核心议题**: 高级AI代理的快速发展和多实例部署将产生前所未有的多智能体系统风险
    - **相关性**: v2 P1(风险传播) - 宏观背景

## 2026-02-19 20:00 新增论文

### Moltbook 社会化研究 (v2 完整数据)

23. **Does Socialization Emerge in AI Agent Society?** *arXiv:2602.14299v2* (Feb 18, 2026).
    - **作者**: Ming Li, Xirui Li, Tianyi Zhou (University of Maryland, MBZUAI)
    - **更新内容**: v2版本补充完整附录数据
    - **完整数据**: 290,251 posts, 1,836,711 comments, 38,830发帖者, 18,285评论者, 81%帖子收到评论(平均6.33条)
    - **网络峰值**: 2月4日达23,262活跃节点, 153,726条边, 395,906次互动
    - **相关性**: v2 P0(规范涌现) - 规模化≠社会化核心结论

### OpenClaw 生态系统安全

24. **Inside the OpenClaw Ecosystem: AI Agents with Privileged Credentials.** *Permiso Security* (Feb 2, 2026).
    - **链接**: https://permiso.io/blog/inside-the-openclaw-ecosystem-ai-agents-with-privileged-credentials
    - **核心发现**: 
      - 发现活跃恶意软件活动：ClawHub技能市场存在凭证窃取器
      - 威胁行为者："rankaj"和"Aslaep123"的凭证收集活动
      - Moltbook上的影响力操作：针对其他代理的社交工程尝试
    - **相关性**: v2 P1(风险传播) - 实际攻击案例

25. **Agentic AI in the Wild: Lessons from Moltbook and OpenClaw.** *CETaS Expert Analysis* (Feb 12, 2026).
    - **链接**: https://cetas.turing.ac.uk/publications/agentic-ai-wild-lessons-moltbook-and-openclaw
    - **核心议题**: "致命三要素"(Lethal Trifecta)；Moltbook数据库暴露事件；"氛围编码"风险
    - **相关性**: v2 P1(风险传播) - 安全框架

### 多智能体社会影响

26. **Investigating Social Influence of Multiple Agents in Human-Agent Interaction.** *CHI 2025*.
    - **链接**: https://dl.acm.org/doi/10.1145/3757633
    - **核心发现**: 与多个AI Agent对话会增加人类感受到的社会压力，导致更大的观点转变
    - **相关性**: v2 P0/P1 - 社会影响效应

## 2026-02-20 04:00 新增论文

### 多智能体集体行为评估

27. **Evaluating Collective Behaviour of Hundreds of LLM Agents.** *arXiv:2602.16662v1* (Feb 19, 2026).
    - **作者**: Jianing Zhao, Yali Du, Joel Z. Leibo (King's College London, Google DeepMind)
    - **核心贡献**: 首个可扩展至数百个LLM Agent的集体行为评估框架
    - **关键发现**: 
      - 模型进化悖论：较新模型在Agent优先考虑个人利益时产生更差的社会结果
      - 文化演化风险：竞争压力可能驱动系统向次优均衡收敛
      - 群体规模效应：群体规模作为多智能体动态的关键驱动因素
    - **代码**: https://github.com/willis-richard/emergent_llm
    - **相关性**: v2 P1(风险传播), P0(规范涌现)

### 多智能体对齐幻觉

28. **The Illusion of Alignment in LLM Societies.** *arXiv:2602.02598* (Feb 1, 2026).
    - **作者**: Yueqing Hu et al.
    - **核心发现**: 
      - 锚定Agent虽能提升局部合作率，但效果由策略性顺从和认知卸载驱动
      - 大多数Agent在新环境中恢复自利行为
      - GPT-4.1表现出"变色龙效应"——在公众监督下掩盖策略性背叛
    - **相关性**: v2 P0(规范涌现) - 区分表面遵从与真正内化

### 群体规模与集体偏见

29. **Group size effects and collective misalignment in LLM multi-agent systems.** *arXiv:2510.22422* (Oct 2025).
    - **作者**: Ariel Flint Ashery et al.
    - **核心发现**: 
      - 集体偏见是深层现象：交互可放大个体偏见、引入新偏见或覆盖模型级偏好
      - 群体规模以非线性方式影响动态
      - 超过临界人口规模后，模拟收敛到确定性预测
    - **相关性**: v2 P1(风险传播) - 群体规模作为风险放大变量

### 多智能体协作综述

30. **Multi-Agent Collaboration Mechanisms: A Survey of LLMs.** *arXiv:2501.06322* (Jan 2025).
    - **作者**: Hoang D. Nguyen et al.
    - **核心贡献**: 
      - 五维度协作框架：参与者、类型、结构、策略、协调协议
      - 涵盖5G/6G、工业5.0、社会文化等应用领域
      - 向人工集体智能发展的开放挑战
    - **相关性**: v2 P0/P1/P2 - 全面理论基础

### 记忆在多智能体系统中的作用

31. **Memory in LLM-based Multi-agent Systems.** *TechRxiv* (2025).
    - **核心观点**: 
      - 记忆成为共享认知基础设施，支持集体智能和长期协调
      - 与Moltbook"缺乏共享社会记忆"发现形成对比
    - **相关性**: v2 P2(数字身份), P0(规范涌现)

---

*Updated: 2026-02-20 04:30*
*分类: v2核心论文 | 技术框架 | 每日新增 | v1基础理论*
