# 05 · 化学信息学

[← 返回首页](../README.md)

分子的表示、读写与格式转换、描述符/指纹生成、子结构匹配、构象生成，
以及面向机器学习的化学特征工程。

> 🔄 **更新情况** 截至 **2026 年 6 月**。活跃度：🟢 高度活跃 ｜ 🟡 稳定维护 ｜ 🟠 缓慢更新。

---

## RDKit

- **官网**：https://www.rdkit.org
- **代码仓库**：https://github.com/rdkit/rdkit ｜ [Releases](https://github.com/rdkit/rdkit/releases)
- **语言 / 许可**：C++ + Python / BSD-3
- **🎯 使用方向**：化学信息学的**事实标准库**。功能涵盖：分子读写（SMILES/SMARTS/Mol/SDF）、
  **指纹与描述符**（Morgan/ECFP、MACCS、物化性质）、子结构搜索、**构象生成（ETKDG）**、
  分子对齐、反应处理、相似性计算，以及为 QSAR/机器学习准备特征。
- **✨ 主要特性**：成熟稳定、文档完善，是几乎所有药物发现/化学 ML 流程的基础依赖；可与 Pandas（PandasTools）联用。
- **🔄 更新情况**：🟢 最新 **2026.03.3**（2026-06-05）。每季度发布（YYYY.MM.patch），维护非常活跃。

## Open Babel

- **官网**：https://openbabel.org
- **代码仓库**：https://github.com/openbabel/openbabel ｜ [Releases](https://github.com/openbabel/openbabel/releases)
- **语言 / 许可**：C++ / GPL-2.0
- **🎯 使用方向**：化学**文件格式转换**与互操作的瑞士军刀，支持 **110+ 种格式**互转
  （如 PDB↔PDBQT↔MOL2↔SMILES），并提供加氢、生成 3D 坐标、简单力场优化等命令行/库功能；
  在对接前的配体准备中很常用。
- **🔄 更新情况**：🟠 稳定但更新缓慢，主版本 **3.1.1**（2020），主要做小修维护。

## DeepChem

- **官网**：https://deepchem.io
- **代码仓库**：https://github.com/deepchem/deepchem ｜ [Releases](https://github.com/deepchem/deepchem/releases)
- **语言 / 许可**：Python / MIT
- **🎯 使用方向**：面向**药物发现、材料、量子化学与生物**的深度学习工具箱，提供大量内置数据集
  （MoleculeNet）、特征化方法、模型基线（图神经网络、序列模型等）与端到端示例，
  适合快速搭建化学/生命科学的机器学习基线。
- **🔄 更新情况**：🟢 活跃维护，持续扩展模型与数据支持。

---

## 同方向值得了解

| 项目 | 说明 |
|------|------|
| [Chemprop](https://github.com/chemprop/chemprop) | 基于消息传递神经网络（D-MPNN）的分子性质预测，工业界常用 |
| [datamol](https://github.com/datamol-io/datamol) | 基于 RDKit 的高层易用封装，简化常见化学信息学操作 |
| [scikit-mol](https://github.com/EBjerrum/scikit-mol) | 将 RDKit 特征化接入 scikit-learn 管线 |
| [Indigo](https://github.com/epam/Indigo) | 另一套化学信息学工具与渲染库（EPAM） |

[← 上一类：材料高通量工作流](04-materials-workflows.md) ｜ [返回首页](../README.md) ｜ [下一类：分子对接与药物设计 →](06-docking-drug-design.md)
