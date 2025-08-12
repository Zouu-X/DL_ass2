# Deep Learning Assignment 2

本项目聚焦于利用深度学习技术对分子数据进行分析与生成，主要包含以下任务：

1. **基于 SMILES 的能量预测**：使用字符级嵌入与 LSTM 模型，根据分子的 SMILES 表示预测形成能。
2. **基于几何信息的能量预测**：采用 SchNet 模型，从原子坐标和类型出发预测形成能。
3. **分子生成**：构建 LSTM 自回归模型生成 SMILES，并评估其有效性、唯一性和新颖性。

## 目录结构

```
ass2_data/            # 原始数据：坐标、原子类型、SMILES、形成能等
clean_data/           # 清洗后的坐标与原子类型数据
models/               # 训练好的模型权重
ass2_skeleton.ipynb   # 完整的实验流程与示例代码
Deep_learning_assignment_2.pdf  # 作业背景与说明
```

## 环境依赖

- Python 3.10+
- PyTorch
- torch-geometric
- RDKit

建议使用 `conda` 创建环境，并安装所需依赖。

## 快速开始

1. 运行 `ass2_skeleton.ipynb`，按照 notebook 中的步骤加载数据、训练模型并评估生成结果。
2. 根据需要，可将 notebook 中的核心模块抽取为脚本或库，便于复用与扩展。

## 进一步学习建议

- 阅读代码中对数据处理、模型训练流程的注释，加深对 PyTorch 与图神经网络的理解。
- 尝试替换或扩展现有模型（如使用 Transformer 或其他 GNN 结构）。
- 编写单元测试和可视化工具，以提高工程质量。

