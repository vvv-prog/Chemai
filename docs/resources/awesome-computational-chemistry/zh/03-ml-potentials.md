# 03 · 机器学习势函数 / 原子尺度机器学习

> **🌐 语言:** <kbd>[English](../03-ml-potentials.md)</kbd> <kbd>[**中文**](03-ml-potentials.md)</kbd>

[← 返回首页](../README.zh.md)

用机器学习拟合势能面（MLIP / NNP），以**接近 DFT 的精度、接近经典力场的速度**，
进行大体系、长时间尺度的分子动力学与材料模拟。近年大量出现**通用预训练势（基础模型）**，可直接使用或微调。

> 🔄 **更新情况** 截至 **2026 年 6 月**。活跃度：🟢 高度活跃 ｜ 🟡 稳定维护 ｜ 🟠 缓慢更新。

---

## DeePMD-kit

- **官网**：https://docs.deepmodeling.com/projects/deepmd
- **代码仓库**：https://github.com/deepmodeling/deepmd-kit ｜ [Releases](https://github.com/deepmodeling/deepmd-kit/releases)
- **语言 / 许可**：Python + C++ / LGPL-3.0
- **🎯 使用方向**：Deep Potential（深度势能）模型的**训练与部署**，与 LAMMPS、GROMACS、ASE 等无缝对接，
  适合材料/液体/催化等大体系的高精度 MD。提供 **DPA 系列通用预训练大模型**。
- **🔄 更新情况**：🟢 **v3.1.x** 系列；新增内置可直接下载的预训练模型（如 **DPA3**）、分布式训练与更多优化器。开发非常活跃（DeepModeling 社区）。

## MACE

- **代码仓库**：https://github.com/ACEsuit/mace ｜ [Releases](https://github.com/ACEsuit/mace/releases)
- **语言 / 许可**：Python / MIT
- **🎯 使用方向**：基于**高阶等变消息传递**的 MLIP，精度与效率领先，是当前最受欢迎的等变 GNN 势之一。
  提供覆盖周期表的**通用基础模型** [mace-foundations](https://github.com/ACEsuit/mace-foundations)（如 MACE-MP、MACE-OFF、MACE-MH），可直接用于材料/分子/表面体系。
- **🔄 更新情况**：🟢 高度活跃，基础模型与代码持续迭代。

## NequIP / Allegro

- **代码仓库**：https://github.com/mir-group/nequip ｜ [Allegro](https://github.com/mir-group/allegro)
- **语言 / 许可**：Python / MIT
- **🎯 使用方向**：**E(3) 等变图神经网络**势，以**数据高效**著称——少量 DFT 数据即可获得高精度；
  Allegro 为其**严格局域、可扩展**的变体，适合超大体系并行。
- **🔄 更新情况**：🟢 活跃维护（近期仍有更新）。

## MatGL（Materials Graph Library）

- **官网**：https://matgl.ai
- **代码仓库**：https://github.com/materialsvirtuallab/matgl ｜ [Releases](https://github.com/materialsvirtuallab/matgl/releases)
- **语言 / 许可**：Python / BSD-3
- **🎯 使用方向**：材料图神经网络库，集成 **M3GNet、CHGNet、MEGNet、TensorNet、SO3Net** 等架构，
  含**通用势（FMM）与性质预测**预训练模型，开箱即用、可微调。与 pymatgen/ASE 紧密集成。
- **🔄 更新情况**：🟢 最新 **v4.0.2**（2026-06-10）。默认采用 PyG 后端、含 QET 架构;发布频繁。
- **🔗 模型说明**：**CHGNet** 引入电荷/磁矩信息；**M3GNet** 含三体相互作用；适合无机晶体材料。

## fairchem（FAIR Chemistry）

- **代码仓库**：https://github.com/facebookresearch/fairchem ｜ [Releases](https://github.com/facebookresearch/fairchem/releases)
- **语言 / 许可**：Python / MIT（部分模型权重另有许可）
- **🎯 使用方向**：Meta FAIR 的化学机器学习库，源自 **Open Catalyst** 项目，
  提供**催化/材料的通用大模型（如 UMA）**与大规模数据集（OC20/OC22 等），面向催化剂筛选与材料发现。
- **🔄 更新情况**：🟢 高度活跃（2026-06 仍有更新）。

## TorchANI

- **代码仓库**：https://github.com/aiqm/torchani ｜ [Releases](https://github.com/aiqm/torchani/releases)
- **语言 / 许可**：Python / MIT
- **🎯 使用方向**：**ANI 系列**神经网络势（侧重有机分子，含 ANI-1x/ANI-2x 预训练模型），
  PyTorch 实现、易上手，适合有机/药物分子的快速势能与力计算。
- **🔄 更新情况**：🟡 稳定维护（2025 仍有更新）。

## SchNetPack

- **代码仓库**：https://github.com/atomistic-machine-learning/schnetpack ｜ [Releases](https://github.com/atomistic-machine-learning/schnetpack/releases)
- **语言 / 许可**：Python / MIT
- **🎯 使用方向**：原子神经网络**建模工具箱**（SchNet、PaiNN 等），含数据管线与内置 MD，
  适合方法学习、研究与自定义模型开发。
- **🔄 更新情况**：🟡 SchNetPack **2.0** 系列，稳定维护。

## sGDML

- **官网**：http://www.sgdml.org
- **代码仓库**：https://github.com/stefanch/sGDML ｜ [Releases](https://github.com/stefanch/sGDML/releases)
- **语言 / 许可**：Python / MIT
- **🎯 使用方向**：**对称梯度域机器学习**（核方法），对单个小分子可用极少数据重构**高精度势能面**，
  适合精确动力学/光谱研究（不追求跨体系通用性）。
- **🔄 更新情况**：🟠 偶尔更新。

---

## 扩展资源

- 📊 [best-of-atomistic-machine-learning](https://github.com/JuDFTteam/best-of-atomistic-machine-learning)：
  按热度排名的原子尺度机器学习项目大全，持续更新，可作为本节的延伸目录。
- 相关：[GAP/SOAP](https://github.com/libAtoms/GAP)、[n2p2](https://github.com/CompPhysVienna/n2p2)、
  [Nequip/Allegro 生态]、[matsciml] 等。

[← 上一类：分子动力学](02-molecular-dynamics.md) ｜ [返回首页](../README.zh.md) ｜ [下一类：材料高通量工作流 →](04-materials-workflows.md)
