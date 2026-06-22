# 01 · 量子化学与电子结构计算

[← 返回首页](../README.md)

求解电子结构（HF、DFT、后 HF、半经验等），用于分子/固体的能量、几何优化、
反应路径、光谱与电子性质计算。

> 🔄 **更新情况** 截至 **2026 年 6 月**，版本号随时间变化，实时状态请点击各项目的 Releases 链接。
> 活跃度：🟢 高度活跃 ｜ 🟡 稳定维护 ｜ 🟠 缓慢/偶尔更新。

---

## PySCF

- **官网**：https://pyscf.org
- **代码仓库**：https://github.com/pyscf/pyscf ｜ [Releases](https://github.com/pyscf/pyscf/releases)
- **语言 / 许可**：Python + C / Apache-2.0
- **🎯 使用方向**：Python 原生的量子化学库，覆盖 HF、DFT、MP2、CCSD(T)、CASSCF/CASPT2、
  TDDFT 等方法，既能做常规分子计算，也是**方法开发与二次开发的首选平台**（模块化、易嵌入自定义代码）。
  支持分子与周期性体系。
- **✨ 主要特性**：纯 Python 接口，便于脚本化与和 NumPy/SciPy/机器学习库联动；
  GPU 加速由配套项目 [gpu4pyscf](https://github.com/pyscf/gpu4pyscf) 提供。
- **🔄 更新情况**：🟢 最新 **v2.13.1**（2026-06-01）。发布频繁（数月一个小版本），社区非常活跃。
- **🔗 生态**：gpu4pyscf（GPU）、[dmrgscf](https://github.com/pyscf/dmrgscf)（DMRG）、与 ASE 集成。

## Psi4

- **官网**：https://psicode.org
- **代码仓库**：https://github.com/psi4/psi4 ｜ [Releases](https://github.com/psi4/psi4/releases)
- **语言 / 许可**：C++ + Python / LGPL-3.0
- **🎯 使用方向**：高精度从头算电子结构，尤其擅长 **SAPT（对称匹配微扰）相互作用能分解**，
  适合非共价相互作用研究与教学。Python API（Psi4NumPy）友好。
- **🔄 更新情况**：🟡 最新 **v1.10**（2025-09）。按年度发布大版本，稳定维护。

## NWChem

- **官网**：https://nwchemgit.github.io
- **代码仓库**：https://github.com/nwchemgit/nwchem ｜ [Releases](https://github.com/nwchemgit/nwchem/releases)
- **语言 / 许可**：Fortran + C / ECL-2.0
- **🎯 使用方向**：面向**大规模并行 HPC** 的高性能计算化学套件，分子量子化学与平面波 DFT 兼备，
  适合在超算上跑大体系（高阶相关方法、TCE 等）。
- **🔄 更新情况**：🟡 最新 **v7.3.1**（2025-11-06）。由 PNNL 等持续维护。

## CP2K

- **官网**：https://www.cp2k.org
- **代码仓库**：https://github.com/cp2k/cp2k ｜ [Releases](https://github.com/cp2k/cp2k/releases)
- **语言 / 许可**：Fortran / GPL-2.0
- **🎯 使用方向**：凝聚态、表面/界面与液相体系的电子结构与 **第一性原理分子动力学（AIMD）**，
  采用混合高斯-平面波（GPW/GAPW）方法，擅长**大体系**与长时间 AIMD。
- **🔄 更新情况**：🟢 采用年度版本号，2025–2026 持续发布，开发活跃。

## Quantum ESPRESSO

- **官网**：https://www.quantum-espresso.org
- **代码仓库**：https://github.com/QEF/q-e ｜ [Releases](https://github.com/QEF/q-e/releases)
- **语言 / 许可**：Fortran / GPL-2.0
- **🎯 使用方向**：基于平面波 + 赝势的周期性体系 DFT，固体材料的**能带、态密度、声子（DFPT）、
  电子-声子耦合**等标准计算，材料计算入门与生产的常用引擎。
- **🔄 更新情况**：🟡 最新稳定版 **v7.4.1**（2025-03）。

## GPAW

- **官网**：https://gpaw.readthedocs.io
- **代码仓库**：https://gitlab.com/gpaw/gpaw
- **语言 / 许可**：Python + C / GPL-3.0
- **🎯 使用方向**：基于 PAW 的 DFT，支持实空间网格、平面波与 LCAO 多种模式；
  **与 ASE 深度集成**，非常适合脚本化的材料/表面计算与高通量流程。
- **🔄 更新情况**：🟡 最新 **v25.7.0**（2025-07-29），跟随 ASE 节奏稳定发布。

## ABINIT

- **官网**：https://www.abinit.org
- **代码仓库**：https://github.com/abinit/abinit ｜ [Releases](https://github.com/abinit/abinit/releases)
- **语言 / 许可**：Fortran / GPL-3.0
- **🎯 使用方向**：平面波 DFT/DFPT，强于**响应性质、声子、GW/BSE 激发态**与介电性质，
  适合需要精确电子激发与光学性质的固体研究。
- **🔄 更新情况**：🟡 最新 **v10.6**（2026-02-07），新增 DMFT、自旋螺旋、ARM/GPU 改进。

## xtb（GFN-xTB）

- **官网**：https://xtb-docs.readthedocs.io
- **代码仓库**：https://github.com/grimme-lab/xtb ｜ [Releases](https://github.com/grimme-lab/xtb/releases)
- **语言 / 许可**：Fortran / LGPL-3.0
- **🎯 使用方向**：半经验**扩展紧束缚**方法（GFN0/1/2-xTB），以接近力场的速度做几何优化、
  频率与能量；常作为大体系或大批量构象的**快速预处理/预筛选**，再交给 DFT 精算。
- **🔄 更新情况**：🟢 近期发布新增 GPU 加速、ALPB 溶剂模型与优化器改进（2026-05）。
- **🔗 生态**：[CREST](https://github.com/crest-lab/crest)（基于 xtb 的自动构象/异构体采样与反应网络探索）。

## DFTB+

- **官网**：https://dftbplus.org
- **代码仓库**：https://github.com/dftbplus/dftbplus ｜ [Releases](https://github.com/dftbplus/dftbplus/releases)
- **语言 / 许可**：Fortran / LGPL-3.0
- **🎯 使用方向**：密度泛函紧束缚（DFTB）与 xTB 方法的实现，介于 DFT 与经典力场之间的
  **快速半经验电子结构**，可做较大体系的几何/动力学与电子输运。
- **🔄 更新情况**：🟡 稳定维护，定期发布。

---

## 同方向值得了解（部分非开源）

| 项目 | 说明 |
|------|------|
| [ORCA](https://www.faccts.de/orca/) | 功能全面、易用，学术**免费但非开源**；DFT/相关方法/激发态的常用选择 |
| [OpenMolcas](https://gitlab.com/Molcas/OpenMolcas) | 开源多参考方法（CASSCF/CASPT2/RASSCF），强相关体系 |
| [CREST](https://github.com/crest-lab/crest) | 基于 xtb 的自动构象采样工具，配合 xtb 使用 |
| [Dalton](https://gitlab.com/dalton/dalton) | 分子性质（响应理论、NMR、磁性质）见长 |

[← 返回首页](../README.md) ｜ [下一类：分子动力学模拟 →](02-molecular-dynamics.md)
