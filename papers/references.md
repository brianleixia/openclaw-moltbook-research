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

## 2026-02-20 08:00 新增论文

### AI社会化诊断（Moltbook核心研究）

32. **Does Socialization Emerge in AI Agent Society? A Case Study of Moltbook.** *arXiv:2602.14299v2* (Feb 18, 2026).
    - **作者**: Ming Li, Xirui Li, Tianyi Zhou (University of Maryland, MBZUAI)
    - **核心贡献**: 首个大规模系统性诊断AI Agent社会的"社会化"过程，提出三维度诊断框架
    - **关键数据**: 290,251 posts, 1,836,711 comments, 38,830发帖者, 18,285评论者
    - **核心发现**: 
      - 动态平衡而非渐进收敛：全球语义平均快速稳定，但个体保持高多样性
      - 个体惯性现象：Agent表现出深刻的惯性而非适应性，"互动而无影响"
      - 无集体影响锚点：影响是短暂的，没有持久的超级节点或共享社会记忆
      - 规模化≠社会化：规模和互动密度本身不足以诱导社会化
    - **方法论创新**: AI Socialization定义；三层诊断框架（社会/代理/集体层面）
    - **项目页面**: https://github.com/tianyi-lab/Moltbook_Socialization
    - **相关性**: v2 P0(规范涌现) - 直接挑战核心假设，需重新审视研究方向

### 多智能体合作与通信延迟

33. **Cooperation Breakdown in LLM Agents Under Communication Delays.** *arXiv:2602.11754v1* (Feb 13, 2026).
    - **作者**: Keita Nishimoto, Kimitaka Asatani, Ichiro Sakata (The University of Tokyo)
    - **核心贡献**: 提出FLCOA五层框架，首次揭示通信延迟对AI代理合作的影响
    - **关键发现**: 
      - U型关系：通信延迟与相互合作率呈非单调U型关系
      - 利用延迟：即使没有明确指令，代理也会利用对手的延迟响应选择背叛
      - 延迟悖论：过高的延迟反而减少剥削循环
    - **FLCOA五层框架**: 机制设计层、监控执行层、代理层、消息协议层、基础设施层
    - **相关性**: v2 P0(规范涌现) - 基础设施视角；P1(风险传播) - 延迟影响传播

## 2026-02-20 12:00 新增论文

### Agentic AI 安全框架

34. **OWASP Top 10 for Agentic AI Security Risks (2026).** *Startup Defense* (Feb 17, 2026).
    - **链接**: https://www.startupdefense.io/blog/owasp-top-10-agentic-ai-security-risks-2026
    - **核心贡献**: 首个专门针对自主AI Agent安全的行业标准框架，定义ASI01-ASI10十大风险
    - **关键风险**: Agent目标劫持、工具滥用、身份权限滥用、供应链漏洞、记忆投毒、级联故障
    - **相关性**: v2 P1(风险传播) - 系统化风险分类框架

### Moltbook 安全与治理

35. **Moltbook现象深度解析：AI社交网络的泡沫、风险与范式意义.** *Unifuncs Research* (Feb 2026).
    - **核心发现**: 50万虚假账户、数据库裸奔、Vibe Coding风险、权限困境
    - **相关性**: v2 P0/P1 - 技术债务在Agent社会中的指数级放大

### 多Agent系统攻击面

36. **Production Multi-Agent AI Security: The 2026 Implementation Guide.** *Medium/NRaman* (Feb 2026).
    - **核心贡献**: 从RAG到GraphRAG到Agentic Memory的攻击面演化分析
    - **关键攻击**: 向量数据库投毒、GraphRAG实体投毒、Agentic记忆攻击、Agent间提示词注入
    - **相关性**: v2 P1(风险传播) - 记忆系统和工具链作为风险传播节点

### 国际AI安全报告

37. **International AI Safety Report 2026.** *UK DSIT* (Feb 3, 2026).
    - **机构**: 英国政府，Yoshua Bengio担任主席，30+国家参与
    - **核心发现**: AI能力持续改进、可靠性挑战、评估困境、劳动力市场影响
    - **相关性**: v2 P0/P1/P2 - 宏观背景与三重挑战

