# 02-产品研究

## 职责

对明确 Candidate Product 进行正式评估。

## 流程

```text
Candidate Product
       ↓
读取业务上下文
       ↓
调用 product-research
       ↓
Product Research Result
       ↓
Business Decision
```

本区只定义：

- 什么时候调用 `product-research`
- 输入哪些业务上下文
- 研究结果保存在哪里
- 与前后业务阶段如何衔接

不重新定义 Evidence、Gate、Unit Economics、Scoring、Market Demand、
Competition、VOC、GO / NO-GO 方法论，这些全部由 `product-research` 提供。

## 产出位置

- 研究结果：`workspace/products/<product-slug>/research/`
- 业务决策：`workspace/products/<product-slug>/decision.md`

具体产品的研究结果不得写入 `.claude/skills/product-research/`（该目录指向独立项目）。
