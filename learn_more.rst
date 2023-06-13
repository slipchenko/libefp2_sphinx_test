.. _learn_more:

********************
Learn more about EFP
********************

Calculations in the condensed phase still remain a major challenge to the theoretical community.
The increased number of nuclear and electronic degrees of freedom makes accurate *ab initio*
calculations of a condensed phase system unfeasible long before the system approaches the bulk.
In this case, the system is often modeled with a parameterized force field.
A drawback of such an approach is the dependence on fitted parameters for a chosen force field,
such that different parameterizations may be optimal for different problems and the best
parameters are often not well defined. The EFP method overcomes this problem.
In EFP, each solvent molecule ("fragment") is represented by a model potential
with a set of parameters determined from a preparatory *ab initio* calculation,
such that the method is free of parameter fitting. Through its force field,
the effective fragments interact with each other and with *ab initio* components.

The original EFP implementation has been extended to macromolecules and polymers,
as described in :ref:`bioefp`. EFP is combined with a number of *ab initio* methods
(:ref:`QM/EFP`) for fast and efficient modeling of electronic structure in the condensed phases.

EFP calculations involve two steps:

* preparation of effective parameters described in :ref:`parameters`
* calculation on the system properties of interest, where the system is composed of
  effective fragments described in :ref:`efp_calcs`