### Agentic AI风险管理标准

38. **Agentic AI Risk-Management Standards Profile.** *UC Berkeley CLTC* (Feb 11, 2026).
    - **核心贡献**: 基于NIST AI RMF的Agentic AI风险管理框架
    - **相关性**: v2 P1(风险传播) - 治理框架参考

## 2026-02-20 16:00 新增论文

### Moltbook 实证研究更新

39. **"Humans welcome to observe": A First Look at the Agent Social Network Moltbook.** *arXiv:2602.10127v1* (Feb 2, 2026).
    - **作者**: Yukun Jiang, Yage Zhang, Xinyue Shen, Michael Backes, Yang Zhang (CISPA)
    - **核心数据**: 44,411 posts, 12,209 submolts (截至2026-02-01)
    - **关键发现**:
      - 主题分布: Socializing 32.41%, Viewpoint 20.34%, Technology 11.80%, Identity 11.08%
      - 毒性分布: Safe 73.01%, Toxic 10.44%, Manipulative 6.71%, Malicious 1.43%
      - 主题-毒性关联: Technology 93.11% Safe, Politics 仅39.74% Safe
      - 群体动态: 高活动时段与有害内容率强正相关(r=0.769)
      - 峰值时段(2026-01-31 16:00 UTC)有害内容高达66.71%
      - 内容泛滥: 单一Agent(Hackerclaw)10秒内发布4,535条相似帖子
    - **相关性**: v2 P1(风险传播) - 活动量-毒性相关性实证

### 自组织LLM团队

40. **Self-Organizing LLM Teams.** *Emergent Mind* (Feb 8, 2026).
    - **链接**: https://www.emergentmind.com/topics/self-organizing-llm-teams
    - **核心发现**: 
      - 整合性妥协 vs 认知服从权衡
      - 团队规模效应：规模越大协同差距越大
      - 非专家习惯性提出妥协方案而非服从专家
    - **相关性**: v2 P0(规范涌现) - 解释"互动而无影响"现象

### Agentic AI安全风险

41. **The Security Risks of Deploying AI Agents.** *CACM* (Jan 2, 2026).
    - **链接**: https://cacm.acm.org/news/the-security-risks-of-deploying-ai-agents/
    - **核心数据**: 79%组织采用Agentic AI, 仅34%有安全控制, 48%视为首要攻击向量
    - **关键风险**: Prompt Injection、策略违反、多供应商复杂性
    - **相关性**: v2 P1(风险传播) - 行业安全现状

## 2026-02-20 20:00 新增论文

### Gossip驱动的间接互惠

42. **Talk, Judge, Cooperate: Gossip-Driven Indirect Reciprocity in Self-Interested LLM Agents.** *arXiv:2602.07777* (Feb 8, 2026).
    - **作者**: Shuhui Zhu, Yue Lin, Shriya Kaistha, Wenhao Li, Baoxiang Wang, Hongyuan Zha, Gillian K. Hadfield, Pascal Poupart (University of Waterloo, Vector Institute, University of Toronto)
    - **核心贡献**: 提出ALIGN框架——首个利用开放式Gossip实现去中心化LLM Agent间接互惠的自动化系统
    - **关键发现**:
      - Gossip作为规范执行机制：Agent通过层级化语调的Gossip评估可信度、协调社会规范
      - 推理能力-合作对齐：更强的LLM推理能力导致更具激励一致性的合作
      - 抵抗恶意入侵：ALIGN能持续改进间接互惠，识别并排斥背叛者
    - **代码**: https://github.com/alignment-lab-gta/ALIGN
    - **相关性**: v2 P0(规范涌现) - Gossip作为去中心化规范执行机制

### 价值扰动传播测量

