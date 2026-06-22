# 06 · 分子对接与药物设计

[← 返回首页](../README.md)

预测小分子配体与蛋白靶点的结合构象（pose）与结合亲和力，用于**虚拟筛选**与先导化合物发现。

> 🔄 **更新情况** 截至 **2026 年 6 月**。活跃度：🟢 高度活跃 ｜ 🟡 稳定维护 ｜ 🟠 缓慢更新。

---

## AutoDock Vina

- **官网**：https://vina.scripps.edu
- **代码仓库**：https://github.com/ccsb-scripps/AutoDock-Vina ｜ [Releases](https://github.com/ccsb-scripps/AutoDock-Vina/releases)
- **语言 / 许可**：C++ + Python / Apache-2.0
- **🎯 使用方向**：**最流行的开源分子对接引擎**，速度快、易用，提供 Python 绑定与命令行；
  适合常规对接与中等规模虚拟筛选。支持 Vina、Vinardo 等评分函数。
- **🔄 更新情况**：🟡 最新 **v1.2.7**，稳定维护（由 Scripps Forli 实验室开发）。

## AutoDock-GPU

- **代码仓库**：https://github.com/ccsb-scripps/AutoDock-GPU ｜ [Releases](https://github.com/ccsb-scripps/AutoDock-GPU/releases)
- **语言 / 许可**：C/C++（OpenCL/CUDA） / GPL-2.0
- **🎯 使用方向**：AutoDock4 评分（拉马克遗传算法）的 **GPU/OpenCL/CUDA 加速版**，
  在大规模虚拟筛选中相比 CPU 有数量级加速，适合超大化合物库的高通量对接。
- **🔄 更新情况**：🟡 稳定维护（Scripps Forli 实验室）。

## smina

- **代码仓库**：https://github.com/mwojcikowski/smina ｜ [Releases](https://github.com/mwojcikowski/smina/releases)
- **语言 / 许可**：C++ / Apache、GPL
- **🎯 使用方向**：AutoDock Vina 的分支，**便于自定义评分函数、灵活的能量最小化与打分**，
  在虚拟筛选脚本化中很受欢迎（输入处理更友好）。
- **🔄 更新情况**：🟠 偶尔更新（功能稳定）。

## gnina

- **代码仓库**：https://github.com/gnina/gnina ｜ [Releases](https://github.com/gnina/gnina/releases)
- **语言 / 许可**：C++ / Apache-2.0
- **🎯 使用方向**：在 smina 基础上集成**卷积神经网络（CNN）打分**的对接工具，
  用深度学习对结合 pose 进行评分与重排序，通常能改善打分/排序质量；适合需要 ML 增强的对接与虚拟筛选。
- **🔄 更新情况**：🟢 最新 **v1.3.2**（2025-07-08）。v1.3 将底层深度学习框架迁移到 **PyTorch**，
  并在 CrossDocked2020 v1.3 上重训 CNN 打分、引入知识蒸馏以加速高通量筛选。活跃维护。

---

## 同方向值得了解

| 项目 | 说明 |
|------|------|
| [Meeko](https://github.com/forlilab/Meeko) | Vina/AutoDock 的配体/受体准备工具（PDBQT 生成），Forli 实验室出品 |
| [DiffDock](https://github.com/gcorso/DiffDock) | 基于扩散模型的深度学习对接（盲对接），研究热点 |
| [DOCK 6](https://dock.compbio.ucsf.edu/) | UCSF 经典对接程序，学术许可 |
| [OpenFE](https://github.com/OpenFreeEnergy/openfe) | 开源相对/绝对结合自由能（FEP）计算框架 |

> 提示：对接前的配体准备常用 **Open Babel**（[见化学信息学](05-cheminformatics.md)）或 Meeko 完成 PDBQT 转换。

[← 上一类：化学信息学](05-cheminformatics.md) ｜ [返回首页](../README.md) ｜ [下一类：轨迹分析与可视化 →](07-visualization-analysis.md)
