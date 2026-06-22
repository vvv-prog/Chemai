# Chemai — Awesome Computational Chemistry (计算化学开源项目精选)

> 🌐 **Language / 语言**：[中文](README.md) ｜ **English**

> A continuously maintained collection of **open-source computational chemistry** projects,
> focused on each project's **usage direction** and **update status** — to help researchers,
> students, and engineers choose tools quickly.

The repository is organized into 7 categories. **Every project has its own detailed entry**
(official site, repository, language/license, usage direction, key features, update status)
under the [`docs/en/`](docs/en/) directory.

- 📌 **Usage direction**: what the project is best at, and typical application scenarios.
- 🔄 **Update status**: latest version / release cadence / maintenance activity as of **June 2026**.
  Versions change over time — **the live status is whatever each project's Releases page says**
  (links are provided in the docs).
- 🏷️ **Activity legend**: 🟢 Highly active (released within the last few months) ｜ 🟡 Steadily maintained (annual/quarterly) ｜ 🟠 Slow / occasional updates.

---

## 📚 Categories (click for detailed docs)

| # | Category | Scope | Representative projects |
|---|----------|-------|-------------------------|
| 01 | [Quantum Chemistry & Electronic Structure](docs/en/01-quantum-chemistry.md) | HF/DFT/post-HF, semi-empirical, periodic systems | PySCF · Psi4 · NWChem · CP2K · Quantum ESPRESSO · GPAW · ABINIT · xtb · DFTB+ |
| 02 | [Molecular Dynamics](docs/en/02-molecular-dynamics.md) | Classical MD, free energy, soft matter | GROMACS · LAMMPS · OpenMM · HOOMD-blue · ESPResSo · AmberTools |
| 03 | [Machine-Learning Potentials / Atomistic ML](docs/en/03-ml-potentials.md) | MLIP / NNP, universal pretrained potentials | DeePMD-kit · MACE · NequIP/Allegro · MatGL · fairchem · TorchANI · SchNetPack · sGDML |
| 04 | [Materials Modeling & High-throughput Workflows](docs/en/04-materials-workflows.md) | Structure handling, automation, provenance | ASE · pymatgen · AiiDA · atomate2 · FireWorks · Custodian |
| 05 | [Cheminformatics](docs/en/05-cheminformatics.md) | Molecular representation, fingerprints, format conversion, chem-ML | RDKit · Open Babel · DeepChem |
| 06 | [Docking & Drug Design](docs/en/06-docking-drug-design.md) | Docking, virtual screening, binding affinity | AutoDock Vina · AutoDock-GPU · smina · gnina |
| 07 | [Trajectory Analysis & Visualization](docs/en/07-visualization-analysis.md) | Trajectory analysis, molecular visualization | MDAnalysis · MDTraj · PyMOL · Avogadro 2 · NGLView/py3Dmol · OVITO |

---

## ⚡ Update overview of major projects (as of 2026-06)

