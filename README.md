GALIC v1.1  - A code for the creation of galaxy inititial conditions 
------------------------------------------------------------------------

GALIC v1.1 is an updated version of GALIC code (http://www.h-its.org/tap/galic) 
which is implementation of a new iterative method to construct steady state
composite halo-disk-bulge galaxy models with prescribed density distribution 
and velocity anisotropy. This update is mainly about the new constraints on the time averaged velocity structure in order to ensure its equality to the target distribution of velocity dispersions.
  
The method and the original version of GALIC is described in full in the paper:
Yurin D. & Springel, V. An iterative method for the construction of N-body galaxy models in collisionless equilibrium. MNRAS, 2014. (preprint: http://arxiv.org/abs/1402.1623). Users of the code are kindly asked to cite the paper if they make
use of the code. 

The updated version is not fully tested and released "as is", without any guarantees
or warrantees. To get support, please open a new issue.

Copyright (c) 2014-2017 by Volker Springel and Denis Yurin 

Known Issues
--------------------------------
#1. Calculation of target velocity dispersions is faulty beyond 8 Mpc for velocity structure of type 2, so don't use it for now for Halo and Bulge, instead if necessary mimic it with velocity structure of type 3 with dispersion R over Z ratio set to 1.

#2. Putting the time-averaged velocity dispersions to the target ones is not fully successful in case of the disk. This means that one can still see the rapid change of the velocity structure in the disk which is not related to the disk relaxation.
