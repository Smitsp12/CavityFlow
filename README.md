# CavityFlow
This repository contains a python code that computes the velocity field in a standard lid driven cavity problem. Streamfunction - Vorticity formulation is used to model the flow. The forward time - centered space (FTCS) method is used for discritization of the governing equations. The steps used for this are as follows:
1) initialize omega and psi as zero over entire domain.
2) set initial and boundary conditions for u and v. u,v = 0 at interior nodes, v = 0 everywhere, u = 1 at top wall.
3) solve the discritized equation for some finite time in a loop
    i) First get the boundary conditions for omega.
    ii) solve discritized vorticity transport and poission equation and from psi get velocity components.
4) update the values of omega, psi, u and v for next iteration.
5) post processing of the resuts.

![Velocity Field](https://github.com/Smitsp12/CavityFlow/assets/132105298/6a8f07d2-291d-4e24-a00f-d58ca543a1f7)
