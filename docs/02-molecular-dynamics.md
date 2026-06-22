# 02 · Molecular Dynamics

> **🌐 Language:** <kbd>[**English**](02-molecular-dynamics.md)</kbd> <kbd>[中文](zh/02-molecular-dynamics.md)</kbd>

[← Back to home](../README.md)

Classical and enhanced-sampling molecular dynamics (MD) for the dynamics, thermodynamic properties,
and free-energy calculations of biomolecules, soft matter, and materials.

> 🔄 **Update status** is as of **June 2026**. Activity: 🟢 Highly active ｜ 🟡 Steadily maintained ｜ 🟠 Slow updates.

---

## GROMACS

- **Website**: https://www.gromacs.org
- **Repository**: https://github.com/gromacs/gromacs ｜ [Downloads](https://manual.gromacs.org/current/download.html)
- **Language / License**: C++ / LGPL-2.1
- **🎯 Usage direction**: the workhorse engine for biomolecular MD — **extremely fast and very
  GPU-optimized**, widely used for proteins, nucleic acids, and membranes, and for **free-energy
  perturbation (FEP)** calculations.
- **✨ Highlights**: highly tuned kernels, a mature analysis toolchain, broad force-field support; the
  2026 series adds the AMBER14SB/19SB protein force fields and OPC/OPC3 water models, and extends
  support for **neural-network potentials (NNP)**.
- **🔄 Update status**: 🟢 latest **2026.2** (2026 series; 2026.0 released 2026-01-19). Annual majors + quarterly patches.

## LAMMPS

- **Website**: https://www.lammps.org
- **Repository**: https://github.com/lammps/lammps ｜ [Releases](https://github.com/lammps/lammps/releases)
- **Language / License**: C++ / GPL-2.0
- **🎯 Usage direction**: **large-scale parallel MD** for materials and soft matter with an enormous
  range of force fields/potentials (metals, polymers, granular, reactive ReaxFF, ML potentials, …),
  and strong extensibility and customization.
- **✨ Highlights**: modular "package" system, easy to plug in DeePMD/MACE and other ML potentials;
  command-script driven; ships a LAMMPS-GUI.
- **🔄 Update status**: 🟢 stable **22Jul2025** (update4), development/feature **30Mar2026**. Frequent updates.

## OpenMM

- **Website**: https://openmm.org
- **Repository**: https://github.com/openmm/openmm ｜ [Releases](https://github.com/openmm/openmm/releases)
- **Language / License**: C++ + Python / MIT, LGPL
- **🎯 Usage direction**: a GPU-accelerated MD **toolkit/library** with an extremely flexible Python API —
  great for custom force fields, custom integrators, and **embedding ML potentials into MD**
  ([openmm-ml](https://github.com/openmm/openmm-ml)). Often the underlying engine for other workflows
  (e.g. OpenFF, folding pipelines).
- **🔄 Update status**: 🟢 latest **v8.5.2** (2026-06-08). Active releases, supports newer Python versions.

## HOOMD-blue

- **Website**: https://hoomd-blue.readthedocs.io
- **Repository**: https://github.com/glotzerlab/hoomd-blue ｜ [Releases](https://github.com/glotzerlab/hoomd-blue/releases)
- **Language / License**: C++ + Python / BSD-3
- **🎯 Usage direction**: GPU-oriented **coarse-grained / colloidal / self-assembly** simulation,
  supporting both molecular dynamics and Monte Carlo (HPMC); Python-driven and common in soft-matter
  and nanoparticle self-assembly research.
- **🔄 Update status**: 🟢 latest **v7.0.x** (2026-04). Active releases.

## ESPResSo

- **Website**: https://espressomd.org
- **Repository**: https://github.com/espressomd/espresso ｜ [Releases](https://github.com/espressomd/espresso/releases)
- **Language / License**: C++ + Python / GPL-3.0
- **🎯 Usage direction**: **soft matter and complex fluids** (polyelectrolytes, charged colloids,
  surfactants), with lattice-Boltzmann hydrodynamic coupling and long-range electrostatics (P3M).
- **🔄 Update status**: 🟡 steadily maintained with periodic releases.

## AmberTools

- **Website**: https://ambermd.org/AmberTools.php
- **Repository**: https://github.com/Amber-MD ｜ downloads on the website
- **Language / License**: C/C++/Python / GPL and others (**open-source portion**)
- **🎯 Usage direction**: the **free, open-source** components of the Amber ecosystem — system building
  (tleap), force-field parameterization (antechamber/GAFF), **MM-PBSA/GBSA binding free energies**, and
  trajectory analysis (cpptraj/pytraj). Works alongside OpenMM/GROMACS.
- **🔄 Update status**: 🟡 annual releases (e.g. AmberTools 25). Note: the main accelerated engine (pmemd, etc.)
  **requires a paid license**; AmberTools itself is open source.

---

## Also worth knowing (some not open source)

| Project | Notes |
|---------|-------|
| [NAMD](https://www.ks.uiuc.edu/Research/namd/) | Large-system parallel MD, **free but not fully open source**; pairs well with VMD |
| [OpenFF Toolkit](https://github.com/openforcefield/openff-toolkit) | Open-source small-molecule force fields (SMIRNOFF) and parameterization tools |
| Amber (pmemd) / Desmond | Commercial / paid licenses — outside this open-source list |

[← Previous: Quantum Chemistry](01-quantum-chemistry.md) ｜ [Back to home](../README.md) ｜ [Next: ML Potentials →](03-ml-potentials.md)
