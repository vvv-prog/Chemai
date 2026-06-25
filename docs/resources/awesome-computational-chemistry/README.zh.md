# 计算化学开源项目精选 (Awesome Computational Chemistry)

> **🌐 语言:** <kbd>[English](README.md)</kbd> <kbd>[**中文**](README.zh.md)</kbd>
>
> 📦 本清单是 [**Chemai**](../../../README.zh.md) 项目的一部分 — 返回[项目说明](../../../README.zh.md)。

> 一个持续维护的**计算化学（Computational Chemistry）开源项目**汇总，
> 聚焦于每个项目的**使用方向**与**更新情况**，方便研究者、学生与工程师快速选型。

本清单按方向分为 7 大类，**每个项目都有独立的详细条目**（官网、代码仓库、语言/许可、
使用方向、主要特性、更新情况），中文详情见本目录下的 [`zh/`](zh/) 子目录（英文版即本目录各文件）。

- 📌 **使用方向**：该项目最擅长解决什么问题、典型应用场景。
- 🔄 **更新情况**：截至 **2026 年 6 月** 的最新版本 / 发布节奏 / 维护活跃度。
  版本会随时间变化，**实时状态以各项目 Releases 页面为准**（文档内已附链接）。
- 🏷️ **活跃度图例**：🟢 高度活跃（近数月有发布）｜🟡 稳定维护（按年/季度发布）｜🟠 缓慢/偶尔更新。

---

## 📚 分类目录（点击进入详细文档）

| # | 分类 | 内容概要 | 代表项目 |
|---|------|---------|---------|
| 01 | [量子化学与电子结构计算](zh/01-quantum-chemistry.md) | HF/DFT/后 HF、半经验、周期性体系 | PySCF · Psi4 · NWChem · CP2K · Quantum ESPRESSO · GPAW · ABINIT · xtb · DFTB+ |
| 02 | [分子动力学模拟](zh/02-molecular-dynamics.md) | 经典 MD、自由能、软物质 | GROMACS · LAMMPS · OpenMM · HOOMD-blue · ESPResSo · AmberTools |
| 03 | [机器学习势函数 / 原子尺度机器学习](zh/03-ml-potentials.md) | MLIP / NNP、通用预训练势 | DeePMD-kit · MACE · NequIP/Allegro · MatGL · fairchem · TorchANI · SchNetPack · sGDML |
| 04 | [材料建模与高通量工作流](zh/04-materials-workflows.md) | 结构操作、自动化、数据溯源 | ASE · pymatgen · AiiDA · atomate2 · FireWorks · Custodian |
| 05 | [化学信息学](zh/05-cheminformatics.md) | 分子表示、指纹、格式转换、化学 ML | RDKit · Open Babel · DeepChem |
| 06 | [分子对接与药物设计](zh/06-docking-drug-design.md) | 对接、虚拟筛选、结合亲和力 | AutoDock Vina · AutoDock-GPU · smina · gnina |
| 07 | [轨迹分析与可视化](zh/07-visualization-analysis.md) | 轨迹分析、分子可视化与出图 | MDAnalysis · MDTraj · PyMOL · Avogadro 2 · NGLView/py3Dmol · OVITO |

---

## ⚡ 主要项目更新概览（截至 2026-06）

