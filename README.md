# Optimal-Control-Softwares

Software
Members of the lab develop open source software packages in the field of optimization and control. Some of the packages attracted already a larger developer community and some are maintained by previous members of the team. For each package, information and links with installation instructions can be found below, first for software packages that are actively developed or supported, and second for past software developments.


Current Software

acados
Fast and embedded solvers for nonlinear optimal control.
SQP optimal-control Model Predictive Control

acados
acados is a software package for the efficient solution of optimal control and estimation problems. It is the successor of the ACADO software package developed at KU Leuven and University of Freiburg by the team of Prof. Moritz Diehl. It provides a collection of computationally efficient building blocks tailored to optimal control and estimation problems. Among others, it implements: modules for the integration of ordinary differential equations (ODE) and differential-algebraic equations (DAE), interfaces to state-of-the-art QP solvers like HPIPM, qpOASES, DAQP, qpDUNES and OSQP, condensing routines and nonlinear programming solvers based on the real-time iteration framework. The back-end of acados uses the high-performance linear algebra package BLASFEO, in order to boost computational efficiency for small to medium scale matrices typical of embedded optimization applications. MATLAB, Octave and Python interfaces can be used to conveniently describe optimal control problems and generate self-contained C code that can be readily deployed on embedded platforms.

The documentation of acados can be found on docs.acados.org/

The source code is available on the acados github repository (https://github.com/acados/acados).


nosnoc
nosnoc (NOnSmooth Numerical Optimal Control) is a tool for numerically solving optimal control problems with nonsmooth dynamical systems with switches and/or state jumps.
optimal-control trajectory-optimization

nosnoc
nosnoc is a tool for numerically solving optimal control problems with nonsmooth dynamical systems with switches and/or state jumps. It supports:

Automatic discretization via the FESD method - high accuracy and correct sensitivities. Note that classical time-stepping methods only have first-order accuracy and wrong sensitivities even when they appear to be differentiable.

Automatic reformulations of systems with state jumps (e.g. contact problems) via time-freezing into Filippov systems/PSS. (enables high accuracy even for systems with state jumps)

Solving the nonsmooth nonlinear programs via homotopy methods. Enables the use of off-the-shelf solvers like IPOPT and SNOPT.

nosnoc relies on the recently introduced Finite Elements with Switch Detection (FESD) which enables high accuracy optimal control of systems with switches and jumps. It enables the treatment of a broad class of nonsmooth systems in a unified way.

nosnoc offers several ways to treat switched systems, piecewise smooth systems, Filippov systems, hybrid systems, rigid body models with impacts and friction in simulation, and optimal control. It discretizes a Dynamic Complementarity System (DCS) with the FESD method and solves the resulting mathematical program with complementarity constraints (MPCCs). The MPCCs are solved in a homotopy loop with a standard solver like IPOPT or SNOPT. The user may directly provide a DCS or define the different modes of a Filippov system and the reformulation is automated.

The package is based on CasADi (https://www.syscop.de/research/software/nosnoc#:~:text=is%20based%20on-,CasADi,-.%20It%20has%20both). It has both a MATLAB and python version, the source code can be found at:
https://github.com/nurkanovic/nosnoc
https://www.syscop.de/research/software/nosnoc#:~:text=nosnoc%20for%20MATLAB-,nosnoc%20for%20python%C2%A0,-Copyright%20%C2%A9%202024%20University


HPIPM
High-performance interior-point-method QP solvers
HPC QP interior-point-method

HPIPM
This is HPIPM, a high-performance interior-point method solver for dense, optimal control- and tree-structured convex quadratic programs. It provides efficient implementations of dense and structure-exploiting algorithms to solve small to medium scale problems arising in model predictive control and embedded optimization in general and it relies on the high-performance linear algebra package BLASFEO (https://www.syscop.de/research/software/syscop.de/research/software/blasfeo).

For an installation guide, examples or benchmarks, please visit the HPIPM github repository (https://github.com/giaf/hpipm).


TuneMPC
Economic tuning of (nonlinear) model predictive control problems.
Model Predictive Control
TuneMPC
TuneMPC is a Python package for economic tuning of nonlinear model predictive control (NMPC) problems.

More precisely, it implements a formal procedure that tunes a tracking (N)MPC scheme so that it is locally first-order equivalent to economic NMPC. For user-provided system dynamics, constraints and economic objective, TuneMPC enables automated computation of optimal steady states and periodic trajectories, and spits out corresponding tuned stage cost matrices.

The tool is publicly available at:
https://github.com/jdeschut/tunempc


AWEbox
Modeling and optimal control of single- and multi-drone airborne wind energy systems
optimal control airborne wind energy
AWEbox
AWEbox is an open-source Python toolbox for modeling and optimal control of AWE systems. Among others, it provides an implementation of validated models tailored for optimal control, and it takes away from the user the burden of formulating and numerically solving common AWE optimal control problems (OCP). A distinctive feature of AWEbox is that it supports optimization of multi-drone systems next to the prevalent single-drone variant as well. The second particular focus of the toolbox is robustness with respect to initialization, which we achieve by means of a formal homotopy strategy. The toolbox supports rigid-wing, lift- and drag-mode AWE systems and is capable of embedding user-provided 3D wind profiles. Building on the open-source optimization framework CasADi, it can be a particularly useful component in AWE system toolchains for performance assessment, system design, controller synthesis, or in a wide area of academic research ranging from AWE modeling to optimization algorithms.

The software is publicly available at:
https://github.com/awebox/awebox

CasADi
CasADi (https://web.casadi.org/) is a symbolic framework for algorithmic differentiation and numeric optimization. Using the syntax of computer algebra systems, it allows users to construct symbolic expressions consisting of either scalar- or (sparse) matrix-valued operations. These expressions can then be efficiently differentiated using state-of-the-art algorithms for algorithmic differentiation in forward and reverse modes and graph coloring techniques for generating complete, large and sparse Jacobians and Hessians.

The main purpose of the tool is to be a low-level tool for quick, yet highly efficient implementation of algorithms for nonlinear numerical optimization. Of particular interest is dynamic optimization, using either a collocation approach, or a shooting-based approach using embedded ODE/DAE-integrators. In either case, CasADi relieves the user from the work of efficiently calculating the relevant derivative or ODE/DAE sensitivity information to an arbitrary degree, as needed by the NLP solver.

For an installation guide, tutorial examples and a detailed documentation, please visit the CasADi (https://web.casadi.org/) webpage or the CasADi github repository (https://github.com/casadi/casadi).


