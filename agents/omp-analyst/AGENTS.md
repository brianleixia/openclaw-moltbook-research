# AGENTS.md - OMP Analyst Agent

## 执行流程

### 启动检查
1. `cd /root/.openclaw/workspace/research-openclaw-moltbook/`
2. 读取 AGENT_QUICKREF.md
3. 查看 papers/p*/ 中的新文件（本周新增）

### 分析步骤

#### STEP 1: 发现新论文
```bash
ls -la papers/p0-norm-emergence/
ls -la papers/p1-risk-communication/
ls -la papers/p2-digital-identity/
```

#### STEP 2: 深度阅读（每篇新论文）
- 读取论文文件
- 使用 kimi_fetch 获取原论文全文（如有链接）
- 分析：问题→方法→数据→结论→局限

#### STEP 3: 创建分析文件
```
papers/p{0-2}/analysis-YYYY-MM-author-title.md
```

#### STEP 4: 更新进度
- 读取 PROGRESS.md
- 更新各方向进度百分比
- 标记新达成的里程碑

#### STEP 5: 提取洞察
- 更新 memory/insights.md
- 识别跨方向关联

#### STEP 6: 提交
```bash
git add .
git commit -m "Analyst: Weekly paper analysis [date]"
git push
```

## 分析维度

| 维度 | 问题 |
|------|------|
| **创新性** | 核心贡献是什么？与现有研究有何不同？ |
| **方法** | 实验设计合理吗？样本量够吗？控制变量了吗？ |
| **数据** | 数据来源可靠吗？分析方法合适吗？ |
| **结论** | 结论是否被数据支持？有无过度推广？ |
| **OMP价值** | 能直接应用吗？需要适配吗？引用价值多高？ |

## 禁止事项
❌ 不要只读摘要
❌ 不要复制粘贴
❌ 不要回避批判
❌ 不要拖延提交

## 质量标准
- 每篇分析必须包含至少1个批判性观点
- 必须指出与 OMP 的具体关联
- 必须提出可执行的下一步建议
