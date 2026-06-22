# 07 · Trajectory Analysis & Visualization

> 🌐 [中文](../07-visualization-analysis.md) ｜ **English**

[← Back to home](../../README.en.md)

**Reading and analyzing** molecular dynamics trajectories, and the **visualization and figure generation** of
molecular structures, trajectories, and computational results.

> 🔄 **Update status** is as of **June 2026**. Activity: 🟢 Highly active ｜ 🟡 Steadily maintained ｜ 🟠 Slow updates.

---

## MDAnalysis

- **Website**: https://www.mdanalysis.org
- **Repository**: https://github.com/MDAnalysis/mdanalysis ｜ [Releases](https://github.com/MDAnalysis/mdanalysis/releases)
- **Language / License**: Python / GPL-2.0
- **🎯 Usage direction**: the mainstream Python library for MD trajectory analysis, **supporting nearly all
  trajectory/topology formats** (GROMACS, Amber, NAMD, LAMMPS, …), with a powerful atom-selection language and rich
  analysis modules (RMSD/RMSF, hydrogen bonds, RDF, density, contact analysis, …) and support for parallel analysis.
- **🔄 Update status**: 🟢 actively maintained (now supports NumPy 2.0+, adds GROMACS 2025 TPR, parallel analysis, etc.).

## MDTraj

- **Website**: https://mdtraj.org
- **Repository**: https://github.com/mdtraj/mdtraj ｜ [Releases](https://github.com/mdtraj/mdtraj/releases)
- **Language / License**: Python / LGPL-2.1
- **🎯 Usage direction**: a **lightweight, fast** trajectory I/O and geometry-analysis library with efficient I/O,
  fitting well with OpenMM, scikit-learn, and the Jupyter ecosystem — suited to high-performance batch analysis.
- **🔄 Update status**: 🟡 steadily maintained (still releasing in early 2026).

## PyMOL (open source)

- **Website**: https://www.pymol.org
- **Repository**: https://github.com/schrodinger/pymol-open-source ｜ [Releases](https://github.com/schrodinger/pymol-open-source/releases)
- **Language / License**: C + Python / BSD-like (open-source edition)
- **🎯 Usage direction**: high-quality **visualization and publication-grade rendering** of molecular structures and
  trajectories; common in structural biology (showing protein/ligand complexes) and scriptable for batch figures via
  Python. Note: maintained by Schrödinger, with the **open-source edition** alongside paid prebuilt/subscription versions.
- **🔄 Update status**: 🟡 latest **3.1.x** (2026-03). Steadily maintained.

## Avogadro 2

- **Website**: https://www.openchemistry.org/projects/avogadro2
- **Repository**: https://github.com/OpenChemistry/avogadro2 ｜ [Releases](https://github.com/OpenChemistry/avogadro2/releases)
- **Language / License**: C++/Qt / BSD-3
- **🎯 Usage direction**: a cross-platform **molecular editing/building/visualization GUI** that can build molecules,
  view orbitals/vibrations, and generate quantum-chemistry input files; a flexible plugin architecture makes it
  friendly for teaching and modeling.
- **🔄 Update status**: 🟡 steadily maintained (the OpenChemistry project).

## NGLView / py3Dmol

- **Repository**: [nglview](https://github.com/nglviewer/nglview) ｜ [3Dmol.js / py3Dmol](https://github.com/3dmol/3Dmol.js)
- **Language / License**: Python + JS / MIT, BSD
- **🎯 Usage direction**: **interactive 3D molecular/trajectory visualization embedded in Jupyter notebooks**, great
  for quick inspection during data analysis and for teaching; py3Dmol is lightweight, while NGLView is more
  full-featured (supports trajectory playback).
- **🔄 Update status**: 🟡 steadily maintained.

## OVITO (Basic)

- **Website**: https://www.ovito.org
- **Repository**: https://gitlab.com/stuko/ovito ｜ [Python package](https://pypi.org/project/ovito/)
- **Language / License**: C++ + Python / GPL (Basic), commercial (Pro)
- **🎯 Usage direction**: visualization and structural analysis of **large-scale atomic configurations / MD trajectories**
  (dislocation analysis, common-neighbor analysis, crystal-structure identification, …); common for materials-simulation
  post-processing, with a Python scripting interface for automated analysis. **Basic is open source**; Pro is paid.
- **🔄 Update status**: 🟡 steady releases.

---

## Also worth knowing (some not open source)

| Project | Notes |
|---------|-------|
| [VMD](https://www.ks.uiuc.edu/Research/vmd/) | The classic tool for large-system trajectory visualization, **free but not open source**; pairs with NAMD |
| [Mol*](https://github.com/molstar/molstar) | Modern web-based molecular visualization (adopted by the official PDB), open source |
| nglview ↔ MDAnalysis | The two can be used together to analyze and view trajectories inside a notebook |

[← Previous: Docking & Drug Design](06-docking-drug-design.md) ｜ [Back to home](../../README.en.md)
