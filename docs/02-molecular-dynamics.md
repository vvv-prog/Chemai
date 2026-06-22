# 02 · 分子动力学模拟

> 🌐 **中文** ｜ [English](en/02-molecular-dynamics.md)

[← 返回首页](../README.md)

经典/增强采样分子动力学（MD），用于生物大分子、软物质、材料体系的动力学行为、
热力学性质与自由能计算。

> 🔄 **更新情况** 截至 **2026 年 6 月**。活跃度：🟢 高度活跃 ｜ 🟡 稳定维护 ｜ 🟠 缓慢更新。

---

## GROMACS

- **官网**：https://www.gromacs.org
- **代码仓库**：https://github.com/gromacs/gromacs ｜ [Releases](https://manual.gromacs.org/current/download.html)
- **语言 / 许可**：C++ / LGPL-2.1
- **🎯 使用方向**：生物分子 MD 的主力引擎，**速度极快、GPU 优化优秀**，
  广泛用于蛋白质、核酸、膜体系的模拟与**自由能微扰（FEP）**计算。
- **✨ 主要特性**：高度优化的内核、成熟的分析工具链、丰富的力场支持；
  2026 版新增 AMBER14SB/19SB 蛋白力场、OPC/OPC3 水模型，并扩展了对**神经网络势（NNP）**的支持。
- **🔄 更新情况**：🟢 最新 **2026.2**（2026 系列，2026.0 于 2026-01-19 发布）。年度大版本 + 季度修订。

## LAMMPS

- **官网**：https://www.lammps.org
- **代码仓库**：https://github.com/lammps/lammps ｜ [Releases](https://github.com/lammps/lammps/releases)
- **语言 / 许可**：C++ / GPL-2.0
- **🎯 使用方向**：材料与软物质的**大规模并行 MD**，力场/势函数种类极其丰富（金属、聚合物、
  颗粒、反应力场 ReaxFF、机器学习势等），可扩展性与定制能力极强。
- **✨ 主要特性**：模块化 package 体系，易接入 DeePMD/MACE 等 ML 势；命令脚本驱动；
  附带 LAMMPS-GUI。
- **🔄 更新情况**：🟢 稳定版 **22Jul2025**（update4），开发/特性版 **30Mar2026**。持续高频更新。

## OpenMM

- **官网**：https://openmm.org
- **代码仓库**：https://github.com/openmm/openmm ｜ [Releases](https://github.com/openmm/openmm/releases)
- **语言 / 许可**：C++ + Python / MIT、LGPL
- **🎯 使用方向**：GPU 加速的 MD **工具箱/库**，Python API 极其灵活，
  适合自定义力场、自定义积分器，以及把**机器学习势嵌入 MD**（[openmm-ml](https://github.com/openmm/openmm-ml)）。
  常作为其他工作流（如 OpenFF、folding 流程）的底层引擎。
- **🔄 更新情况**：🟢 最新 **v8.5.2**（2026-06-08）。活跃发布，支持新 Python 版本。

## HOOMD-blue

- **官网**：https://hoomd-blue.readthedocs.io
- **代码仓库**：https://github.com/glotzerlab/hoomd-blue ｜ [Releases](https://github.com/glotzerlab/hoomd-blue/releases)
- **语言 / 许可**：C++ + Python / BSD-3
- **🎯 使用方向**：面向 GPU 的**粗粒化/胶体/自组装**模拟，支持分子动力学与蒙特卡洛（HPMC），
  Python 脚本驱动，软物质与纳米粒子自组装研究常用。
- **🔄 更新情况**：🟢 最新 **v7.0.x**（2026-04）。活跃发布。

## ESPResSo

- **官网**：https://espressomd.org
- **代码仓库**：https://github.com/espressomd/espresso ｜ [Releases](https://github.com/espressomd/espresso/releases)
- **语言 / 许可**：C++ + Python / GPL-3.0
- **🎯 使用方向**：**软物质与复杂流体**（聚电解质、带电胶体、表面活性剂），
  支持与格子玻尔兹曼流体力学耦合、静电长程算法（P3M）等。
- **🔄 更新情况**：🟡 稳定维护，定期发布。

## AmberTools

- **官网**：https://ambermd.org/AmberTools.php
- **代码仓库**：https://github.com/Amber-MD ｜ 下载见官网
- **语言 / 许可**：C/C++/Python / GPL 及其他（**开源部分**）
- **🎯 使用方向**：Amber 力场生态的**免费开源**组件——体系建模（tleap）、力场参数化（antechamber/GAFF）、
  **MM-PBSA/GBSA 结合自由能**、轨迹分析（cpptraj/pytraj）。可配合 OpenMM/GROMACS 等使用。
- **🔄 更新情况**：🟡 年度发布（如 AmberTools 25）。注意：主程序（pmemd 等加速版）**需付费许可**，AmberTools 本身开源。

---

## 同方向值得了解（部分非开源）

| 项目 | 说明 |
|------|------|
| [NAMD](https://www.ks.uiuc.edu/Research/namd/) | 大体系并行 MD，**免费但非完全开源**；与 VMD 配套良好 |
| [OpenFF Toolkit](https://github.com/openforcefield/openff-toolkit) | 开源小分子力场（SMIRNOFF）参数化工具 |
| Amber（pmemd）/ Desmond | 商业/付费许可，不在本开源列表范围 |

[← 上一类：量子化学](01-quantum-chemistry.md) ｜ [返回首页](../README.md) ｜ [下一类：机器学习势函数 →](03-ml-potentials.md)