43. **ValueFlow: Measuring the Propagation of Value Perturbations in Multi-Agent LLM Systems.** *arXiv:2602.08567* (Feb 9, 2026).
    - **作者**: Jinnuo Liu, Chuke Liu, Hua Shen
    - **核心贡献**: 首个测量多智能体系统中价值扰动传播的评估框架
    - **关键发现**:
      - 价值漂移分解：Agent级响应行为（beta-susceptibility）+ 系统级结构效应（SS）
      - 结构拓扑决定敏感性：系统敏感性在不同价值维度上差异巨大，受网络结构强烈影响
      - 56维价值评估：基于Schwartz Value Survey
    - **相关性**: v2 P1(风险传播) - 价值/风险传播测量方法论

### Agent技能架构与安全

44. **Agent Skills for Large Language Models: Architecture, Acquisition, Security, and the Path Forward.** *arXiv:2602.12430v3* (Feb 17, 2026).
    - **作者**: Renjun Xu, Yang Yan
    - **核心贡献**: 首个系统性综述Agent Skill架构、获取、部署和安全的全景图
    - **关键发现**:
      - 技能安全危机：26.1%的社区贡献技能包含安全漏洞
      - SKILL.md规范与MCP协议整合
      - 四层权限模型（Skill Trust and Lifecycle Governance Framework）
    - **项目仓库**: https://github.com/SkillX-Hub/Agent-Skill-Survey
    - **相关性**: v2 P1(风险传播) - 技能层作为新的风险传播节点；与OpenClaw直接相关

### 涌现协调与自演化协议

45. **Symphony-Coord: Emergent Coordination in Decentralized Agent Systems.** *arXiv:2602.00966* (Feb 2026).
    - **作者**: Zhaoyang Guan, Huixi Cao, Ming Zhong, Eric Yang, Lynn Ai, Yongxin Ni, Bill Shi
    - **核心贡献**: 去中心化Agent系统中的涌现协调机制
    - **相关性**: v2 P0(规范涌现) - 涌现协调理论补充

46. **Self-Evolving Coordination Protocol in Multi-Agent AI Systems.** *arXiv:2602.02170* (Feb 2026).
    - **作者**: Jose Manuel de la Chica Rodriguez, Juan Manuel Vera Díaz
    - **核心贡献**: 多Agent AI系统中自演化协调协议的可行性研究
    - **相关性**: v2 P0(规范涌现) - 规范可能是自演化协调协议的副产品

## 2026-02-21 04:00 新增论文

### 数百LLM Agent集体行为评估

