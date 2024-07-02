#Molecular Dynamics Simulation Steps

1.Preparation of Ligand Topology:
```
The CHARMM General Force Field (CgenFF) server was used to produce the desired ligand topology.
```
2.Preparation of Protein Topology:
```
The pdb2gmx script was used to prepare the protein topology.
```
3.Combination of Topologies:
```
The ligand and protein topologies were combined and subjected to the Charmm36-July-2017 force field to produce energy minimized conformations of the processed complexes.
```
4.Solvation:
```
The ligand-protein complexes were solvated in a cubic simulation box using the SPC216 water model.
```
5.Energy Minimization:
```
Steepest descent algorithm was applied for the energy minimization of the complexes, with a maximum of 50,000 steps.
```
6.Equilibration:
```
The system was equilibrated under the NVT ensemble (const no. of particles, volume, and temp) for 2 ns.
After NVT, under the NPT ensemble system was equilibrated (i.e const no. particles, temp and pressure) for 10 ns.
```
7.Production Phase:
```
The well-equilibrated and solvated structures were subjected to the production phase of simulation without any restraints for a period of 200 ns.
System coordinates were saved every 2 ps.
```
8.Trajectory Analysis:
```
The MD produced trajectories were analyzed using quantitative parameters such as root mean square deviation (RMSD), root mean square fluctuation (RMSF), radius of gyration (Rg), and hydrogen bond contact profile.
Analysis was conducted using in-built scripts of GROMACS.
```
