# NPTEL foundations for scientific computing, AI and simulation

[Documentation index](README.md) · [JFXLMS architecture](../README.md)

Consolidation date: 2026-10-11. Provenance: the former `NPTEL National Programme.txt`, blob `7da521df2a2030c87fc75f8512830c31d4d3605c`, retained in Git history. This English guide replaces the TXT in the current documentation. It organizes the source material; it is not an exhaustive catalog and does not confirm enrollment, certificates, instructors, institutions or syllabi for a current course session.

## Contents

- [Scientific computing](#scientific-computing)
- [Artificial intelligence and data science](#artificial-intelligence-and-data-science)
- [Simulation engineering](#simulation-engineering)
- [Consolidation with JFXLMS](#consolidation-with-jfxlms)
- [Proposed registry and indexing](#proposed-registry-and-indexing)
- [Official references](#official-references)

## Scientific computing

The source groups mathematical models, numerical analysis and high-performance computing (HPC).

| Documentation ID | Topic / original search terms | Content described in the source |
| --- | --- | --- |
| NPTEL-SC-01 | Scientific Computing / High-Performance Computing | Advanced numerical methods, computational linear algebra, ordinary and partial differential equations (ODE/PDE), parallelization with MPI, OpenMP and CUDA |
| NPTEL-SC-02 | Numerical Methods for Engineers & Scientists | Optimization, finite differences, finite elements (FEM) and curve fitting |
| NPTEL-SC-03 | Parallel Computing | Distributed programming, processor architecture and scientific algorithms on massively parallel architectures |

Referenced tools: C/C++, Fortran, Python, MPI, OpenMP and CUDA. These are source references, not installed dependencies or guaranteed tools for every course. The source attributes SC-01 to IIT Madras/IIT Kharagpur; these claims require a specific official course-page match before publication as course metadata.

## Artificial intelligence and data science

The source presents conceptual foundations, deep learning and reinforcement learning.

| Documentation ID | Topic / original search terms | Content described in the source |
| --- | --- | --- |
| NPTEL-AI-01 | Artificial Intelligence: Search Methods / Foundations | A* search, Minimax, knowledge representation, Bayesian networks and constraint satisfaction |
| NPTEL-AI-02 | Deep Learning | Convolutional neural networks (CNN), recurrent networks (RNN/LSTM), Transformers, Adam/SGD optimizers and PyTorch/TensorFlow |
| NPTEL-AI-03 | Reinforcement Learning | Markov decision processes (MDP), Q-Learning, Deep Q-Networks (DQN) and policy gradients |
| NPTEL-AI-04 | Applied AI & Computer Vision | Natural language processing (NLP), advanced computer vision and applications in finance and healthcare |

Referenced tools: Python, PyTorch, TensorFlow and Scikit-Learn. The source attributes AI-01 to IIT Delhi/IIT Madras, AI-02 to IIT Ropar/IIT Madras and AI-03 to IIT Madras. These remain source claims pending qualification against individual sessions; AI-04 groups topics rather than identifying a single course.

## Simulation engineering

The source brings together physical modeling, computational fluid dynamics and complex systems.

| Documentation ID | Topic / original search terms | Content described in the source |
| --- | --- | --- |
| NPTEL-SE-01 | Computational Fluid Dynamics (CFD) | Navier–Stokes discretization, finite volume methods (FVM), SIMPLE/PISO algorithms and turbulence modeling |
| NPTEL-SE-02 | Finite Element Method (FEM) in Engineering | Structural analysis, multiphysics, heat transfer and linear/nonlinear elements |
| NPTEL-SE-03 | Mathematical Modelling and Simulation of Chemical/Mechanical Processes | Dynamic processes, stochastic methods, Monte Carlo simulation and industrial digital twins |

Referenced tools: OpenFOAM, ANSYS/COMSOL, MATLAB and Python. The source attributes SE-01 to IIT Kanpur/IIT Kharagpur; this does not establish that all listed tools or techniques belong to one session.

## Consolidation with JFXLMS

This guide extends the academic-foundations component of the main README. It complements the existing NPTEL registry and does not duplicate the Microsoft certification, cloud, software architecture or finance pathways.

| Area | Proposed educational use | Proposed OpenTwin laboratory evidence |
| --- | --- | --- |
| Scientific computing | Numerical methods and reproducible execution | Analytic comparison, error/convergence, parameters and measured execution times |
| AI and data science | Foundations for tutoring, assessment and learning models | Synthetic or authorized datasets, reproducible splits, metrics and instructor review |
| Simulation engineering | Physical models and system coupling | Units, initial/boundary conditions, solver version and independent reference |

These evidence proposals are JFXLMS editorial additions, not official NPTEL deliverables. Enrollment and certificates remain in provider systems. An NPTEL certificate is not a Microsoft Certification. This documentation change does not implement the related laboratories or adapters.

## Proposed registry and indexing

The ten table IDs are internal documentation topic keys, not official NPTEL course codes. Each row is a unique topic entry; its original title and acronyms support lookup.

Before adding a real course to the learning-resource registry described in the README, record:

- Internal resource ID and official course URL.
- Original title, any editorial translation and material language.
- Institution, instructor, session and verification date.
- Prerequisites and objectives from the official course page.
- Session-specific access, reuse and certification conditions.
- Related competencies, proposed laboratory and evidence provenance.

This is documentation indexing. It does not implement a RAG index, search engine, course download or NPTEL synchronization. Check reuse conditions before redistributing teaching material.

## Official references

Consulted on 2026-10-11 to locate examples. Listed sessions may be archived and do not establish current enrollment availability. They are not exact equivalents of every title in the source.

- [Official NPTEL catalog](https://nptel.ac.in/courses): locate the course page and session for each resource.
- [High Performance Scientific Computing, session noc25_ma27](https://onlinecourses.nptel.ac.in/e-learning/preview/noc25_ma27): an official example related to SC-01.
- [Scientific Computing Using Python, session noc23_ph46](https://onlinecourses.nptel.ac.in/noc23_ph46/preview): an example related to scientific computing.
- [Applied Computational Fluid Dynamics, course 101104450](https://nptel.ac.in/courses/101104450): an example related to SE-01.
- [Computational Fluid Dynamics, course 112105045](https://nptel.ac.in/courses/112105045): an additional reference for SE-01.
