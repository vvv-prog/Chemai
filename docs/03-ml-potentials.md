# 03 · Machine-Learning Potentials / Atomistic ML

> **🌐 Language:** <kbd>[**English**](03-ml-potentials.md)</kbd> <kbd>[中文](zh/03-ml-potentials.md)</kbd>

[← Back to home](../README.md)

Using machine learning to fit the potential energy surface (MLIP / NNP) to run molecular dynamics and
materials simulations at **near-DFT accuracy and near-force-field speed** over large systems and long
time scales. Recent years have brought many **universal pretrained potentials (foundation models)** that
can be used directly or fine-tuned.

> 🔄 **Update status** is as of **June 2026**. Activity: 🟢 Highly active ｜ 🟡 Steadily maintained ｜ 🟠 Slow updates.

---

## DeePMD-kit

- **Website**: https://docs.deepmodeling.com/projects/deepmd
- **Repository**: https://github.com/deepmodeling/deepmd-kit ｜ [Releases](https://github.com/deepmodeling/deepmd-kit/releases)
- **Language / License**: Python + C++ / LGPL-3.0
- **🎯 Usage direction**: **training and deployment** of Deep Potential models, integrating seamlessly with
  LAMMPS, GROMACS, ASE, etc., for high-accuracy MD of large systems (materials/liquids/catalysis).
  Provides the **DPA series of universal pretrained models**.
- **🔄 Update status**: 🟢 **v3.1.x** series; adds built-in downloadable pretrained models (e.g. **DPA3**),
  distributed training, and more optimizers. Very active (DeepModeling community).

## MACE

- **Repository**: https://github.com/ACEsuit/mace ｜ [Releases](https://github.com/ACEsuit/mace/releases)
- **Language / License**: Python / MIT
- **🎯 Usage direction**: an MLIP based on **higher-order equivariant message passing**, leading in accuracy
  and efficiency and one of the most popular equivariant GNN potentials today. Provides **universal foundation
  models** [mace-foundations](https://github.com/ACEsuit/mace-foundations) (e.g. MACE-MP, MACE-OFF, MACE-MH)
  usable out of the box across materials/molecular/surface systems.
- **🔄 Update status**: 🟢 highly active; foundation models and code iterate continuously.

## NequIP / Allegro

- **Repository**: https://github.com/mir-group/nequip ｜ [Allegro](https://github.com/mir-group/allegro)
- **Language / License**: Python / MIT
- **🎯 Usage direction**: **E(3)-equivariant graph neural network** potentials, known for being **data
  efficient** — high accuracy from a small amount of DFT data; Allegro is its **strictly local, scalable**
  variant, suited to very large systems in parallel.
- **🔄 Update status**: 🟢 actively maintained (recent updates).

## MatGL (Materials Graph Library)

- **Website**: https://matgl.ai
- **Repository**: https://github.com/materialsvirtuallab/matgl ｜ [Releases](https://github.com/materialsvirtuallab/matgl/releases)
- **Language / License**: Python / BSD-3
- **🎯 Usage direction**: a materials graph-neural-network library integrating **M3GNet, CHGNet, MEGNet,
  TensorNet, SO3Net** and more, with **universal potentials (FMMs) and property-prediction** pretrained models
  that work out of the box and can be fine-tuned. Tightly integrated with pymatgen/ASE.
- **🔄 Update status**: 🟢 latest **v2.0.0** (2025-11-13), switching to a PyG backend by default and adding the QET architecture.
- **🔗 Model notes**: **CHGNet** incorporates charge/magnetic-moment information; **M3GNet** includes three-body
  interactions; well suited to inorganic crystalline materials.

## fairchem (FAIR Chemistry)

- **Repository**: https://github.com/facebookresearch/fairchem ｜ [Releases](https://github.com/facebookresearch/fairchem/releases)
- **Language / License**: Python / MIT (some model weights under separate terms)
- **🎯 Usage direction**: Meta FAIR's chemistry machine-learning library, originating from the **Open Catalyst**
  project; provides **universal models for catalysis/materials (e.g. UMA)** and large datasets (OC20/OC22, …),
  geared toward catalyst screening and materials discovery.
- **🔄 Update status**: 🟢 highly active (still updated as of 2026-06).

## TorchANI

- **Repository**: https://github.com/aiqm/torchani ｜ [Releases](https://github.com/aiqm/torchani/releases)
- **Language / License**: Python / MIT
- **🎯 Usage direction**: the **ANI series** of neural-network potentials (focused on organic molecules, with
  ANI-1x/ANI-2x pretrained models), a PyTorch implementation that is easy to pick up for fast energies/forces
  of organic/drug-like molecules.
- **🔄 Update status**: 🟡 steadily maintained (still updated in 2025).

## SchNetPack

- **Repository**: https://github.com/atomistic-machine-learning/schnetpack ｜ [Releases](https://github.com/atomistic-machine-learning/schnetpack/releases)
- **Language / License**: Python / MIT
- **🎯 Usage direction**: an atomistic neural-network **modeling toolbox** (SchNet, PaiNN, …) with a data
  pipeline and built-in MD, suited to learning methods, research, and custom model development.
- **🔄 Update status**: 🟡 SchNetPack **2.0** series, steadily maintained.

## sGDML

- **Website**: http://www.sgdml.org
- **Repository**: https://github.com/stefanch/sGDML ｜ [Releases](https://github.com/stefanch/sGDML/releases)
- **Language / License**: Python / MIT
- **🎯 Usage direction**: **symmetric gradient-domain machine learning** (a kernel method) that reconstructs a
  **high-accuracy potential energy surface** for a single small molecule from very little data — ideal for
  accurate dynamics/spectroscopy studies (not aimed at cross-system generality).
- **🔄 Update status**: 🟠 occasional updates.

---

## Further resources

- 📊 [best-of-atomistic-machine-learning](https://github.com/JuDFTteam/best-of-atomistic-machine-learning):
  a continuously updated, popularity-ranked catalog of atomistic ML projects — a good extension of this section.
- Related: [GAP/SOAP](https://github.com/libAtoms/GAP), [n2p2](https://github.com/CompPhysVienna/n2p2),
  the NequIP/Allegro ecosystem, matsciml, and others.

[← Previous: Molecular Dynamics](02-molecular-dynamics.md) ｜ [Back to home](../README.md) ｜ [Next: Materials Workflows →](04-materials-workflows.md)
