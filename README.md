# Optimal Control Software Repository

Welcome to the **Optimal Control Software Repository**, a curated collection of tools and software packages for optimization and control. These tools support a wide range of applications, including model predictive control, dynamic optimization, embedded solvers, and systems with nonsmooth dynamics.

Before diving into the list, consider exploring the [**PLATO Optimization Software Guide**](https://plato.asu.edu/guide.html) — a decision tree resource that helps identify appropriate software for your optimization problem. Maintained by Arizona State University, PLATO categorizes both public domain and open academic tools, with emphasis on problem classes and licensing. It is especially helpful if you’re unsure which solver or package is right for your need

---

## **Current Software**

### [acados](https://github.com/acados/acados)
**Keywords**: Fast and embedded solvers, nonlinear optimal control, model predictive control.

acados provides efficient solutions for optimal control and estimation problems. Key features include:
- Modules for ODE and DAE integration.
- Interfaces to advanced QP solvers like HPIPM, qpOASES, DAQP, qpDUNES, and OSQP.
- Nonlinear programming solvers using the real-time iteration framework.
- Python, MATLAB, and Octave interfaces.

Learn more on the [official documentation page](https://docs.acados.org/).

---

### [nosnoc](https://github.com/nurkanovic/nosnoc)
**Keywords**: Nonsmooth dynamics, state jumps, optimal control.

nosnoc specializes in solving optimal control problems for systems with nonsmooth dynamics, such as switches and state jumps. Highlights:
- Automatic discretization with the FESD method for high accuracy.
- Support for Filippov systems and time-freezing formulations.
- Solves Mathematical Programs with Complementarity Constraints (MPCCs).

Find tutorials and examples on the [official website](https://www.syscop.de/research/software/nosnoc).

---

### [HPIPM](https://github.com/giaf/hpipm)
**Keywords**: High-performance QP solvers, interior-point methods.

HPIPM is a high-performance solver for convex quadratic programs tailored to embedded optimization. It leverages the BLASFEO library for efficient computation. Key applications include model predictive control and tree-structured QPs.

Visit the [HPIPM GitHub repository](https://github.com/giaf/hpipm) for installation and examples.

---

### [TuneMPC](https://github.com/jdeschut/tunempc)
**Keywords**: Economic tuning, nonlinear MPC.

TuneMPC is a Python package that enables economic tuning of nonlinear model predictive control problems, optimizing tracking schemes for equivalence with economic NMPC.

Explore the tool on its [GitHub repository](https://github.com/jdeschut/tunempc).

---

### [AWEbox](https://github.com/awebox/awebox)
**Keywords**: Airborne wind energy, optimal control.

AWEbox is an open-source Python toolbox for modeling and optimizing airborne wind energy systems. It supports:
- Single- and multi-drone systems.
- User-defined 3D wind profiles.
- Homotopy strategies for robustness.

Get started on the [AWEbox GitHub repository](https://github.com/awebox/awebox).

---

### [CasADi](https://github.com/casadi/casadi)
**Keywords**: Symbolic differentiation, dynamic optimization.

CasADi is a powerful framework for algorithmic differentiation and numeric optimization, particularly suited for dynamic optimization. Features include:
- Collocation and shooting-based approaches for ODE/DAE integration.
- Efficient computation of derivatives for NLP solvers.

Access tutorials and documentation on the [CasADi webpage](https://web.casadi.org/).

For a extensive list of projects based on CasADi, refer to [best-of-casadi](https://github.com/brunoml5/best-of-casadi) or [promo](https://github.com/casadi/promo).

---

### [BLASFEO](https://github.com/giaf/blasfeo)
**Keywords**: Linear algebra, high-performance computing.

BLASFEO provides optimized linear algebra routines for matrices of moderate size, outperforming other BLAS implementations in embedded optimization contexts.

Visit the [BLASFEO GitHub repository](https://github.com/giaf/blasfeo) for installation and benchmarks.

---

### [LCQPow](https://github.com/hallfjonas/LCQPow)
**Keywords**: Quadratic programs, complementarity constraints.

LCQPow is an open-source solver for quadratic programs with linear complementarity constraints, utilizing a penalty homotopy approach. The methodology is detailed in [this paper](https://ieeexplore.ieee.org/abstract/document/9439931).

Explore examples and installation instructions on the [LCQPow GitHub repository](https://github.com/hallfjonas/LCQPow).

---

## **Past Software Developments (possibly not maintained anymore)**

### [qpOASES](https://github.com/coin-or/qpOASES)
**Keywords**: Quadratic programming

qpOASES is an open-source C++ implementation of the recently proposed online active set strategy, which was inspired by important observations from the field of parametric quadratic programming (QP). It has several theoretical features that make it particularly suited for model predictive control (MPC) applications.

For further information and installation intstructions visit the [qpOASES webpage](https://projects.coin-or.org/qpOASES).

---

### [tmpc](https://github.com/mkatliar/tmpc)
**Keywords**: Optimal Control, SQP

tmpc is a C++ library for Model Predictive Control

The source code is publicly available on https://gitlab.syscop.de/mikhail.katliar/tmpc/-/tree/master

---

### [casiopeia](https://github.com/adbuerger/casiopeia)
**Keywords**: Parameter Estimation, Experimental Design

casiopeia holds a user-friendly environment for optimum experimental design and parameter estimation and identification applications. It does so by providing Python classes that can be initialized with the problem specifications, while the computations can then easily be performed using the available class functions.

Please note: casiopeia makes use of the optimization framework [CasADi](http://www.casadi.org/). For casiopeia to work, you need CasADi version = 3.1.0 to be installed on your system, otherwise the installation of casiopeia will abort.

casiopeia is still in it's testing state, and does not yet contain all the features it will provide in future versions. Therefore, you should check for updates on a regular basis.

For an installation guide, a tutorial on how to use casiopeia and a detailed documentation, please visit the [manual pages](http://casiopeia.readthedocs.io/).

---

### [ACADO Toolkit](https://github.com/acado/acado)
**Keywords**: Nonlinear Optimal Control, Model Predictive Control, Code Generation

NOTE: ACADO Toolkit is not maintained anymore. We recommend using acados instead, which offers similar functionalites.
 
[ACADO Toolkit](https://acado.github.io/) is a software environment and algorithm collection for automatic control and dynamic optimization. It provides a general framework for using a great variety of algorithms for direct optimal control, including model predictive control, state and parameter estimation and robust optimization. ACADO Toolkit is implemented as self-contained C++ code and comes along with user-friendly [MATLAB interface](http://acado.github.io/matlab_overview.html). The object-oriented design allows for convenient coupling of existing optimization packages and for extending it with user-written optimization routines.

For an installation guide, tutorial examples and a detailed documentation, please visit the [ACADO Toolkit webpage](http://acado.github.io/index.html).In addition, user questions can be posted on [our sourceforge forum](https://sourceforge.net/p/acado/discussion/) while the codebase itself is hosted on our github page.

---

### [Open Optimal Control Library (OpenOCL)](https://github.com/OpenOCL/OpenOCL)
**Keywords**: Modeling, Optimal Control, Trajectory Optimization

OpenOCL is a software-toolbox written in Matlab for modeling optimal control and trajectory optimization problems. It interfaces Ipopt to solve the optimal control problems numerically, and calculates the necessary derivatives by automatic differentiation using CasADi. It implements direct methods to optimal control (collocation/pseudo-spectral methods).

Visit the project website to get more information and download the software: https://openocl.org

---

### [Optidef](https://github.com/jeslago/optidef)
**Keywords**: Latex Package

A small li­brary that pro­vides a stan­dard set of en­vi­ron­ments for writ­ing op­ti­miza­tion prob­lems in Latex. You can find the official repository in ctan and the last updated version in github.

Usage
If you update your TeX packages ([instructions here](http://tex.stackexchange.com/questions/55437/how-do-i-update-my-tex-distribution)), you can simply use it by adding to the preamble of your document:

\usepackage{optidef}

If you do not want to update your packages, just download the package from ctan and add it to your project path.

Documentation
[optidef.pdf](https://www.syscop.de/files/users/Jesus.lago/optidef.pdf)

---

## [CVXPY](https://www.cvxpy.org)

**Keywords**: Convex optimization, modeling language, mixed integer convex programs

CVXPY is a Python embedded language for expressing convex optimization problems in a natural mathematical form. It supports

* Linear, quadratic, conic, and semidefinite programs
* Geometric and quasiconvex programs
* Mixed integer convex models
* GPU acceleration beginning in version 1.7
* Solvers such as OSQP, SCS, and Clarabel

Website: [https://www.cvxpy.org](https://www.cvxpy.org)

---

## [Fatrop](https://github.com/meco-group/fatrop)

**Keywords**: Nonlinear programming, real time optimization, interior point methods

Fatrop is a constrained nonlinear optimal control problem solver that is fast and achieves a high numerical robustness.

The main features of the solver are:

high numerical robustness thanks to advanced numerical optimization techniques, inspired by Ipopt
fast by exploiting the optimal control problem structure through a specialized linear solver, based on a generalized Riccati recursion
high performance linear algebra through integration of BLASFEO
effective handling of path equality and inequality constraints, without relying on penalty methods
ability to incorporate exact Lagrangian Hessian information
ability to be initialized from any, possibly infeasible, solution estimate

Repository: [https://github.com/meco-group/fatrop](https://github.com/meco-group/fatrop)

---

## MadNLP

**Keywords**: Interior point methods, large scale nonlinear programming, Julia

MadNLP is a nonlinear programming solver written in Julia. It features a modern interior point method that exploits sparsity and supports automatic differentiation through the Julia ecosystem. It integrates well with modeling tools like JuMP.

Repository: [https://github.com/MadNLP/MadNLP.jl](https://github.com/MadNLP/MadNLP.jl)

---

## OpEn

**Keywords**: Operator splitting, embedded optimization, MPC

OpEn is a toolkit for generating fast tailored solvers for optimal control and embedded decision making. It uses proximal splitting methods and produces C code suitable for real time systems. The Python interface is casadi based and supports parametric MPC problems.

Repository: [https://github.com/alphaville/optimization-engine](https://github.com/alphaville/optimization-engine)

---

## DoMPC

**Keywords**: Nonlinear MPC, Python, simulation and control

DoMPC is a Python framework that simplifies the setup of nonlinear model predictive controllers. It offers

* Direct multiple shooting
* Integrators and discretization tools
* Simulation and closed loop control modules

Repository: [https://github.com/do-mpc/do-mpc](https://github.com/do-mpc/do-mpc)

---

## JAXopt

**Keywords**: Auto differentiation, first order methods, JAX optimization

JAXopt is a library of gradient based and projection based optimization algorithms that run on CPU, GPU, or TPU. It supports

* First order solvers
* Fixed point iterations
* Implicit differentiation
* JIT compilation via JAX

Repository: [https://github.com/google/jaxopt](https://github.com/google/jaxopt)

---

## Diffrax

**Keywords**: Differentiable ODE solvers, JAX, neural ODEs

Diffrax provides a large collection of numerical integrators for ordinary differential equations fully compatible with JAX autodiff and JIT compilation. It supports event handling, adaptive step solvers, and implicit integrators, making it suitable for scientific computing and machine learning.

Repository: [https://github.com/patrick-kidger/diffrax](https://github.com/patrick-kidger/diffrax)

---

## **Contributions**

If you have suggestions or would like to contribute a new tool, feel free to open a pull request or an issue. This repository aims to grow with the optimization and control community!

---

## **License**

Each software package is maintained by its respective authors and teams. Please refer to the individual repositories for licensing details.
