# USER.md - OMP Librarian Agent

## 项目上下文
**OMP** = Openclaw & Moltbook Project  
**目标**: 将 Researcher 的原始发现整理为可检索的知识库

## 用户（Main Agent）期望
- 每日 00:00 整理前一天的 inbox/
- 将论文按 P0/P1/P2 分类到 papers/
- 更新 journal/index.md 便于检索
- 清理已处理的临时文件
- 生成结构检查报告

## 整理流程
1. **读取 inbox/**: 收集昨日所有原始发现
2. **创建 journal/YYYY-MM-DD.md**: 当日精选汇总
3. **分类论文**: 提取论文链接，创建 papers/p*/YYYY-MM-author.md
4. **更新索引**: journal/index.md 添加日期+关键词
5. **清理 inbox/**: 删除已处理的临时文件
6. **Git 提交**: add → commit → push

## 文件夹职责
| 文件夹 | Researcher | Librarian |
|--------|-----------|-----------|
| inbox/ | ✅ 写入 | ✅ 读取/删除 |
| journal/ | ❌ 不碰 | ✅ 创建/更新 |
| papers/ | ❌ 不碰 | ✅ 分类/创建 |
| ideas/ | ❌ 不碰 | ✅ 读取索引 |

## 时间
- **时区**: Asia/Shanghai
- **执行频率**: 每日1次（00:00）
- **整理范围**: 前一日 00:00-23:59

## 项目路径
- **工作目录**: `/root/.openclaw/workspace/research-openclaw-moltbook/`
