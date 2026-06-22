# 05 · Cheminformatics

> **🌐 Language:** <kbd>[**English**](05-cheminformatics.md)</kbd> <kbd>[中文](zh/05-cheminformatics.md)</kbd>

[← Back to home](../README.md)

Molecular representation, reading/writing and format conversion, descriptor/fingerprint generation,
substructure matching, conformer generation, and chemical feature engineering for machine learning.

> 🔄 **Update status** is as of **June 2026**. Activity: 🟢 Highly active ｜ 🟡 Steadily maintained ｜ 🟠 Slow updates.

---

## RDKit

- **Website**: https://www.rdkit.org
- **Repository**: https://github.com/rdkit/rdkit ｜ [Releases](https://github.com/rdkit/rdkit/releases)
- **Language / License**: C++ + Python / BSD-3
- **🎯 Usage direction**: the **de facto standard** cheminformatics library. It covers molecular I/O
  (SMILES/SMARTS/Mol/SDF), **fingerprints and descriptors** (Morgan/ECFP, MACCS, physicochemical properties),
  substructure search, **conformer generation (ETKDG)**, molecular alignment, reaction handling, similarity, and
  feature preparation for QSAR/ML.
- **✨ Highlights**: mature, stable, well-documented; the base dependency for almost every drug-discovery / chemical
  ML pipeline; integrates with Pandas (PandasTools).
- **🔄 Update status**: 🟢 latest **2026.03.3** (2026-06-05). Quarterly releases (YYYY.MM.patch), very actively maintained.

## Open Babel

- **Website**: https://openbabel.org
- **Repository**: https://github.com/openbabel/openbabel ｜ [Releases](https://github.com/openbabel/openbabel/releases)
- **Language / License**: C++ / GPL-2.0
- **🎯 Usage direction**: the Swiss-army knife of chemical **file-format conversion** and interoperability,
  supporting **110+ formats** (e.g. PDB↔PDBQT↔MOL2↔SMILES) plus command-line/library features such as adding
  hydrogens, generating 3D coordinates, and simple force-field optimization; common in ligand preparation before docking.
- **🔄 Update status**: 🟠 stable but slow; main version **3.1.1** (2020), mostly minor maintenance.

## DeepChem

- **Website**: https://deepchem.io
- **Repository**: https://github.com/deepchem/deepchem ｜ [Releases](https://github.com/deepchem/deepchem/releases)
- **Language / License**: Python / MIT
- **🎯 Usage direction**: a deep-learning toolbox for **drug discovery, materials, quantum chemistry, and biology**,
  providing many built-in datasets (MoleculeNet), featurization methods, model baselines (graph neural networks,
  sequence models, …), and end-to-end examples — good for quickly building chemical/life-science ML baselines.
- **🔄 Update status**: 🟢 actively maintained, continually expanding model and data support.

---

## Also worth knowing

| Project | Notes |
|---------|-------|
| [Chemprop](https://github.com/chemprop/chemprop) | Molecular property prediction via message-passing neural networks (D-MPNN); popular in industry |
| [datamol](https://github.com/datamol-io/datamol) | A high-level, ergonomic wrapper around RDKit that simplifies common cheminformatics operations |
| [scikit-mol](https://github.com/EBjerrum/scikit-mol) | Brings RDKit featurization into scikit-learn pipelines |
| [Indigo](https://github.com/epam/Indigo) | Another cheminformatics toolkit and rendering library (EPAM) |

[← Previous: Materials Workflows](04-materials-workflows.md) ｜ [Back to home](../README.md) ｜ [Next: Docking & Drug Design →](06-docking-drug-design.md)
