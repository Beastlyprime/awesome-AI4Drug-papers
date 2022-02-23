# Awesome-AI4Drug-Papers

A collection of AI for Drug Design related papers and corresponding code sources (in progress).

-------------

## Molecule

### Molecule Generation

- NeurIPS (2021) [Hit and Lead Discovery with Explorative RL and Fragment-based Molecule Generation](https://proceedings.neurips.cc/paper/2021/hash/41da609c519d77b29be442f8c1105647-Abstract.html). A novel RL framework that generates pharmacochemically acceptable molecules with large docking scores.
- ICLR oral (2022) [Data-Efficient Graph Grammar Learning for Molecular Generation ](https://openreview.net/forum?id=l4IHywGq6a). A data-efficient generative model that can be learned from datasets with orders of magnitude smaller sizes than common benchmarks. 
- ICLR spotlight (2022) [Spanning Tree-based Graph Generation for Molecules ](https://openreview.net/forum?id=w60btE_8T2m). Formulating molecular graph generation as a construction of a spanning tree and the residual edges. 
- ICLR spotlight (2022) [Amortized Tree Generation for Bottom-up Synthesis Planning and Synthesizable Molecular Design ](https://openreview.net/forum?id=FRxhHdnxt1). Demonstrating the potential to solve both problems of design and synthesis simultaneously.
- ICLR (2022) [Learning to Extend Molecular Scaffolds with Structural Motifs ](https://openreview.net/forum?id=ZTsoE8G3GG). A new fragment-based generative model of molecules that can be constrained to include an arbitrary subgraph (scaffold).
- ICLR (2022) [Differentiable Scaffolding Tree for Molecule Optimization ](https://openreview.net/forum?id=w_drCosT76). Make the molecular optimization problem differentiable at the structure level.
- ICLR (2022) [Top-N: Equivariant Set and Graph Generation without Exchangeability ](https://openreview.net/forum?id=-Gk_IPJWvk). Top-n can replace i.i.d. generation in any VAE or GAN -- it is easier to train and better captures complex dependencies in the data.
- ICLR (2022) [Multi-objective Optimization by Learning Space Partition ](https://openreview.net/forum?id=FlwzVjfMryn). LaMOO substantially outperforms strong baselines on multiple real-world MOO tasks, by up to 225% in sample efficiency for neural architecture search on Nasbench201, and up to 10% for molecular design.
- ICLR (2022) [Spatial Graph Attention and Curiosity-driven Policy for Antiviral Drug Discovery ](https://openreview.net/forum?id=kavTY__jxp).  All reviewers are convinced about the novelty of the proposed method. They all appreciate the attempt to attack COVID-19 using machine learning.
- ICLR (2022) [An Autoregressive Flow Model for 3D Molecular Geometry Generation from Scratch ](https://openreview.net/forum?id=C03Ajc-NS5W).  3D molecular geometry generation from scratch.

### Ensembles Generation

- NeurIPS (2021) [GeoMol: Torsional Geometric Generation of Molecular 3D Conformer Ensembles](https://proceedings.neurips.cc/paper/2021/hash/725215ed82ab6306919b485b81ff9615-Abstract.html). Prediction of a molecule's 3D conformer ensemble from the molecular graph holds a key role in areas of cheminformatics and drug discovery. 

### Property Prediction

- NeurIPS (2021) [Property-Aware Relation Networks for Few-Shot Molecular Property Prediction](https://proceedings.neurips.cc/paper/2021/hash/91bc333f6967019ac47b49ca0f2fa757-Abstract.html). Molecular property prediction is essentially a few-shot problem which makes it hard to use regular machine learning models.
- NeurIPS (2021) [Motif-based Graph Self-Supervised Learning for Molecular Property Prediction](https://proceedings.neurips.cc/paper/2021/hash/85267d349a5e647ff0a9edcb5ffd1e02-Abstract.html). Most existing self-supervised pretraining frameworks for GNNs only focus on node-level or graph-level tasks. These approaches cannot capture the rich information in subgraphs or graph motifs.
- NeurIPS (2021) [Deep Molecular Representation Learning via Fusing Physical and Chemical Information](https://proceedings.neurips.cc/paper/2021/hash/884d247c6f65a96a7da4d1105d584ddd-Abstract.html). Two networks specialize in their own tasks and cooperate by providing expertise to each other.
- ICLR oral (2022) [Meta-Learning with Fewer Tasks through Task Interpolation ](https://openreview.net/forum?id=ajXWF7bVR8d).  The bottleneck of current meta-learning algorithms is the requirement of a large number of meta-training tasks, which may not be accessible in real-world scenarios.
- ICLR (2022) [Constrained Graph Mechanics Networks ](https://openreview.net/forum?id=SHbhHHfePhP). Can be used for molecular dynamics prediction.

####  Physics Properties

- NeurIPS (2021) [SE(3)-equivariant prediction of molecular wavefunctions and electronic densities](https://proceedings.neurips.cc/paper/2021/hash/78f1893678afbeaa90b1fa01b9cfb860-Abstract.html) Introduce general SE(3)-equivariant operations and building blocks for constructing deep learning architectures for geometric point cloud data and apply them to reconstruct wavefunctions of atomistic systems with unprecedented accuracy. 
- ICLR spotlight (2022) [Equivariant Transformers for Neural Network based Molecular Potentials ](https://openreview.net/forum?id=zNHzqZ9wrRB). A novel equivariant Transformer architecture for the prediction of molecular potentials and provide insights into the molecular representation through extensive analysis of the model's attention weights. Highlight the importance of datasets including off-equilibrium conformations for the evaluation of molecular potentials.
- ICLR spotlight (2022) [Ab-Initio Potential Energy Surfaces by Pairing GNNs with Neural Wave Functions ](https://openreview.net/forum?id=apv504XsysP). A new network architecture that solves the Schrödinger equation for multiple geometries simultaneously.
- ICLR (2022) [Simple GNN Regularisation for 3D Molecular Property Prediction and Beyond ](https://openreview.net/forum?id=1wVvweK3oIb).   Adding node-label noise to a GNN. There is little technical novelty. The proposed applications of the approach are interesting.

### Representation Learning

- NeurIPS (2021) [Directional Message Passing on Molecular Graphs via Synthetic Coordinates](https://proceedings.neurips.cc/paper/2021/hash/82489c9737cc245530c7a6ebef3753ec-Abstract.html). Propose synthetic coordinates that enable the use of advanced GNNs without requiring the true molecular configuration.
- NeurIPS (2021) [GemNet: Universal Directional Graph Neural Networks for Molecules](https://proceedings.neurips.cc/paper/2021/hash/35cf8659cfcb13224cbd47863a34fc58-Abstract.html).  We show that GNNs with directed edge embeddings and two-hop message passing are indeed universal approximators for predictions that are invariant to translation, and equivariant to permutation and rotation. 
- ICLR (2022) [Learning 3D Representations of Molecular Chirality with Invariance to Bond Rotations ](https://openreview.net/forum?id=hm2tNDdgaFK). A method of processing the 3D torsion angles of a molecular conformer to learn tetrahedral chirality while integrating a novel invariance to rotations about internal molecular bonds directly into the model architecture.
- ICLR (2022) [A Program to Build E(N)-Equivariant Steerable CNNs](https://openreview.net/forum?id=WE4qe9xlnQw).  A general method to build G-steerable kernel spaces for equivariant steerable CNNs.
- ICLR spotlight (2022) [Geometric and Physical Quantities improve E(3) Equivariant Message Passing ](https://openreview.net/forum?id=_xwr8gOBeV1). Generalise equivariant graph networks such that node and edge updates are able to leverage covariant information.
- ICLR (2022) [Chemical-Reaction-Aware Molecule Representation Learning ](https://openreview.net/forum?id=6sh3pIzKS-). Make use of chemical reactions to improve the generalization ability of learned molecule embeddings
- ICLR (2022) [Pre-training Molecular Graph Representation with 3D Geometry ](https://openreview.net/forum?id=xQUe1pOKPam). A new SSL framework to make 3D geomety information helpful for 2D representation, in terms of the downstream tasks with 2D info only.
- ICLR (2022) [Spherical Message Passing for 3D Molecular Graphs ](https://openreview.net/forum?id=givsRXsOt9r). Incorporating torsion information when representing 3D molecules is novel and helpful.
- ICLR (2022) [MoReL: Multi-omics Relational Learning ](https://openreview.net/forum?id=DnG75_KyHjX). Multi-omics data analysis has the potential to discover hidden molecular interactions, revealing potential regulatory and/or signal transduction pathways for cellular processes of interest when studying life and disease systems. 
- ICLR (2022) [Graph Neural Networks with Learnable Structural and Positional Representations ](https://openreview.net/forum?id=wTTjnvGphYj). This work adds the positional encoding (akin to those in transformers, but adapted) to GNNs.

## Protein

### Design

- ICLR spotlight (2022) [Iterative Refinement Graph Neural Network for Antibody Sequence-Structure Co-design ](https://openreview.net/forum?id=LI2bhrE_2A). The reviewers are in agreement that the problem is one of importance, and that the technical and empirical contributions are strong. There are concerns over the relevance of evaluating the method by using a predictive model as ground truth. Still, the overall contributions remain.
- ICLR (2022) [Maximum n-times Coverage for Vaccine Design ](https://openreview.net/forum?id=ULfq0qR25dY). The results are used to produce a panstrain COVID vaccine. 

### Representation Learning

- NeurIPS (2021) [Multi-Scale Representation Learning on Proteins](https://proceedings.neurips.cc/paper/2021/hash/d494020ff8ec181ef98ed97ac3f25453-Abstract.html). A multi-scale graph construction of a protein.
- ICLR (2022) [OntoProtein: Protein Pretraining With Gene Ontology Embedding ](https://openreview.net/forum?id=yfe1VMYAXa4). A general framework to integrate knowledge graph (gene ontology) into protein pre-training. 

### Function Prediction

- NeurIPS (2021) [Language models enable zero-shot prediction of the effects of mutations on protein function](https://proceedings.neurips.cc/paper/2021/hash/f51338d736f95dd42427296047067694-Abstract.html). Modeling the effect of sequence variation on function is a fundamental problem for understanding and designing proteins.

### Contact Prediction / Docking

- NeurIPS (2021) [Co-evolution Transformer for Protein Contact Prediction](https://proceedings.neurips.cc/paper/2021/hash/770f8e448d07586afbf77bb59f698587-Abstract.html). Protein contact prediction (PCP) is an essential building block of many protein structure related applications.
- ICLR (2022) [Geometric Transformers for Protein Interface Contact Prediction ](https://openreview.net/forum?id=CS4463zx6Hi). A geometry-evolving graph transformer for 3D protein structures.

- ICLR spotlight (2022) [Independent SE(3)-Equivariant Models for End-to-End Rigid Protein Docking ](https://openreview.net/forum?id=GQjaI9mLet). Guarantees the same resulting protein complex independent of the initial placement of the two 3D structures.

