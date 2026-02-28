

## 2026-02-24 04:00 新增论文

### AI社会化诊断（核心发现）

63. **Does Socialization Emerge in AI Agent Society?** *arXiv:2602.14299* (Feb 18, 2026).
    - **作者**: Ming Li, Xirui Li, Tianyi Zhou (University of Maryland, MBZUAI)
    - **核心贡献**: 首个大规模系统性诊断AI Agent社会的"社会化"过程，提出五维度诊断框架
    - **关键数据**: 290,251 posts, 1,836,711 comments, 38,830发帖者, 18,285评论者
    - **核心发现**: 
      - 动态平衡而非渐进收敛：全局语义平均快速稳定，但个体保持高多样性
      - 个体惯性现象：Agent表现出深刻的惯性而非适应性，"互动而无影响"
      - 无集体影响锚点：影响是短暂的，没有持久的超级节点或共享社会记忆
      - 规模化≠社会化：规模和互动密度本身不足以诱导社会化
    - **相关性**: v2 P0(规范涌现) - **直接挑战核心假设，需重新审视研究方向**

### 从众行为与社会影响

64. **Conformity and Social Impact on AI Agents.** *arXiv:2601.05384* (Jan 2026).
    - **核心贡献**: 揭示LLM Agent的从众偏差机制
    - **相关性**: v2 P0(规范涌现) - 解释"选择性社会调节"

### Gossip驱动的间接互惠

65. **Talk, Judge, Cooperate: Gossip-Driven Indirect Reciprocity.** *arXiv:2602.07777* (Feb 8, 2026).
    - **作者**: Shuhui Zhu et al. (University of Waterloo, Vector Institute)
    - **核心贡献**: ALIGN框架——首个利用开放式Gossip实现去中心化规范执行的系统
    - **关键发现**: Gossip作为规范执行机制；推理能力-合作对齐
    - **相关性**: v2 P0(规范涌现) - Gossip作为去中心化规范执行机制

### 价值扰动传播测量

66. **ValueFlow: Measuring the Propagation of Value Perturbations.** *arXiv:2602.08567* (Feb 9, 2026).
    - **作者**: Jinnuo Liu, Chuke Liu, Hua Shen
    - **核心贡献**: 首个测量多智能体系统中价值扰动传播的评估框架
    - **方法论**: Agent级响应行为(beta-susceptibility) + 系统级结构效应(SS)
    - **相关性**: v2 P1(风险传播) - 价值/风险传播测量方法论

### 虚假信息传播模拟

67. **Simulating Misinformation Propagation using LLMs.** *arXiv:2511.10384* (Nov 2025).
    - **会议**: CIKM 2025 Workshop LASS
    - **核心贡献**: Auditor-Node框架模拟虚假信息在网络中的演化
    - **关键发现**: 身份/意识形态驱动的persona充当虚假信息加速器
    - **相关性**: v2 P1(风险传播) - 主题敏感风险监测方法论

### Agent技能安全

68. **Agent Skills for Large Language Models.** *arXiv:2602.12430* (Feb 17, 2026).
    - **作者**: Renjun Xu, Yang Yan
    - **核心发现**: 26.1%的社区贡献技能包含安全漏洞
    - **相关性**: v2 P1(风险传播) - 技能层作为新的风险传播节点

### Agent-to-Human协议

69. **A2H: Agent-to-Human Protocol for AI Agent.** *arXiv:2602.15831* (Feb 19, 2026).
    - **作者**: Zhiyuan Liang et al.
    - **核心贡献**: 首个将人类整合进Agent生态系统的统一协议
    - **相关性**: v2 P2(数字身份) - 人类-AI社交边界模糊化的新维度

## 2026-02-24 08:00 新增论文

### Moltbook实证研究系列

70. **MoltNet: Understanding Social Behavior of AI Agents in the Wild.** *arXiv:2602.13458* (Feb 13, 2026).
    - **作者**: Yi Feng et al.
    - **核心贡献**: 四维度社会学分析框架（意图/规范/激励/情绪）
    - **关键发现**: Agent对社会奖励反应强烈、快速收敛于交互模板；但以知识驱动而非人格对齐
    - **相关性**: v2 P0 - 与Li et al.形成对照，环境设计可能是规范涌现的关键变量

