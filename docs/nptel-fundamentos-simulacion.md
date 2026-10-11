# NPTEL: fundamentos para computación científica, IA y simulación

[Índice documental](README.md) · [Arquitectura JFXLMS](../README.md) · [TXT fuente](NPTEL%20National%20Programme.txt)

Fecha de consolidación: 2026-10-11. Fuente: `NPTEL National Programme.txt`, blob `7da521df2a2030c87fc75f8512830c31d4d3605c`. El TXT se conserva íntegro como antecedente. Esta guía traduce los títulos y organiza su contenido; no es un catálogo exhaustivo ni confirma matrículas, certificados, docentes, instituciones o temarios de una edición vigente.

## Índice

- [Computación científica](#computacion-cientifica)
- [Inteligencia artificial y ciencia de datos](#inteligencia-artificial-y-ciencia-de-datos)
- [Ingeniería de simulación](#ingenieria-de-simulacion)
- [Consolidación con JFXLMS](#consolidacion-con-jfxlms)
- [Registro e indexación propuestos](#registro-e-indexacion-propuestos)
- [Referencias oficiales](#referencias-oficiales)
- [English consolidated summary](#english-consolidated-summary)

<a id="computacion-cientifica"></a>
## Computación científica

El TXT agrupa modelos matemáticos, análisis numérico y programación de alto rendimiento (HPC).

| ID documental | Traducción al español | Nombre original / términos de búsqueda | Contenido descrito en el TXT |
| --- | --- | --- | --- |
| NPTEL-SC-01 | Computación científica / computación de alto rendimiento | Scientific Computing / High-Performance Computing | Métodos numéricos avanzados, álgebra lineal computacional, ecuaciones diferenciales ordinarias y parciales (ODE/PDE), paralelización con MPI, OpenMP y CUDA |
| NPTEL-SC-02 | Métodos numéricos para ingenieros y científicos | Numerical Methods for Engineers & Scientists | Optimización, diferencias finitas, elementos finitos (FEM) y ajuste de curvas |
| NPTEL-SC-03 | Computación paralela | Parallel Computing | Programación distribuida, arquitectura de procesadores y algoritmos científicos en arquitecturas masivamente paralelas |

Herramientas mencionadas: C/C++, Fortran, Python, MPI, OpenMP y CUDA. Son referencias del texto, no dependencias instaladas ni herramientas garantizadas de todos los cursos. Las atribuciones del TXT a IIT Madras/IIT Kharagpur para SC-01 requieren vincularse a una ficha oficial concreta antes de publicarse como metadatos de un curso.

<a id="inteligencia-artificial-y-ciencia-de-datos"></a>
## Inteligencia artificial y ciencia de datos

El TXT presenta fundamentos conceptuales, aprendizaje profundo y aprendizaje por refuerzo.

| ID documental | Traducción al español | Nombre original / términos de búsqueda | Contenido descrito en el TXT |
| --- | --- | --- | --- |
| NPTEL-AI-01 | Inteligencia artificial: métodos de búsqueda y fundamentos | Artificial Intelligence: Search Methods / Foundations | Búsqueda A*, Minimax, representación del conocimiento, redes bayesianas y satisfacción de restricciones |
| NPTEL-AI-02 | Aprendizaje profundo | Deep Learning | Redes convolucionales (CNN), recurrentes (RNN/LSTM), Transformers, optimizadores Adam/SGD y PyTorch/TensorFlow |
| NPTEL-AI-03 | Aprendizaje por refuerzo | Reinforcement Learning | Procesos de decisión de Markov (MDP), Q-Learning, redes Q profundas (DQN) y gradientes de política |
| NPTEL-AI-04 | IA aplicada y visión por computador | Applied AI & Computer Vision | Procesamiento del lenguaje natural (NLP), visión avanzada y aplicaciones a finanzas y salud |

Herramientas mencionadas: Python, PyTorch, TensorFlow y Scikit-Learn. El TXT atribuye AI-01 a IIT Delhi/IIT Madras, AI-02 a IIT Ropar/IIT Madras y AI-03 a IIT Madras. Estas atribuciones se conservan como afirmaciones de la fuente pendientes de correspondencia con cada edición; AI-04 agrupa temas y no identifica un curso único.

<a id="ingenieria-de-simulacion"></a>
## Ingeniería de simulación

El TXT reúne modelado físico, dinámica de fluidos computacional y sistemas complejos.

| ID documental | Traducción al español | Nombre original / términos de búsqueda | Contenido descrito en el TXT |
| --- | --- | --- | --- |
| NPTEL-SE-01 | Dinámica de fluidos computacional | Computational Fluid Dynamics (CFD) | Discretización de Navier–Stokes, volumen finito (FVM), SIMPLE/PISO y turbulencia |
| NPTEL-SE-02 | Método de elementos finitos en ingeniería | Finite Element Method (FEM) in Engineering | Análisis estructural, multifísica, transferencia de calor y elementos lineales/no lineales |
| NPTEL-SE-03 | Modelado matemático y simulación de procesos químicos y mecánicos | Mathematical Modelling and Simulation of Chemical/Mechanical Processes | Procesos dinámicos, métodos estocásticos, Monte Carlo y gemelos digitales industriales |

Herramientas mencionadas: OpenFOAM, ANSYS/COMSOL, MATLAB y Python. La atribución SE-01 a IIT Kanpur/IIT Kharagpur procede del TXT; no establece que todas las herramientas o técnicas enumeradas pertenezcan a una misma edición.

<a id="consolidacion-con-jfxlms"></a>
## Consolidación con JFXLMS

Este documento amplía el componente de fundamentos académicos del README. No sustituye el registro NPTEL existente ni duplica las rutas de certificación Microsoft, nube, arquitectura de software o finanzas.

| Área | Uso educativo propuesto | Evidencia propuesta de laboratorio OpenTwin |
| --- | --- | --- |
| Computación científica | Fundamentos de cálculo numérico y ejecución reproducible | Comparación con solución analítica, error/convergencia, parámetros y tiempos medidos |
| IA y ciencia de datos | Fundamentos para tutoría, evaluación y modelos de aprendizaje | Datos sintéticos o autorizados, particiones reproducibles, métricas y revisión docente |
| Ingeniería de simulación | Fundamentos de modelos físicos y acoplamiento | Unidades, condiciones iniciales/de frontera, versión del solver y referencia independiente |

Las evidencias anteriores son propuestas editoriales de JFXLMS, no entregables oficiales de NPTEL. La inscripción y los certificados permanecen en los sistemas del proveedor. Un certificado NPTEL no equivale a una certificación Microsoft. Los laboratorios y adaptadores aquí relacionados no están implementados por este cambio documental.

<a id="registro-e-indexacion-propuestos"></a>
## Registro e indexación propuestos

Los diez IDs de las tablas son claves de temas en esta documentación, no códigos oficiales NPTEL. Cada fila constituye una entrada única; la búsqueda admite tanto el título traducido como el nombre original y sus siglas.

Antes de incorporar un curso real al registro de recursos del README, completar:

- ID interno del recurso y URL oficial del curso.
- Título original, traducción editorial e idioma del material.
- Institución, docente, edición/sesión y fecha de consulta.
- Prerrequisitos y objetivos tomados de la ficha oficial.
- Condiciones de acceso, reutilización y certificación de esa edición.
- Competencias relacionadas, laboratorio propuesto y procedencia de la evidencia.

Esta indexación es documental: no implica que exista un índice RAG, motor de búsqueda, descarga de cursos o sincronización con NPTEL. No redistribuir material docente sin comprobar sus condiciones de reutilización.

<a id="referencias-oficiales"></a>
## Referencias oficiales

Consultadas el 2026-10-11 para localizar ejemplos; las sesiones indicadas pueden estar archivadas y no prueban disponibilidad actual de matrícula. No se tratan como equivalencias exactas de todos los títulos del TXT.

- [Catálogo oficial NPTEL](https://nptel.ac.in/courses): localizar la ficha y sesión de cada curso.
- [High Performance Scientific Computing, sesión noc25_ma27](https://onlinecourses.nptel.ac.in/e-learning/preview/noc25_ma27): ejemplo oficial relacionado con SC-01.
- [Scientific Computing Using Python, sesión noc23_ph46](https://onlinecourses.nptel.ac.in/noc23_ph46/preview): ejemplo relacionado con computación científica.
- [Applied Computational Fluid Dynamics, ficha 101104450](https://nptel.ac.in/courses/101104450): ejemplo relacionado con SE-01.
- [Computational Fluid Dynamics, ficha 112105045](https://nptel.ac.in/courses/112105045): referencia adicional para SE-01.

<a id="english-consolidated-summary"></a>
## English consolidated summary

The source TXT is already mostly Spanish. This companion organizes it into ten topic records and translates its English headings while retaining searchable original titles. The records cover scientific/high-performance computing, numerical methods, parallel computing, AI search and foundations, deep learning, reinforcement learning, applied AI/computer vision, CFD, FEM and chemical/mechanical process simulation.

The source describes numerical linear algebra, ODE/PDE methods, optimization, finite differences/elements, curve fitting and distributed algorithms; AI search, knowledge representation, Bayesian networks, constraints, CNN/RNN/LSTM/Transformers, Adam/SGD, MDPs, Q-learning, DQN and policy gradients; and Navier–Stokes discretization, finite volumes, SIMPLE/PISO, turbulence, structural/thermal/multiphysics analysis, stochastic methods, Monte Carlo and industrial digital twins.

Its tool lists include C/C++, Fortran, Python, MPI, OpenMP, CUDA, PyTorch, TensorFlow, Scikit-Learn, OpenFOAM, ANSYS/COMSOL and MATLAB. They are source references, not installed JFXLMS dependencies or guaranteed course syllabi. Institution and session assignments require qualification against a specific official course page.

For JFXLMS, these topics complement the existing NPTEL registry and professional-pathway architecture. Proposed OpenTwin lab evidence includes analytic comparisons and convergence, reproducible data splits and metrics, units, boundary conditions, solver versions and independent references. Provider certificates, enrollment and current sessions remain external. This documentation implements no course adapter, RAG index, simulation or credential issuance.
