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
