# 04 · 材料建模与高通量工作流

[← 返回首页](../README.md)

原子结构的构建与操作、与各类计算引擎的统一接口，以及**高通量计算的自动化、任务管理与数据溯源**。
这是连接「计算引擎」与「大规模科研产出」的中间层。

> 🔄 **更新情况** 截至 **2026 年 6 月**。活跃度：🟢 高度活跃 ｜ 🟡 稳定维护 ｜ 🟠 缓慢更新。

---

## ASE（Atomic Simulation Environment）

- **官网**：https://ase-lib.org
- **代码仓库**：https://gitlab.com/ase/ase
- **语言 / 许可**：Python / LGPL
- **🎯 使用方向**：原子模拟的**通用粘合层**——统一的 `Atoms` 结构对象和 **Calculator 接口**，
  可用同一套 Python 脚本驱动几乎所有主流 DFT 引擎（GPAW、QE、VASP、CP2K…）与机器学习势，
  并提供几何优化、NEB、声子、MD 等通用算法。是材料计算脚本化的事实标准。
- **🔄 更新情况**：🟢 最新 **v3.28.0**（2026-03-17）。活跃维护。

## pymatgen（Python Materials Genomics）

- **官网**：https://pymatgen.org
- **代码仓库**：https://github.com/materialsproject/pymatgen ｜ [Releases](https://github.com/materialsproject/pymatgen/releases)
- **语言 / 许可**：Python / MIT
- **🎯 使用方向**：Materials Project 的核心库，提供结构/对称性分析、**相图、Pourbaix 图、电子结构/能带分析、
  输入输出解析（VASP/QE 等）**，是材料数据分析与计算管线的基石。
- **🔄 更新情况**：🟢 采用日历版本号（如 **2026.5.18**），发布非常频繁。

## AiiDA

- **官网**：https://www.aiida.net
- **代码仓库**：https://github.com/aiidateam/aiida-core ｜ [Releases](https://github.com/aiidateam/aiida-core/releases)
- **语言 / 许可**：Python / MIT
- **🎯 使用方向**：高通量计算的**工作流引擎 + 数据溯源（provenance）平台**，自动记录每个计算的输入/输出/依赖关系，
  保证海量任务的**可复现性**，并在集群上调度执行。适合系统性的材料/化学高通量研究。
- **🔄 更新情况**：🟢 **v2.6.x** 系列，活跃维护，有公开发布路线图。

## atomate2

- **代码仓库**：https://github.com/materialsproject/atomate2 ｜ [Releases](https://github.com/materialsproject/atomate2/releases)
- **语言 / 许可**：Python / 修改版 BSD
- **🎯 使用方向**：**模块化材料计算工作流库**，把 VASP、QE 以及 CHGNet/M3GNet/MACE/NequIP 等机器学习势的
  标准计算流程（弛豫、能带、声子、弹性常数…）封装为可复用的 `Maker`，基于 jobflow，可对接 FireWorks。
- **🔄 更新情况**：🟢 活跃（2025 年框架论文发表，社区培训持续开展）。

## FireWorks

- **官网**：https://materialsproject.github.io/fireworks
- **代码仓库**：https://github.com/materialsproject/fireworks ｜ [Releases](https://github.com/materialsproject/fireworks/releases)
- **语言 / 许可**：Python / 修改版 BSD
- **🎯 使用方向**：工作流（Workflow / FireWork / FireTask）的**定义、存储（MongoDB）与在集群上的分发执行**，
  支持动态工作流、失败重试，常作为 atomate/atomate2 的执行后端。
- **🔄 更新情况**：🟡 稳定维护。

## Custodian

- **官网**：https://materialsproject.github.io/custodian
- **代码仓库**：https://github.com/materialsproject/custodian ｜ [Releases](https://github.com/materialsproject/custodian/releases)
- **语言 / 许可**：Python / MIT
- **🎯 使用方向**：计算任务的**「看护」与即时错误恢复（JIT）**框架——为 VASP/QE 等程序包裹错误检测与自动纠错逻辑
  （如修正不收敛、调整参数后重启），是高通量计算稳定运行的关键，常与 pymatgen/atomate2 配合。
- **🔄 更新情况**：🟡 稳定维护。

---

## 同方向值得了解

| 项目 | 说明 |
|------|------|
| [jobflow](https://github.com/materialsproject/jobflow) | atomate2 底层的工作流定义库，轻量灵活 |
| [phonopy](https://github.com/phonopy/phonopy) | 声子计算（有限位移法）的标准工具 |
| [spglib](https://github.com/spglib/spglib) | 晶体对称性分析底层库（被 ASE/pymatgen 使用） |
| [matminer](https://github.com/hackingmaterials/matminer) | 材料数据挖掘与特征工程 |
| [OPTIMADE](https://github.com/Materials-Consortia/OPTIMADE) | 材料数据库统一查询 API 标准 |

[← 上一类：机器学习势函数](03-ml-potentials.md) ｜ [返回首页](../README.md) ｜ [下一类：化学信息学 →](05-cheminformatics.md)