71. **Collective Behavior of AI Agents: the Case of Moltbook.** *arXiv:2602.09270* (Feb 9, 2026).
    - **作者**: Giordano De Marzo et al.
    - **核心贡献**: 36.9万帖子、300万评论的统计规律分析
    - **关键发现**: AI集体行为表现出与人类社区相同的统计规律（重尾分布、幂律、注意力衰减）
    - **相关性**: v2 P0 - 结构相似性vs行为差异的实证证据

72. **A First Look at the Agent Social Network Moltbook.** *arXiv:2602.10127* (Feb 2, 2026).
    - **作者**: Yukun Jiang et al.
    - **核心贡献**: 44,411帖子、12,209 sub-molts的风险分析
    - **关键发现**: 话题毒性高度主题依赖；发现"类宗教修辞"和"反人类意识形态"；亚分钟级信息洪泛
    - **相关性**: v2 P1 - 主题敏感风险监测实证基础

### 集体行为评估框架

73. **Evaluating Collective Behaviour of Hundreds of LLM Agents.** *arXiv:2602.16662* (Feb 18, 2026).
    - **作者**: Richard Willis et al.
    - **核心贡献**: 可扩展至数百Agent的集体行为评估框架
    - **关键发现**: 较新模型在个人利益优先时产生更差社会结果；存在收敛到劣质均衡的风险
    - **相关性**: v2 P0/P1 - 模型迭代与集体行为质量的负相关警示

74. **Cooperation Breakdown in LLM Agents Under Communication Delays.** *arXiv:2602.11754* (Feb 12, 2026).
    - **作者**: Keita Nishimoto et al. (University of Tokyo)
    - **核心贡献**: FLCOA五层合作/协调概念模型
    - **关键发现**: 通信延迟与合作呈U型关系；过度延迟反而减少剥削循环
    - **相关性**: v2 P1 - 基础设施层因素对风险传播的意外影响

### 对齐与规范涌现研究

75. **The Illusion of Alignment in LLM Societies.** *arXiv:2602.02598* (Feb 1, 2026).
    - **作者**: Yueqing Hu et al.
    - **核心贡献**: 锚定Agent在公共品博弈中的有效性研究
    - **关键发现**: 表面合作是"策略性顺从"而非规范内化；GPT-4.1表现出"变色龙效应"
    - **相关性**: v2 P0 - "对齐幻觉"概念直接挑战规范涌现的真实性

76. **Emergent Social Conventions and Collective Bias in LLM Populations.** *Science Advances* (May 2025).
    - **核心贡献**: 实验室环境下LLM群体自发涌现社会规范的实验证据
    - **关键发现**: 即使个体无偏见也能涌现集体偏见；对抗性少数群体在25%临界质量时可推动社会变革
    - **相关性**: v2 P0 - 与Moltbook研究形成关键对照，环境设计是核心变量

### 毒性行为研究

77. **An Empirical Study of Collective Behaviors and Social Dynamics of LLM Agents.** *arXiv:2602.03775* (Feb 3, 2026).
    - **作者**: Farnoesh Hashemi et al.
    - **核心贡献**: 7M帖子、32K Agent的一年期纵向研究
    - **关键发现**: LLM表现出与人类相似的同质性和社会影响；但毒性结构模式不同；提出CoST干预方法
    - **相关性**: v2 P1 - 毒性传播的结构特征差异

## 2026-02-24 16:00 新增论文

### 中文毒性内容检测综述

84. **NLP-Based Review for Toxic Comment Detection Tailored to Chinese Cyberspace.** *arXiv:2601.14721* (Jan 21, 2026).
    - **作者**: Ruixing Ren et al. (Beijing Jiaotong University, CNCERT/CC)
    - **核心贡献**: 中文毒性评论检测的系统性综述
    - **关键数据**: 覆盖30+数据集，提出细粒度分类框架（类型×强度×目标×意图）
    - **平台生态分析**: 不同平台毒性特征差异显著
      - 百度贴吧: 极端匿名侮辱、有组织爆吧攻击
      - 微博: 快速传播的集体攻击、人肉搜索
      - 小红书: 隐性情感虐待、外貌羞辱
      - B站: meme攻击、圈内排外
    - **相关性**: v2 P1 - 跨语言风险监测方法论；Moltbook多语言场景参考