| Project | Category | Latest version / status | Activity |
|---------|----------|-------------------------|----------|
| [PySCF](docs/en/01-quantum-chemistry.md#pyscf) | Quantum chemistry | v2.13.1 (2026-06) | 🟢 |
| [Psi4](docs/en/01-quantum-chemistry.md#psi4) | Quantum chemistry | v1.10 (2025-09) | 🟡 |
| [NWChem](docs/en/01-quantum-chemistry.md#nwchem) | Quantum chemistry | v7.3.1 (2025-11) | 🟡 |
| [CP2K](docs/en/01-quantum-chemistry.md#cp2k) | Quantum chemistry | Annual releases (active 2025–2026) | 🟢 |
| [Quantum ESPRESSO](docs/en/01-quantum-chemistry.md#quantum-espresso) | Quantum chemistry | v7.4.1 (2025-03) | 🟡 |
| [GPAW](docs/en/01-quantum-chemistry.md#gpaw) | Quantum chemistry | v25.7.0 (2025-07) | 🟡 |
| [ABINIT](docs/en/01-quantum-chemistry.md#abinit) | Quantum chemistry | v10.6 (2026-02) | 🟡 |
| [xtb](docs/en/01-quantum-chemistry.md#xtb-gfn-xtb) | Semi-empirical | GPU acceleration added (2026-05) | 🟢 |
| [GROMACS](docs/en/02-molecular-dynamics.md#gromacs) | Molecular dynamics | 2026.2 (2026 series) | 🟢 |
| [LAMMPS](docs/en/02-molecular-dynamics.md#lammps) | Molecular dynamics | stable 22Jul2025 / feature 30Mar2026 | 🟢 |
| [OpenMM](docs/en/02-molecular-dynamics.md#openmm) | Molecular dynamics | v8.5.2 (2026-06) | 🟢 |
| [DeePMD-kit](docs/en/03-ml-potentials.md#deepmd-kit) | ML potential | v3.1.x (incl. DPA3 pretrained) | 🟢 |
| [MACE](docs/en/03-ml-potentials.md#mace) | ML potential | foundation models iterating | 🟢 |
| [MatGL](docs/en/03-ml-potentials.md#matgl-materials-graph-library) | ML potential | v2.0.0 (2025-11) | 🟢 |
| [fairchem](docs/en/03-ml-potentials.md#fairchem-fair-chemistry) | ML potential | active (2026-06) | 🟢 |
| [ASE](docs/en/04-materials-workflows.md#ase-atomic-simulation-environment) | Workflow | v3.28.0 (2026-03) | 🟢 |
| [pymatgen](docs/en/04-materials-workflows.md#pymatgen-python-materials-genomics) | Workflow | 2026.5.18 (calendar versioning) | 🟢 |
| [RDKit](docs/en/05-cheminformatics.md#rdkit) | Cheminformatics | 2026.03.3 (2026-06) | 🟢 |
| [Open Babel](docs/en/05-cheminformatics.md#open-babel) | Cheminformatics | 3.1.1 (slow updates) | 🟠 |
| [AutoDock Vina](docs/en/06-docking-drug-design.md#autodock-vina) | Docking | v1.2.7 | 🟡 |
| [gnina](docs/en/06-docking-drug-design.md#gnina) | Docking | v1.3.2 (2025-07, moved to PyTorch) | 🟢 |
| [MDAnalysis](docs/en/07-visualization-analysis.md#mdanalysis) | Trajectory analysis | active (NumPy 2 support) | 🟢 |
| [PyMOL (open source)](docs/en/07-visualization-analysis.md#pymol-open-source) | Visualization | 3.1.x (2026-03) | 🟡 |

> See each category doc for the full project list and per-project details.

---

## 🧭 Quick selection guide

| My need | Where to start |
|---------|----------------|
| Accurate molecular energies/spectra (small–medium systems) | **PySCF** / **Psi4** (high accuracy), **ORCA** (free, not open source) |
| DFT for periodic solids/materials | **Quantum ESPRESSO** / **CP2K** / **GPAW** / **ABINIT** |
| Large-scale quantum chemistry on HPC | **NWChem** / **CP2K** |
| Ultra-fast pre-screening / conformer search | **xtb + CREST** / **DFTB+** |
| Protein / biomolecular MD | **GROMACS** / **OpenMM** / **AmberTools** |
| Large-scale materials / soft-matter MD | **LAMMPS** / **HOOMD-blue** |
| Near-DFT-accuracy MD on large systems via ML | **MACE** / **DeePMD-kit** / **NequIP** / **MatGL** |
| High-throughput automation | **ASE** + **pymatgen** + **atomate2** / **AiiDA** |
| Molecular descriptors / fingerprints / cheminformatics | **RDKit** (+ **Open Babel** for format conversion) |
| Virtual screening / molecular docking | **AutoDock Vina** / **AutoDock-GPU** / **gnina** |
| MD trajectory analysis | **MDAnalysis** / **MDTraj** |
| Molecular visualization & figures | **PyMOL** / **Avogadro 2** / **NGLView** |

---

## 🤝 Contributing

Additions and corrections are welcome:

- **New projects**: provide the GitHub/website link, language and license, a one-line usage
  direction, and the latest version with release date; add it to the matching
  [`docs/en/`](docs/en/) category file (and its [`docs/`](docs/) Chinese counterpart if possible).
- **Status updates**: versions change over time — if you spot stale info, please submit a fix
  (with a Releases link as evidence).
- **Inclusion criteria**: open source (OSI license preferred), directly related to computational
  chemistry, with real users or active maintenance.

> ⚠️ **Disclaimer**: the "update status" was compiled around **June 2026** from each project's
> public Releases page and is for reference only; defer to the official repository's live release
> info. Licenses are as declared in each repository.
