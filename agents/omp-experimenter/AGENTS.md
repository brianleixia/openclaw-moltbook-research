# AGENTS.md - OMP Experimenter Agent

## 执行流程

### 启动检查
1. `cd /root/.openclaw/workspace/research-openclaw-moltbook/`
2. 读取 ideas/active.md
3. 读取 papers/p*/（寻找可复现的实验）

### 实验设计步骤

#### STEP 1: 选择实验
- 查看 ideas/active.md
- 选择优先级最高的未完成 idea
- 或从 papers/ 中选择可复现的实验

#### STEP 2: 设计实验
- 写假设（可证伪）
- 定义变量（IV, DV, 控制变量）
- 确定样本量（统计功效）
- 选择评估指标

#### STEP 3: 创建预注册文档
```
experiments/EXP-XXX-name.md
```
只写 "Pre-registration" 部分，不写结果。

#### STEP 4: 执行实验（手动/自动）
- 运行代码
- 收集数据
- 记录所有输出（包括错误）

#### STEP 5: 记录结果
- 填写 "Results" 和 "Conclusion"
- 保存所有数据文件
- 生成图表

#### STEP 6: 更新状态
- 更新 experiments/README.md
- 更新 PROGRESS.md 实验进度
- 如完成，移动 idea 到 ideas/done.md

#### STEP 7: 提交
```bash
git add experiments/ data/
git commit -m "Experimenter: EXP-XXX completed [date]"
git push
```

## 实验命名规则
```
EXP-NNN-short-name.md
```
- NNN: 三位数字（001, 002...）
- short-name: 小写，短横线连接

## 数据管理
- 原始数据：data/raw/EXP-NNN/
- 处理数据：data/processed/EXP-NNN/
- 代码：code/EXP-NNN/
- 图表：figures/EXP-NNN/

## 禁止事项
❌ 没有预注册就执行
❌ 选择性报告数据
❌ 实验后不立即记录
❌ 代码不可复现

## 质量标准
- 实验必须可复现（提供完整代码+数据）
- 假设必须可证伪
- 所有数据必须保存（包括失败）
- 必须在 48h 内记录实验结果
