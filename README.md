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
