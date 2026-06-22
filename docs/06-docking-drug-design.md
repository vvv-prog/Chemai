# 06 · Docking & Drug Design

> **🌐 Language:** <kbd>[**English**](06-docking-drug-design.md)</kbd> <kbd>[中文](zh/06-docking-drug-design.md)</kbd>

[← Back to home](../README.md)

Predicting the binding pose and binding affinity of small-molecule ligands to protein targets, for
**virtual screening** and lead discovery.

> 🔄 **Update status** is as of **June 2026**. Activity: 🟢 Highly active ｜ 🟡 Steadily maintained ｜ 🟠 Slow updates.

---

## AutoDock Vina

- **Website**: https://vina.scripps.edu
- **Repository**: https://github.com/ccsb-scripps/AutoDock-Vina ｜ [Releases](https://github.com/ccsb-scripps/AutoDock-Vina/releases)
- **Language / License**: C++ + Python / Apache-2.0
- **🎯 Usage direction**: the **most popular open-source docking engine** — fast, easy to use, with Python
  bindings and a CLI; suited to routine docking and medium-scale virtual screening. Supports the Vina and
  Vinardo scoring functions.
- **🔄 Update status**: 🟡 latest **v1.2.7**, steadily maintained (by the Forli Lab at Scripps Research).

## AutoDock-GPU

- **Repository**: https://github.com/ccsb-scripps/AutoDock-GPU ｜ [Releases](https://github.com/ccsb-scripps/AutoDock-GPU/releases)
- **Language / License**: C/C++ (OpenCL/CUDA) / GPL-2.0
- **🎯 Usage direction**: a **GPU/OpenCL/CUDA-accelerated** version of AutoDock4 scoring (Lamarckian genetic
  algorithm), offering order-of-magnitude speedups over CPU for large-scale virtual screening — suited to
  high-throughput docking of very large compound libraries.
- **🔄 Update status**: 🟡 steadily maintained (Scripps Forli Lab).

## smina

- **Repository**: https://github.com/mwojcikowski/smina ｜ [Releases](https://github.com/mwojcikowski/smina/releases)
- **Language / License**: C++ / Apache, GPL
- **🎯 Usage direction**: a fork of AutoDock Vina that makes **custom scoring functions and flexible energy
  minimization/scoring** easy, popular for scripted virtual screening (with friendlier input handling).
- **🔄 Update status**: 🟠 occasional updates (functionally stable).

## gnina

- **Repository**: https://github.com/gnina/gnina ｜ [Releases](https://github.com/gnina/gnina/releases)
- **Language / License**: C++ / Apache-2.0
- **🎯 Usage direction**: a docking tool built on smina that integrates **convolutional neural network (CNN)
  scoring**, using deep learning to score and re-rank binding poses — typically improving scoring/ranking
  quality; suited to ML-enhanced docking and virtual screening.
- **🔄 Update status**: 🟢 latest **v1.3.2** (2025-07-08). v1.3 migrated the underlying deep-learning framework to
  **PyTorch**, retrained CNN scoring on CrossDocked2020 v1.3, and introduced knowledge distillation to speed up
  high-throughput screening. Actively maintained.

---

## Also worth knowing

| Project | Notes |
|---------|-------|
| [Meeko](https://github.com/forlilab/Meeko) | Ligand/receptor preparation (PDBQT generation) for Vina/AutoDock, from the Forli Lab |
| [DiffDock](https://github.com/gcorso/DiffDock) | Diffusion-model-based deep-learning docking (blind docking); a research hotspot |
| [DOCK 6](https://dock.compbio.ucsf.edu/) | The classic UCSF docking program, academic license |
| [OpenFE](https://github.com/OpenFreeEnergy/openfe) | Open-source relative/absolute binding free-energy (FEP) framework |

> Tip: ligand preparation before docking is often done with **Open Babel** ([see Cheminformatics](05-cheminformatics.md))
> or Meeko for PDBQT conversion.

[← Previous: Cheminformatics](05-cheminformatics.md) ｜ [Back to home](../README.md) ｜ [Next: Trajectory Analysis & Visualization →](07-visualization-analysis.md)
