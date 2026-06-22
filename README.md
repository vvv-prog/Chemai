# Chemai — 计算化学开源项目精选 (Awesome Computational Chemistry)

> 一个持续维护的**计算化学（Computational Chemistry）开源项目**汇总列表，
> 聚焦于每个项目的**使用方向**与**更新情况**，方便研究者、学生与工程师快速选型。

本列表覆盖量子化学 / 电子结构、分子动力学、机器学习势函数、材料高通量工作流、
化学信息学、分子对接与药物设计、轨迹分析与可视化等方向。

- 📌 **使用方向**：该项目最擅长解决什么问题，典型应用场景。
- 🔄 **更新情况**：截至 **2026 年 6 月** 的最新版本 / 发布节奏 / 维护活跃度。
  版本号会随时间变化，**实时状态请以各项目的 Releases 页面为准**（表格中已附链接）。
- 🏷️ **活跃度图例**：🟢 高度活跃（近数月有发布）｜🟡 稳定维护（按年/季度发布）｜🟠 缓慢/偶尔更新。

---

## 目录

1. [量子化学与电子结构计算](#1-量子化学与电子结构计算)
2. [分子动力学模拟](#2-分子动力学模拟)
3. [机器学习势函数 / 原子尺度机器学习](#3-机器学习势函数--原子尺度机器学习)
4. [材料建模与高通量工作流](#4-材料建模与高通量工作流)
5. [化学信息学](#5-化学信息学)
6. [分子对接与药物设计](#6-分子对接与药物设计)
7. [轨迹分析与可视化](#7-轨迹分析与可视化)
8. [如何选型（速查）](#8-如何选型速查)
9. [参与贡献](#9-参与贡献)

---

## 1. 量子化学与电子结构计算

求解电子结构（HF、DFT、后 HF 等），用于分子/固体的能量、几何优化、光谱、反应路径等。

| 项目 | 语言 / 许可 | 使用方向 | 更新情况（截至 2026-06） |
|------|------------|---------|--------------------------|
| **[PySCF](https://github.com/pyscf/pyscf)** | Python/C · Apache-2.0 | Python 原生量子化学库，HF/DFT/MP2/CCSD(T)/多参考方法，易作为科研与方法开发的二次开发平台；配套 [gpu4pyscf](https://github.com/pyscf/gpu4pyscf) 提供 GPU 加速 | 🟢 最新 **v2.13.1**（2026-06-01），发布频繁，社区活跃 |
| **[Psi4](https://github.com/psi4/psi4)** | C++/Python · LGPL-3.0 | 高精度从头算（含 SAPT 相互作用能分析），Python API 友好，教学与方法研究常用 | 🟡 最新 **v1.10**（2025-09），按年度发布 |
| **[NWChem](https://github.com/nwchemgit/nwchem)** | Fortran/C · ECL-2.0 | 面向**大规模并行 HPC** 的高性能量子化学/平面波 DFT，适合超算上的大体系计算 | 🟡 最新 **v7.3.1**（2025-11），持续维护 |
| **[CP2K](https://github.com/cp2k/cp2k)** | Fortran · GPL-2.0 | 凝聚态/界面体系的混合高斯-平面波 DFT 与 AIMD，擅长大体系第一性原理分子动力学 | 🟢 年度版本号（2025–2026 持续发布），见 [Releases](https://github.com/cp2k/cp2k/releases) |
| **[Quantum ESPRESSO](https://github.com/QEF/q-e)** | Fortran · GPL-2.0 | 平面波赝势 DFT，固体材料能带、声子、电子-声子耦合等周期性体系计算 | 🟡 最新 **v7.4.1**（2025-03） |
| **[GPAW](https://gitlab.com/gpaw/gpaw)** | Python/C · GPL-3.0 | 基于 PAW 的实空间/平面波 DFT，与 ASE 深度集成，脚本化材料计算 | 🟡 稳定维护，跟随 ASE 发布节奏 |
| **[ABINIT](https://github.com/abinit/abinit)** | Fortran · GPL-3.0 | 平面波 DFT/DFPT，强于响应性质、GW/BSE 激发态与声子 | 🟡 年度发布（ABINIT 2025 系列），持续维护 |
| **[xtb (GFN-xTB)](https://github.com/grimme-lab/xtb)** | Fortran · LGPL-3.0 | 半经验扩展紧束缚（GFN1/GFN2-xTB），**超快**几何优化与大体系/构象筛选预处理 | 🟢 近期发布新增 GPU 加速与 ALPB 改进（2026-05） |
| **[DFTB+](https://github.com/dftbplus/dftbplus)** | Fortran · LGPL-3.0 | 密度泛函紧束缚（DFTB），介于 DFT 与力场之间的快速半经验电子结构 | 🟡 稳定维护，定期发布 |

> 相关生态：[CREST](https://github.com/crest-lab/crest)（基于 xtb 的自动构象/异构体采样）、
> [ORCA](https://www.faccts.de/orca/)（学术免费但**非开源**）、[OpenMolcas](https://gitlab.com/Molcas/OpenMolcas)（多参考/CASPT2）。

---

## 2. 分子动力学模拟

经典力场分子动力学（MD），用于生物大分子、软物质、材料的动力学与自由能计算。

| 项目 | 语言 / 许可 | 使用方向 | 更新情况（截至 2026-06） |
|------|------------|---------|--------------------------|
| **[GROMACS](https://github.com/gromacs/gromacs)** | C++ · LGPL-2.1 | 生物分子 MD 的主力，速度极快、GPU 优化好；蛋白质/膜/自由能微扰 | 🟢 **2026.2**（2026 系列，2026.0 于 2026-01 发布），新增 AMBER 力场与 NNP 支持 |
| **[LAMMPS](https://github.com/lammps/lammps)** | C++ · GPL-2.0 | 材料/软物质大规模 MD，力场与势函数极其丰富，可扩展性强 | 🟢 稳定版 **22Jul2025**（update4），开发版 **30Mar2026** |
| **[OpenMM](https://github.com/openmm/openmm)** | C++/Python · MIT/LGPL | GPU 加速的 MD 工具箱，Python API 灵活，易嵌入自定义力/ML 势（[openmm-ml](https://github.com/openmm/openmm-ml)） | 🟢 最新 **v8.5.2**（2026-06） |
| **[HOOMD-blue](https://github.com/glotzerlab/hoomd-blue)** | C++/Python · BSD-3 | 面向 GPU 的粗粒化/胶体/自组装模拟，Python 脚本驱动 | 🟢 活跃发布 |
| **[ESPResSo](https://github.com/espressomd/espresso)** | C++/Python · GPL-3.0 | 软物质与复杂流体（聚电解质、带电体系、流体力学耦合） | 🟡 稳定维护 |
| **[AmberTools](https://ambermd.org/AmberTools.php)** | C/C++/Python · GPL/其他 | Amber 力场生态的**开源**部分（建模、参数化、MM/PBSA、cpptraj 分析） | 🟡 年度发布（主程序 Amber 需付费，AmberTools 开源） |

> 说明：**NAMD** 学术免费但非完全开源；**Desmond**、商业版 **Amber** 等不在本列表范围。

---

## 3. 机器学习势函数 / 原子尺度机器学习

用机器学习拟合势能面（MLIP），以接近 DFT 精度、接近力场速度进行大规模/长时间模拟。

| 项目 | 语言 / 许可 | 使用方向 | 更新情况（截至 2026-06） |
|------|------------|---------|--------------------------|
| **[DeePMD-kit](https://github.com/deepmodeling/deepmd-kit)** | Python/C++ · LGPL-3.0 | 深度势能（Deep Potential）训练与部署，对接 LAMMPS/GROMACS，含预训练大模型（DPA 系列） | 🟢 **v3.1.3** 系列，新增内置预训练模型 DPA3 与分布式训练 |
| **[MACE](https://github.com/ACEsuit/mace)** | Python · MIT | 高阶等变消息传递 MLIP，精度/效率领先；含通用基础模型 [mace-foundations](https://github.com/ACEsuit/mace-foundations) | 🟢 高度活跃，基础模型持续迭代 |
| **[NequIP / Allegro](https://github.com/mir-group/nequip)** | Python · MIT | E(3) 等变图神经网络势，数据高效，小数据集即可高精度；Allegro 为可扩展变体 | 🟢 活跃维护 |
| **[MatGL](https://github.com/materialsvirtuallab/matgl)** | Python · BSD-3 | 材料图神经网络库，集成 **M3GNet / CHGNet / MEGNet / TensorNet**，含通用势与性质预测预训练模型 | 🟢 **v2.0.0**（2025-11），默认 PyG 后端 |
| **[fairchem](https://github.com/FAIR-Chem/fairchem)** | Python · MIT | Meta FAIR 的 Open Catalyst 生态，催化/材料的通用大模型（UMA 等）与数据集 | 🟢 高度活跃 |
| **[TorchANI](https://github.com/aiqm/torchani)** | Python · MIT | ANI 系列神经网络势（有机分子），PyTorch 实现，易上手 | 🟡 稳定维护 |
| **[SchNetPack](https://github.com/atomistic-machine-learning/schnetpack)** | Python · MIT | 原子神经网络建模工具箱（SchNet/PaiNN 等），适合方法学习与研究 | 🟡 稳定维护 |
| **[sGDML](https://github.com/stefanch/sGDML)** | Python · MIT | 小分子高精度对称梯度力场（核方法），适合精确势能面重构 | 🟠 偶尔更新 |

> 速览榜单：[best-of-atomistic-machine-learning](https://github.com/JuDFTteam/best-of-atomistic-machine-learning)
> 维护了一份按热度排名的原子尺度机器学习项目大全，可作为本节的扩展。

---

## 4. 材料建模与高通量工作流

原子结构操作、数据接口与高通量计算自动化（连接 DFT 引擎、管理大批量任务）。

| 项目 | 语言 / 许可 | 使用方向 | 更新情况（截至 2026-06） |
|------|------------|---------|--------------------------|
| **[ASE](https://gitlab.com/ase/ase)** | Python · LGPL | 原子模拟环境，统一的结构对象与 **Calculator 接口**，胶水式驱动几乎所有 DFT/MLIP 引擎 | 🟢 最新 **v3.28.0**（2026-03） |
| **[pymatgen](https://github.com/materialsproject/pymatgen)** | Python · MIT | Materials Project 核心库，结构/对称/相图/电子结构分析，材料数据管线基石 | 🟢 日历版本号（如 **2026.5.18**），发布频繁 |
| **[AiiDA](https://github.com/aiidateam/aiida-core)** | Python · MIT | 高通量计算的**工作流引擎与数据溯源**（provenance），管理海量任务与可复现性 | 🟢 活跃维护 |
| **[atomate2](https://github.com/materialsproject/atomate2)** | Python · 修改版 BSD | 模块化材料计算工作流库，封装 VASP/QE 与多种 MLIP 的标准流程 | 🟢 活跃（2025 框架论文发布） |
| **[FireWorks](https://github.com/materialsproject/fireworks)** | Python · 修改版 BSD | 工作流任务的定义、管理与在集群上的分发执行 | 🟡 稳定维护 |
| **[Custodian](https://github.com/materialsproject/custodian)** | Python · MIT | 计算任务的"看护"与错误自动恢复（即时纠错），常配合 atomate2/pymatgen | 🟡 稳定维护 |

---

## 5. 化学信息学

分子表示、描述符、指纹、化学反应与机器学习特征工程。

| 项目 | 语言 / 许可 | 使用方向 | 更新情况（截至 2026-06） |
|------|------------|---------|--------------------------|
| **[RDKit](https://github.com/rdkit/rdkit)** | C++/Python · BSD-3 | 化学信息学事实标准：分子读写、指纹/描述符、子结构匹配、构象生成、QSAR 特征 | 🟢 最新 **2026.03.3**（2026-06），季度发布 |
| **[Open Babel](https://github.com/openbabel/openbabel)** | C++ · GPL-2.0 | 化学文件**格式转换**与互操作（110+ 格式），命令行/库两用 | 🟠 稳定但更新缓慢（主版本 3.1.1） |
| **[DeepChem](https://github.com/deepchem/deepchem)** | Python · MIT | 面向药物发现/材料/量子化学的深度学习工具箱，大量数据集与模型基线 | 🟢 活跃维护 |

> 扩展资源：[awesome-drug-discovery](https://github.com/yboulaamane/awesome-drug-discovery)
> 汇总了药物发现方向的计算工具与数据库。

---

## 6. 分子对接与药物设计

预测小分子-蛋白结合构象与亲和力，用于虚拟筛选与先导化合物发现。

| 项目 | 语言 / 许可 | 使用方向 | 更新情况（截至 2026-06） |
|------|------------|---------|--------------------------|
| **[AutoDock Vina](https://github.com/ccsb-scripps/AutoDock-Vina)** | C++/Python · Apache-2.0 | 最流行的开源分子对接引擎，速度快、Python 绑定，虚拟筛选首选 | 🟡 最新 **v1.2.7**，稳定维护 |
| **[AutoDock-GPU](https://github.com/ccsb-scripps/AutoDock-GPU)** | C/C++ · GPL-2.0 | AutoDock4 评分的 GPU/OpenCL 加速版，适合大规模虚拟筛选 | 🟡 稳定维护 |
| **[smina](https://github.com/mwojcikowski/smina)** | C++ · Apache/GPL | Vina 分支，便于自定义评分函数与最小化，文档社区友好 | 🟠 偶尔更新 |
| **[gnina](https://github.com/gnina/gnina)** | C++ · Apache-2.0 | 集成 **CNN 打分**的对接工具（基于 smina），深度学习增强的姿态评分 | 🟢 活跃维护 |

---

## 7. 轨迹分析与可视化

MD 轨迹的读取/分析，以及分子结构与结果的可视化。

| 项目 | 语言 / 许可 | 使用方向 | 更新情况（截至 2026-06） |
|------|------------|---------|--------------------------|
| **[MDAnalysis](https://github.com/MDAnalysis/mdanalysis)** | Python · GPL-2.0 | MD 轨迹分析的主流 Python 库，支持几乎所有轨迹格式，丰富的分析模块 | 🟢 活跃维护（已支持 NumPy 2） |
| **[MDTraj](https://github.com/mdtraj/mdtraj)** | Python · LGPL-2.1 | 轻量快速的轨迹读写与分析，与 OpenMM/Python 生态契合 | 🟡 稳定维护 |
| **[PyMOL (开源版)](https://github.com/schrodinger/pymol-open-source)** | C/Python · 类 BSD | 分子结构与轨迹的高质量可视化、出图，结构生物学常用 | 🟡 稳定维护（开源版） |
| **[Avogadro 2](https://github.com/OpenChemistry/avogadro2)** | C++/Qt · BSD-3 | 跨平台分子编辑/建模/可视化 GUI，教学与建模友好 | 🟡 稳定维护 |
| **[NGLView](https://github.com/nglviewer/nglview)** / **[py3Dmol](https://github.com/3dmol/3Dmol.js)** | Python/JS · MIT/BSD | Jupyter Notebook 内嵌交互式 3D 分子可视化 | 🟡 稳定维护 |
| **[OVITO (基础版)](https://www.ovito.org/)** | C++/Python · GPL/商业 | 大规模原子构型/MD 轨迹可视化与分析（基础版开源） | 🟡 稳定发布 |

> 注：**VMD** 免费但非开源；其在大体系轨迹可视化中仍非常常用。

---

## 8. 如何选型（速查）

| 我的需求 | 推荐起点 |
|---------|---------|
| 分子的精确能量/光谱（小到中等体系） | **PySCF** / **Psi4**（高精度）、**ORCA**（免费非开源） |
| 周期性固体/材料的 DFT | **Quantum ESPRESSO** / **CP2K** / **GPAW** / **ABINIT** |
| 超算上的大规模量子化学 | **NWChem** / **CP2K** |
| 超快预筛选/构象搜索 | **xtb + CREST** / **DFTB+** |
| 蛋白质/生物分子 MD | **GROMACS** / **OpenMM** / **AmberTools** |
| 材料/软物质大规模 MD | **LAMMPS** / **HOOMD-blue** |
| 用 ML 势做近 DFT 精度的大体系 MD | **MACE** / **DeePMD-kit** / **NequIP** / **MatGL** |
| 高通量自动化计算 | **ASE** + **pymatgen** + **atomate2** / **AiiDA** |
| 分子描述符/指纹/化学信息学 | **RDKit**（+ **Open Babel** 做格式转换） |
| 虚拟筛选/分子对接 | **AutoDock Vina** / **AutoDock-GPU** / **gnina** |
| MD 轨迹分析 | **MDAnalysis** / **MDTraj** |
| 分子可视化出图 | **PyMOL** / **Avogadro 2** / **NGLView** |

---

## 9. 参与贡献

欢迎补充与勘误：

- **新增项目**：请提供 GitHub/官网链接、语言与许可证、一句话使用方向、最新版本与发布日期。
- **更新状态**：版本号随时间变化，发现过时信息请提交修订（并附 Releases 链接佐证）。
- **收录标准**：开源（OSI 许可优先）、与计算化学直接相关、有实际用户或活跃维护。

> ⚠️ 免责声明：表格中的"更新情况"为 **2026 年 6 月**前后通过公开 Releases 页面整理，仅供参考；
> 请以各项目官方仓库的实时发布信息为准。许可证以各仓库声明为准。
