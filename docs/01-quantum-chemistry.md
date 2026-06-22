# 01 · Quantum Chemistry & Electronic Structure

> **🌐 Language:** <kbd>[**English**](01-quantum-chemistry.md)</kbd> <kbd>[中文](zh/01-quantum-chemistry.md)</kbd>

[← Back to home](../README.md)

Solving the electronic structure (HF, DFT, post-HF, semi-empirical, …) for energies, geometry
optimization, reaction paths, spectra, and electronic properties of molecules and solids.

> 🔄 **Update status** is as of **June 2026**. Versions change over time — click each project's
> Releases link for the live status. Activity: 🟢 Highly active ｜ 🟡 Steadily maintained ｜ 🟠 Slow/occasional.

---

## PySCF

- **Website**: https://pyscf.org
- **Repository**: https://github.com/pyscf/pyscf ｜ [Releases](https://github.com/pyscf/pyscf/releases)
- **Language / License**: Python + C / Apache-2.0
- **🎯 Usage direction**: a Python-native quantum chemistry library covering HF, DFT, MP2, CCSD(T),
  CASSCF/CASPT2, TDDFT, and more. It works for routine molecular calculations and is also a
  **top platform for method development and customization** (modular, easy to embed custom code).
  Supports both molecular and periodic systems.
- **✨ Highlights**: pure-Python interface that pairs naturally with NumPy/SciPy and ML libraries;
  GPU acceleration via [gpu4pyscf](https://github.com/pyscf/gpu4pyscf).
- **🔄 Update status**: 🟢 latest **v2.13.1** (2026-06-01). Frequent releases (a minor version every
  few months), very active community.

## Psi4

- **Website**: https://psicode.org
- **Repository**: https://github.com/psi4/psi4 ｜ [Releases](https://github.com/psi4/psi4/releases)
- **Language / License**: C++ + Python / LGPL-3.0
- **🎯 Usage direction**: high-accuracy ab initio electronic structure, especially strong at
  **SAPT (symmetry-adapted perturbation theory) interaction-energy decomposition** — well suited to
  non-covalent interaction studies and teaching. Friendly Python API (Psi4NumPy).
- **🔄 Update status**: 🟡 latest **v1.10** (2025-09). Annual major releases, steadily maintained.

## NWChem

- **Website**: https://nwchemgit.github.io
- **Repository**: https://github.com/nwchemgit/nwchem ｜ [Releases](https://github.com/nwchemgit/nwchem/releases)
- **Language / License**: Fortran + C / ECL-2.0
- **🎯 Usage direction**: a high-performance computational chemistry suite built for **massively
  parallel HPC**, covering both molecular quantum chemistry and plane-wave DFT — suitable for large
  systems on supercomputers (high-order correlation methods, TCE, etc.).
- **🔄 Update status**: 🟡 latest **v7.3.1** (2025-11-06). Maintained by PNNL and collaborators.

## CP2K

- **Website**: https://www.cp2k.org
- **Repository**: https://github.com/cp2k/cp2k ｜ [Releases](https://github.com/cp2k/cp2k/releases)
- **Language / License**: Fortran / GPL-2.0
- **🎯 Usage direction**: electronic structure and **ab initio molecular dynamics (AIMD)** for
  condensed-phase, surface/interface, and liquid systems, using the mixed Gaussian/plane-wave
  (GPW/GAPW) approach — strong for **large systems** and long AIMD runs.
- **🔄 Update status**: 🟢 calendar versioning; active releases through 2025–2026.

## Quantum ESPRESSO

- **Website**: https://www.quantum-espresso.org
- **Repository**: https://github.com/QEF/q-e ｜ [Releases](https://github.com/QEF/q-e/releases)
- **Language / License**: Fortran / GPL-2.0
- **🎯 Usage direction**: plane-wave + pseudopotential DFT for periodic systems — standard
  calculations of **band structure, density of states, phonons (DFPT), and electron–phonon coupling**
  for solids; a common engine for materials work.
- **🔄 Update status**: 🟡 latest stable **v7.4.1** (2025-03).

## GPAW

- **Website**: https://gpaw.readthedocs.io
- **Repository**: https://gitlab.com/gpaw/gpaw
- **Language / License**: Python + C / GPL-3.0
- **🎯 Usage direction**: PAW-based DFT supporting real-space grids, plane waves, and LCAO modes;
  **deeply integrated with ASE**, ideal for scripted materials/surface calculations and
  high-throughput pipelines.
- **🔄 Update status**: 🟡 latest **v25.7.0** (2025-07-29), steady releases following ASE's cadence.

## ABINIT

- **Website**: https://www.abinit.org
- **Repository**: https://github.com/abinit/abinit ｜ [Releases](https://github.com/abinit/abinit/releases)
- **Language / License**: Fortran / GPL-3.0
- **🎯 Usage direction**: plane-wave DFT/DFPT, strong at **response properties, phonons, GW/BSE excited
  states**, and dielectric properties — suited to solids requiring accurate electronic excitations and
  optical properties.
- **🔄 Update status**: 🟡 latest **v10.6** (2026-02-07), adding DMFT, spin spirals, and ARM/GPU improvements.

## xtb (GFN-xTB)

- **Website**: https://xtb-docs.readthedocs.io
- **Repository**: https://github.com/grimme-lab/xtb ｜ [Releases](https://github.com/grimme-lab/xtb/releases)
- **Language / License**: Fortran / LGPL-3.0
- **🎯 Usage direction**: semi-empirical **extended tight-binding** methods (GFN0/1/2-xTB) that deliver
  geometry optimization, frequencies, and energies at near-force-field speed; commonly used as a
  **fast pre-processing / pre-screening** step for large systems or large batches of conformers before
  DFT refinement.
- **🔄 Update status**: 🟢 recent release adds GPU acceleration, the ALPB solvation model, and optimizer
  improvements (2026-05).
- **🔗 Ecosystem**: [CREST](https://github.com/crest-lab/crest) (xtb-based automated conformer/isomer
  sampling and reaction-network exploration).

## DFTB+

- **Website**: https://dftbplus.org
- **Repository**: https://github.com/dftbplus/dftbplus ｜ [Releases](https://github.com/dftbplus/dftbplus/releases)
- **Language / License**: Fortran / LGPL-3.0
- **🎯 Usage direction**: an implementation of density-functional tight-binding (DFTB) and xTB methods —
  **fast semi-empirical electronic structure** between DFT and classical force fields, for geometry/dynamics
  of larger systems and electronic transport.
- **🔄 Update status**: 🟡 steadily maintained with periodic releases.

---

## Also worth knowing (some not open source)

| Project | Notes |
|---------|-------|
| [ORCA](https://www.faccts.de/orca/) | Comprehensive and easy to use; **free for academia but not open source**; a common choice for DFT/correlated/excited-state methods |
| [OpenMolcas](https://gitlab.com/Molcas/OpenMolcas) | Open-source multireference methods (CASSCF/CASPT2/RASSCF) for strongly correlated systems |
| [CREST](https://github.com/crest-lab/crest) | xtb-based automated conformer sampling; used together with xtb |
| [Dalton](https://gitlab.com/dalton/dalton) | Strong at molecular properties (response theory, NMR, magnetic properties) |

[← Back to home](../README.md) ｜ [Next: Molecular Dynamics →](02-molecular-dynamics.md)