| 项目 | 分类 | 最新版本 / 状态 | 活跃度 |
|------|------|----------------|--------|
| [PySCF](zh/01-quantum-chemistry.md#pyscf) | 量子化学 | v2.13.1（2026-06） | 🟢 |
| [Psi4](zh/01-quantum-chemistry.md#psi4) | 量子化学 | v1.10.2（2026-06） | 🟢 |
| [NWChem](zh/01-quantum-chemistry.md#nwchem) | 量子化学 | v7.3.1（2025-11） | 🟡 |
| [CP2K](zh/01-quantum-chemistry.md#cp2k) | 量子化学 | 年度发布（2025–2026 活跃） | 🟢 |
| [Quantum ESPRESSO](zh/01-quantum-chemistry.md#quantum-espresso) | 量子化学 | v7.5（2025-08） | 🟢 |
| [GPAW](zh/01-quantum-chemistry.md#gpaw) | 量子化学 | v25.7.0（2025-07） | 🟡 |
| [ABINIT](zh/01-quantum-chemistry.md#abinit) | 量子化学 | v10.6.7（2026-05） | 🟡 |
| [xtb](zh/01-quantum-chemistry.md#xtbgfn-xtb) | 半经验 | 新增 GPU 加速（2026-05） | 🟢 |
| [GROMACS](zh/02-molecular-dynamics.md#gromacs) | 分子动力学 | 2026.2（2026 系列） | 🟢 |
| [LAMMPS](zh/02-molecular-dynamics.md#lammps) | 分子动力学 | 稳定 22Jul2025 / 特性 30Mar2026 | 🟢 |
| [OpenMM](zh/02-molecular-dynamics.md#openmm) | 分子动力学 | v8.5.2（2026-06） | 🟢 |
| [DeePMD-kit](zh/03-ml-potentials.md#deepmd-kit) | ML 势 | v3.1.x（DPA3）;v3.2 测试版（DPA4） | 🟢 |
| [MACE](zh/03-ml-potentials.md#mace) | ML 势 | v0.3.16（2025-05） | 🟢 |
| [MatGL](zh/03-ml-potentials.md#matglmaterials-graph-library) | ML 势 | v4.0.2（2026-06） | 🟢 |
| [fairchem](zh/03-ml-potentials.md#fairchemfair-chemistry) | ML 势 | fairchem-core v2.21.0（2025-06） | 🟢 |
| [ASE](zh/04-materials-workflows.md#aseatomic-simulation-environment) | 工作流 | v3.29.0（2026-06） | 🟢 |
| [pymatgen](zh/04-materials-workflows.md#pymatgenpython-materials-genomics) | 工作流 | 2026.5.4（日历版本） | 🟢 |
| [RDKit](zh/05-cheminformatics.md#rdkit) | 化学信息学 | 2026.03.3（2026-05） | 🟢 |
| [Open Babel](zh/05-cheminformatics.md#open-babel) | 化学信息学 | 3.2.0（2025-05，更新缓慢） | 🟠 |
| [AutoDock Vina](zh/06-docking-drug-design.md#autodock-vina) | 对接 | v1.2.7 | 🟡 |
| [gnina](zh/06-docking-drug-design.md#gnina) | 对接 | v1.3.2（2025-07，迁移 PyTorch） | 🟢 |
| [MDAnalysis](zh/07-visualization-analysis.md#mdanalysis) | 轨迹分析 | v2.10.0（2024-10，支持 NumPy 2） | 🟢 |
| [PyMOL（开源版）](zh/07-visualization-analysis.md#pymol开源版) | 可视化 | 3.1.x（2026-03） | 🟡 |

> 完整项目列表与每个项目的详细信息见各分类文档。

---

## 🧭 如何选型（速查）

| 我的需求 | 推荐起点 |
|---------|---------|
| 分子的精确能量/光谱（小到中等体系） | **PySCF** / **Psi4**（高精度）、**ORCA**（免费非开源） |
| 周期性固体/材料的 DFT | **Quantum ESPRESSO** / **CP2K** / **GPAW** / **ABINIT** |
| 超算上的大规模量子化学 | **NWChem** / **CP2K** |
| 超快预筛选 / 构象搜索 | **xtb + CREST** / **DFTB+** |
| 蛋白质/生物分子 MD | **GROMACS** / **OpenMM** / **AmberTools** |
| 材料/软物质大规模 MD | **LAMMPS** / **HOOMD-blue** |
| 用 ML 势做近 DFT 精度的大体系 MD | **MACE** / **DeePMD-kit** / **NequIP** / **MatGL** |
| 高通量自动化计算 | **ASE** + **pymatgen** + **atomate2** / **AiiDA** |
| 分子描述符/指纹/化学信息学 | **RDKit**（+ **Open Babel** 做格式转换） |
| 虚拟筛选 / 分子对接 | **AutoDock Vina** / **AutoDock-GPU** / **gnina** |
| MD 轨迹分析 | **MDAnalysis** / **MDTraj** |
| 分子可视化出图 | **PyMOL** / **Avogadro 2** / **NGLView** |

---

## 🤝 参与贡献

欢迎补充与勘误：

- **新增项目**：请提供 GitHub/官网链接、语言与许可证、一句话使用方向、最新版本与发布日期，
  归入本目录下对应的 [`zh/`](zh/) 中文分类文件（如可能也同步更新英文版，即本目录各同名文件）。
- **更新状态**：版本号随时间变化，发现过时信息请提交修订（并附 Releases 链接佐证）。
- **收录标准**：开源（OSI 许可优先）、与计算化学直接相关、有实际用户或活跃维护。

> ⚠️ **免责声明**：文档中的「更新情况」为 **2026 年 6 月**前后通过各项目公开 Releases 页面整理，仅供参考；
> 请以官方仓库的实时发布信息为准。许可证以各仓库声明为准。