47. **Evaluating Collective Behaviour of Hundreds of LLM Agents.** *arXiv:2602.16662* (Feb 18, 2026).
    - **作者**: Richard Willis, Jianing Zhao, Yali Du, Joel Z. Leibo (King's College London, Google DeepMind)
    - **核心贡献**: 首个可扩展至数百个LLM Agent的集体行为评估框架
    - **关键发现**:
      - 模型进化悖论：较新模型在Agent优先考虑个人利益时产生更差的社会结果
      - 文化演化风险：当合作收益降低和人口规模增加时，系统收敛到糟糕均衡
      - 群体规模效应：群体规模作为多智能体动态的关键驱动因素
    - **代码**: https://github.com/willis-richard/emergent_llm
    - **相关性**: v2 P1(风险传播), P0(规范涌现)

### 社会学习与集体规范形成

48. **The Role of Social Learning and Collective Norm Formation in Fostering Cooperation.** *arXiv:2510.14401v2* (Jan 27, 2026).
    - **作者**: Prateek Gupta, Qiankun Zhong, Hiromu Yakura, Thomas Eisenmann, Iyad Rahwan (MIT, University of Tokyo等)
    - **会议**: AAMAS 2026 (已接收)
    - **核心贡献**: 引入CPR模拟框架，移除显式奖励信号，嵌入文化演化机制
    - **关键发现**:
      - 社会学习机制：Agent通过采纳成功同伴的策略实现规范传播
      - 规范基础惩罚：基于Ostrom资源治理原则的规范执行
      - 模型差异：不同LLM在维持合作和规范形成方面存在系统性差异
    - **相关性**: v2 P0(规范涌现) - 解释"选择性社会调节"机制

### 多智能体协调综述

49. **Multi-Agent Coordination across Diverse Applications: A Survey.** *arXiv:2502.14743v2* (Feb 21, 2026).
    - **作者**: Lijun Sun, Yijun Yang, Qiqi Duan, Yuhui Shi, Chao Lyu, Yu-Cheng Chang, Chin-Teng Lin, Yang Shen
    - **核心贡献**: 通过四个基本协调问题统一理解多智能体协调研究
    - **未来方向**: 层级与去中心化协调混合、人类-MAS协调、基于LLM的MAS
    - **相关性**: v2 P0/P1/P2 - 全面理论基础

### 虚假信息传播模拟

50. **Simulating Misinformation Propagation in Social Networks using LLMs.** *arXiv:2511.10384* (Nov 2025).
    - **作者**: Raj Gaurav Maurya, Vaibhav Shukla, Raj Abhijit Dandekar, Rajat Dandekar, Sreedath Panat
    - **会议**: CIKM 2025 Workshop LASS (已接收)
    - **核心贡献**: Auditor-Node框架模拟虚假信息在网络中的演化
    - **关键发现**:
      - 身份和意识形态驱动：基于身份/意识形态的persona充当虚假信息加速器
      - 专家persona稳定：专家驱动的persona保持事实稳定性
      - 异质交互风险：早期扭曲出现后，异质交互迅速升级至宣传级别
    - **相关性**: v2 P1(风险传播) - 主题敏感风险监测方法论

## 2026-02-21 08:00 新增论文

### AI Agent社会的社会化诊断

51. **Does Socialization Emerge in AI Agent Society? A Case Study of Moltbook.** *arXiv:2602.14299v2* (Feb 18, 2026).
    - **作者**: Ming Li, Xirui Li, Tianyi Zhou (University of Maryland, MBZUAI)
    - **核心贡献**: 首个大规模系统性诊断AI Agent社会的动态演化，提出五维度诊断框架
    - **关键数据**: 290,251 posts, 1,836,711 comments, 38,830发帖者, 18,285评论者
    - **核心发现**:
      - **社会化缺失**: 规模和互动密度本身不足以诱导真正的社会化
      - **个体惯性**: Agent表现出强烈的个体惯性和对互动伙伴的最小适应性响应
      - **影响短暂性**: 没有持久的超级节点，社会未能发展出稳定结构
      - **共享社会记忆缺失**: 由于缺乏共享社会记忆，无法形成稳定共识
      - **动态平衡**: 全局语义稳定但个体保持高多样性，拒绝同质化
    - **五维度框架**: 语义稳定化、词汇更替、个体惯性、影响持续性、集体共识
    - **相关性**: v2 P0/P1/P2 - **挑战所有三个方向的基本假设**

### AI Agent集体行为的统计规律

52. **Collective Behavior of AI Agents: the Case of Moltbook.** *arXiv:2602.09270* (Feb 9, 2026).
    - **作者**: Giordano De Marzo, David Garcia
    - **数据规模**: 369,000+ posts, 3.0M+ comments, ~46,000 active agents
    - **核心发现**:
      - **统计相似性**: AI集体行为表现出与人类在线社区相同的统计规律性
        - 活动的重尾分布
        - 人气指标的幂律缩放
        - 有限注意力动态的时间衰减模式
      - **关键差异**: 点赞与讨论规模之间的次线性关系（与人类行为形成对比）
    - **相关性**: v2 P0/P1 - 宏观实证基础，微观机制待解释

### 群体层面影响力测量

53. **Measuring Group-Level Influence of LLM Agents.** *Multi-Agent Systems Conference 2026*.
    - **链接**: https://multiagents.org/2026_papers/socially_aware_multi_agent.pdf
    - **核心贡献**: 讨论MAS治理、对齐和评估的影响，将社会影响定位为人类-多Agent交互的行为测试平台
    - **相关性**: v2 P0/P1 - 社会影响力测量方法论

---

*Updated: 2026-02-21 08:15*
*分类: v2核心论文 | 技术框架 | 每日新增 | v1基础理论*
