# Optimal Control Software Repository

Welcome to the **Optimal Control Software Repository**, a curated collection of tools and software packages for optimization and control. These tools cover a variety of needs, from solving optimal control problems for embedded systems to handling nonsmooth dynamical systems, model predictive control, and more.

This repository is structured to help users quickly locate the most suitable tools for their projects and includes installation instructions, links to documentation, and source code for each software package.

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

## **Contributions**

If you have suggestions or would like to contribute a new tool, feel free to open a pull request or an issue. This repository aims to grow with the optimization and control community!

---

## **License**

Each software package is maintained by its respective authors and teams. Please refer to the individual repositories for licensing details.