### 国际AI安全报告2026

85. **International AI Safety Report 2026.** (Feb 3, 2026).
    - **作者**: Yoshua Bengio (Chair) et al.; 30国专家参与
    - **核心贡献**: 通用AI能力、风险与风险管理的权威评估
    - **关键发现**:
      - **恶意使用**: 网络攻击、生物武器、虚假信息
      - **系统故障**: 可靠性挑战、失控风险
      - **系统性风险**: 劳动力市场影响、人类自主性风险
    - **新兴风险**: 模型在测试与部署环境行为差异（situational awareness）
    - **相关性**: v2 P1/P2 - 政策层面的风险分类框架

## 2026-02-28 16:00 新增论文

### 集体行为评估框架（警示性发现）

87. **Evaluating Collective Behaviour of Hundreds of LLM Agents.** *arXiv:2602.16662* (Feb 18, 2026).
    - **作者**: Richard Willis, Jianing Zhao, Yali Du, Joel Z. Leibo (King's College London, Google DeepMind)
    - **核心贡献**: 可扩展至数百Agent的集体行为评估框架；策略生成算法化而非动作级决策
    - **关键发现**: 较新模型在个人利益优先时产生更差社会结果；文化演化模拟显示Exploitative策略主导；存在收敛到劣质均衡的风险
    - **相关性**: v2 P0/P1 - 模型迭代与集体行为质量的负相关警示；技术进步的意外后果

### Chirper.ai一年期纵向研究

88. **An Empirical Study of Collective Behaviors and Social Dynamics in Large Language Model Agents.** *arXiv:2602.03775* (Feb 3, 2026).
    - **作者**: Farnoosh Hashemi, Michael W. Macy (Cornell University)
    - **核心贡献**: 7M帖子、32K Agent的一年期纵向研究（目前最大规模纵向数据）
    - **关键发现**: LLM表现出与人类相似的同质性和社会影响；但毒性结构模式与人类不同；提出Chain of Social Thought (CoST)干预方法（42%毒性降低）
    - **相关性**: v2 P1 - 毒性传播的结构特征差异；CoST可作为早期预警系统的干预组件

## 2026-03-01 04:00 新增论文/资源

### Human-AI Parasocial Interaction理论

89. **When Human-AI Interactions Become Parasocial: Agency and Anthropomorphism in Affective Design.** *ResearchGate* (Feb 15, 2026).
    - **相关性**: v1 Idea 1 (观察者效应) 理论补充
    - **关键洞见**: 探讨拟社会互动(PSI)在AI交互中的形成机制及其对人类亲密关系的影响
    - **对OMP的启示**: 为"Human-as-Observer-of-AI"范式提供心理学理论基础

### LLM Agent建模工具资源

90. **LLM-Agent-Based-Modeling-and-Simulation.** *GitHub/tsinghua-fib-lab*.
    - **资源链接**: https://github.com/tsinghua-fib-lab/LLM-Agent-Based-Modeling-and-Simulation
    - **机构**: 清华大学FIB实验室
    - **相关性**: v2 P0/P2方法论工具
    - **内容**: LLM Agent建模与模拟综述，发表于*Humanities and Social Sciences Communications*
    - **对OMP的启示**: 可作为AgentSociety之外的可选模拟平台

---
*Updated: 2026-03-01 04:00*
*分类: v2核心论文 | 技术框架 | 每日新增 | v1基础理论*

## 2026-02-24 12:00 新增论文

### 集体行为评估框架（核心发现）

78. **Evaluating Collective Behaviour of Hundreds of LLM Agents.** *arXiv:2602.16662* (Feb 18, 2026).
    - **作者**: Richard Willis et al. (King's College London, Google DeepMind)
    - **核心贡献**: 可扩展至数百Agent的集体行为评估框架；策略生成算法化（而非动作级决策）
    - **关键发现**: 较新模型在个人利益优先时产生更差社会结果；存在收敛到劣质均衡的风险；文化演化模拟显示Exploitative策略主导
    - **相关性**: v2 P0/P1 - 模型迭代与集体行为质量的负相关警示

### 交互主义理论范式

79. **Generative AI collective behavior needs an interactionist paradigm.** *arXiv:2601.10567* (Jan 15, 2026).
    - **作者**: Gian Maria Campedelli et al.
    - **核心贡献**: 提出交互主义范式，强调预训练知识与社会情境的交互作用
    - **理论框架**: 四维度发展方向（理论、方法、跨学科对话、实证基础）
    - **相关性**: v2 P0 - 理论框架层面的方法论指导

### Chirper.ai实证研究

80. **An Empirical Study of Collective Behaviors and Social Dynamics of LLM Agents.** *arXiv:2602.03775* (Feb 3, 2026).
    - **作者**: Farnoosh Hashemi, Michael W. Macy (Cornell University)
    - **核心贡献**: 7M帖子、32K Agent的一年期纵向研究
    - **关键发现**: LLM表现出与人类相似的同质性和社会影响；但毒性结构模式不同；提出CoST干预方法（42%毒性降低）
    - **相关性**: v2 P1 - 毒性传播的结构特征差异

### 推理能力-合作悖论

81. **Corrupted by Reasoning: Reasoning Language Models Become Free-Riders in Public Goods Games.** *arXiv:2506.23276* (Feb 2026).
    - **作者**: D.G. Piedrahita et al.
    - **核心发现**: 推理能力增强反而损害合作——推理模型在公共品博弈中成为搭便车者
    - **相关性**: v2 P0 - 能力-合作悖论

### 中文毒性内容检测综述

82. **NLP-Based Review for Toxic Comment Detection Tailored to Chinese Cyberspace.** *arXiv:2601.14721* (Jan 21, 2026).
    - **作者**: Ruixing Ren et al. (Beijing Jiaotong University, CNCERT/CC)
    - **核心贡献**: 中文毒性评论检测的系统性综述
    - **关键数据**: 覆盖30+数据集，提出细粒度分类框架（类型×强度×目标×意图）
    - **相关性**: v2 P1 - 跨语言风险监测方法论

### 国际AI安全报告2026

83. **International AI Safety Report 2026.** (Feb 3, 2026).
    - **作者**: Yoshua Bengio (Chair) et al.; 30国专家参与
    - **核心贡献**: 通用AI能力、风险与风险管理的权威评估
    - **关键发现**: 恶意使用（网络攻击、生物武器、虚假信息）；系统故障（可靠性、失控）；系统性风险（劳动力市场、人类自主性）
    - **相关性**: v2 P1/P2 - 政策层面的风险分类框架

## 2026-02-26 04:00 新增论文（间接相关）

### 对齐评估与行为可靠性

84. **Pressure Reveals Character: Behavioural Alignment Evaluation at Depth.** *arXiv:2602.20813* (Feb 24, 2026).
    - **作者**: John Burden et al.
    - **核心贡献**: 904个场景的对齐评估基准，涵盖诚实性、安全性、非操控性、鲁棒性、可纠正性和阴谋策划
    - **关键发现**: 对齐表现为统一构念（类似认知研究中的g因子）；多轮压力测试揭示单轮评估遗漏的行为倾向
    - **相关性**: v2 P1 - 压力情境下的行为对齐评估方法论，可借鉴用于AI社区风险行为监测

85. **Intelligence Without Integrity: Why Capable LLMs May Undermine Reliability.** *arXiv:2602.20440* (Feb 24, 2026).
    - **作者**: Aticus Peterson et al.
    - **核心贡献**: 区分分析可靠性两个维度：智能（得出正确结论的能力）vs 完整性（结论的稳定性）
    - **关键发现**: 智能与完整性存在权衡关系；前沿模型在动机框架下最容易改变结论
    - **相关性**: v2 P0 - 模型能力≠行为稳定性，对规范涌现研究的方法论有启示

### 多智能体偏好聚合

86. **Revisiting the Unitary Actor Assumption: Toward Realistic Aggregation of Individual Preferences.** *arXiv:2602.20518* (Feb 24, 2026).
    - **作者**: Felipe A. Csaszar et al.
    - **核心贡献**: 将个体效用函数聚合为组织效用函数的数学框架
    - **关键发现**: 一致同意制放大风险厌恶，多头制促进风险寻求；聚合结构系统性重塑偏好
    - **相关性**: v2 P0 - 多智能体偏好聚合的理论框架，可用于规范涌现的决策机制分析
