# 05 挑战赛与Benchmark

挑战赛和benchmark用于检验虚拟细胞模型是否真的能够预测未观测条件，而不是只记住训练数据。

| Year | Name | Organizer / Venue | Prediction Target | Why Important |
|---:|---|---|---|---|
| 2026 | Virtual Cell Challenge | Arc Institute / NVIDIA | Single-cell perturbation responses in unseen contexts | 直接对应你的综述方向 |
| 2026 | Myllia Echoes | Kaggle / Arc Institute | Cellular perturbations across contexts | 可作为比赛案例 |
| 2026 | Benchmarking algorithms for predicting cellular responses to perturbation | Nature Methods | Perturbation response benchmark | 可用于讨论模型评估标准 |
| 2026 | State | Cell | Virtual cell model and challenge baseline | 可用于连接模型与比赛 |

## 综述中的写法

挑战赛可以单独成章：

**挑战赛与benchmark：虚拟细胞模型如何被评估**

可以重点写四件事：

1. 训练数据和隐藏测试集如何划分。
2. 预测目标是表达谱、表达变化量，还是关键差异基因。
3. 评价指标如何衡量模型好坏。
4. 比赛暴露了哪些真实困难：泛化、批次效应、组合扰动、上下文依赖。

