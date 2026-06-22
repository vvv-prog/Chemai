# 07 · 轨迹分析与可视化

> **🌐 语言:** <kbd>[English](../07-visualization-analysis.md)</kbd> <kbd>[**中文**](07-visualization-analysis.md)</kbd>

[← 返回首页](../README.zh.md)

分子动力学**轨迹的读取与分析**，以及分子结构、轨迹与计算结果的**可视化与出图**。

> 🔄 **更新情况** 截至 **2026 年 6 月**。活跃度：🟢 高度活跃 ｜ 🟡 稳定维护 ｜ 🟠 缓慢更新。

---

## MDAnalysis

- **官网**：https://www.mdanalysis.org
- **代码仓库**：https://github.com/MDAnalysis/mdanalysis ｜ [Releases](https://github.com/MDAnalysis/mdanalysis/releases)
- **语言 / 许可**：Python / GPL-2.0
- **🎯 使用方向**：MD 轨迹分析的主流 Python 库，**支持几乎所有轨迹/拓扑格式**
  （GROMACS、Amber、NAMD、LAMMPS…），提供强大的原子选择语言与丰富分析模块
  （RMSD/RMSF、氢键、RDF、密度、接触分析等），并支持并行分析。
- **🔄 更新情况**：🟢 活跃维护（已支持 NumPy 2.0+，新增 GROMACS 2025 TPR、并行分析等）。

## MDTraj

- **官网**：https://mdtraj.org
- **代码仓库**：https://github.com/mdtraj/mdtraj ｜ [Releases](https://github.com/mdtraj/mdtraj/releases)
- **语言 / 许可**：Python / LGPL-2.1
- **🎯 使用方向**：**轻量、快速**的轨迹读写与几何分析库，I/O 高效，与 OpenMM、scikit-learn、
  Jupyter 生态契合，适合需要高性能批量分析的场景。
- **🔄 更新情况**：🟡 稳定维护（2026 年初仍有发布）。

## PyMOL（开源版）

- **官网**：https://www.pymol.org
- **代码仓库**：https://github.com/schrodinger/pymol-open-source ｜ [Releases](https://github.com/schrodinger/pymol-open-source/releases)
- **语言 / 许可**：C + Python / 类 BSD（开源版）
- **🎯 使用方向**：高质量的分子结构与轨迹**可视化与出版级渲染**，结构生物学（蛋白/配体复合物展示）常用；
  可用 Python 脚本批量出图。注意：由 Schrödinger 维护，**开源版**与付费的预编译/订阅版本并存。
- **🔄 更新情况**：🟡 最新 **3.1.x**（2026-03）。稳定维护。

## Avogadro 2

- **官网**：https://www.openchemistry.org/projects/avogadro2
- **代码仓库**：https://github.com/OpenChemistry/avogadro2 ｜ [Releases](https://github.com/OpenChemistry/avogadro2/releases)
- **语言 / 许可**：C++/Qt / BSD-3
- **🎯 使用方向**：跨平台的**分子编辑/建模/可视化 GUI**，可搭建分子、查看轨道/振动、生成量子化学输入文件，
  插件架构灵活，教学与建模友好。
- **🔄 更新情况**：🟡 稳定维护（OpenChemistry 项目）。

## NGLView / py3Dmol

- **代码仓库**：[nglview](https://github.com/nglviewer/nglview) ｜ [3Dmol.js / py3Dmol](https://github.com/3dmol/3Dmol.js)
- **语言 / 许可**：Python + JS / MIT、BSD
- **🎯 使用方向**：在 **Jupyter Notebook 中内嵌交互式 3D 分子/轨迹可视化**，
  非常适合数据分析过程中的快速查看与教学演示；py3Dmol 轻量、NGLView 功能更全（支持轨迹播放）。
- **🔄 更新情况**：🟡 稳定维护。

## OVITO（基础版）

- **官网**：https://www.ovito.org
- **代码仓库**：https://gitlab.com/stuko/ovito ｜ [Python 包](https://pypi.org/project/ovito/)
- **语言 / 许可**：C++ + Python / GPL（基础版）、商业版（Pro）
- **🎯 使用方向**：**大规模原子构型/MD 轨迹**的可视化与结构分析（位错分析、公共近邻分析、晶体结构识别等），
  材料模拟后处理常用；提供 Python 脚本接口用于自动化分析。**基础版开源**，Pro 版为付费。
- **🔄 更新情况**：🟡 稳定发布。

---

## 同方向值得了解（部分非开源）

| 项目 | 说明 |
|------|------|
| [VMD](https://www.ks.uiuc.edu/Research/vmd/) | 大体系轨迹可视化经典工具，**免费但非开源**；与 NAMD 配套 |
| [Mol*](https://github.com/molstar/molstar) | 现代 Web 端分子可视化（PDB 官方采用），开源 |
| [nglview ↔ MDAnalysis] | 二者可联用，在 Notebook 中边分析边看轨迹 |

[← 上一类：分子对接与药物设计](06-docking-drug-design.md) ｜ [返回首页](../README.zh.md)
