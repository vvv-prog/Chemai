# 04 · Materials Modeling & High-throughput Workflows

> 🌐 [中文](../04-materials-workflows.md) ｜ **English**

[← Back to home](../../README.en.md)

Building and manipulating atomic structures, providing a unified interface to the various calculation
engines, and handling the **automation, job management, and data provenance** of high-throughput computing.
This is the layer that connects "calculation engines" to large-scale scientific output.

> 🔄 **Update status** is as of **June 2026**. Activity: 🟢 Highly active ｜ 🟡 Steadily maintained ｜ 🟠 Slow updates.

---

## ASE (Atomic Simulation Environment)

- **Website**: https://ase-lib.org
- **Repository**: https://gitlab.com/ase/ase
- **Language / License**: Python / LGPL
- **🎯 Usage direction**: the universal **glue layer** for atomistic simulation — a unified `Atoms` structure
  object and a **Calculator interface** that lets one set of Python scripts drive nearly all major DFT engines
  (GPAW, QE, VASP, CP2K, …) and ML potentials, plus common algorithms (geometry optimization, NEB, phonons, MD).
  It is the de facto standard for scripted materials calculations.
- **🔄 Update status**: 🟢 latest **v3.28.0** (2026-03-17). Actively maintained.

## pymatgen (Python Materials Genomics)

- **Website**: https://pymatgen.org
- **Repository**: https://github.com/materialsproject/pymatgen ｜ [Releases](https://github.com/materialsproject/pymatgen/releases)
- **Language / License**: Python / MIT
- **🎯 Usage direction**: the core library of the Materials Project, providing structure/symmetry analysis,
  **phase diagrams, Pourbaix diagrams, electronic-structure/band analysis, and I/O parsing (VASP/QE, …)** —
  the foundation of materials data analysis and computational pipelines.
- **🔄 Update status**: 🟢 calendar versioning (e.g. **2026.5.18**), very frequent releases.

## AiiDA

- **Website**: https://www.aiida.net
- **Repository**: https://github.com/aiidateam/aiida-core ｜ [Releases](https://github.com/aiidateam/aiida-core/releases)
- **Language / License**: Python / MIT
- **🎯 Usage direction**: a **workflow engine + data provenance** platform for high-throughput computing that
  automatically records every calculation's inputs/outputs/dependencies for **reproducibility**, and schedules
  execution on clusters — ideal for systematic high-throughput materials/chemistry research.
- **🔄 Update status**: 🟢 **v2.6.x** series, actively maintained with a public release roadmap.

## atomate2

- **Repository**: https://github.com/materialsproject/atomate2 ｜ [Releases](https://github.com/materialsproject/atomate2/releases)
- **Language / License**: Python / modified BSD
- **🎯 Usage direction**: a **modular materials-workflow library** that packages the standard pipelines (relaxation,
  band structure, phonons, elastic constants, …) for VASP, QE, and ML potentials such as CHGNet/M3GNet/MACE/NequIP
  into reusable `Maker`s; built on jobflow and able to use FireWorks.
- **🔄 Update status**: 🟢 active (framework paper published in 2025, with ongoing community training).

## FireWorks

- **Website**: https://materialsproject.github.io/fireworks
- **Repository**: https://github.com/materialsproject/fireworks ｜ [Releases](https://github.com/materialsproject/fireworks/releases)
- **Language / License**: Python / modified BSD
- **🎯 Usage direction**: **definition, storage (MongoDB), and cluster execution/dispatch** of workflows
  (Workflow / FireWork / FireTask), with support for dynamic workflows and failure retries; often the execution
  backend for atomate/atomate2.
- **🔄 Update status**: 🟡 steadily maintained.

## Custodian

- **Website**: https://materialsproject.github.io/custodian
- **Repository**: https://github.com/materialsproject/custodian ｜ [Releases](https://github.com/materialsproject/custodian/releases)
- **Language / License**: Python / MIT
- **🎯 Usage direction**: a **"babysitting" and just-in-time (JIT) error-recovery** framework for calculations —
  it wraps programs like VASP/QE with error detection and automatic correction logic (e.g. fixing non-convergence,
  adjusting parameters and restarting). Key to robust high-throughput runs and commonly paired with pymatgen/atomate2.
- **🔄 Update status**: 🟡 steadily maintained.

---

## Also worth knowing

| Project | Notes |
|---------|-------|
| [jobflow](https://github.com/materialsproject/jobflow) | The lightweight, flexible workflow-definition library underlying atomate2 |
| [phonopy](https://github.com/phonopy/phonopy) | The standard tool for phonon calculations (finite-displacement method) |
| [spglib](https://github.com/spglib/spglib) | The underlying crystal-symmetry analysis library (used by ASE/pymatgen) |
| [matminer](https://github.com/hackingmaterials/matminer) | Materials data mining and feature engineering |
| [OPTIMADE](https://github.com/Materials-Consortia/OPTIMADE) | A standard API for unified queries across materials databases |

[← Previous: ML Potentials](03-ml-potentials.md) ｜ [Back to home](../../README.en.md) ｜ [Next: Cheminformatics →](05-cheminformatics.md)
