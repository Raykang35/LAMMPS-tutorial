# LAMMPS tutorial

A. Useful command

1. Minimize command: `minimize etol ftol maxiter maxeval`

   etol: stopping tolerance for energy (unitless)

   ftol: stopping tolerance for force

   maxiter: max number of iterations

   maxeval: max number of force/energy evaluations

3. Fix command: `fix ID group-ID style args`
   
   ID: users name this "fix" by themselves

   group-ID: ID of the group of atoms to apply the fix to

   style: one of a list of possible style names https://docs.lammps.org/Commands_fix.html#

   args: arguments used by the style

4. Dump command: `dump ID group-ID style N file attribute1 attribute2 ...`
   
   style: atom or atom/adios or atom/gz or atom/zstd or cfg or cfg/gz or cfg/zstd or cfg/uef or custom or custom/gz or custom/zstd or custom/adios or dcd or grid or grid/vtk or h5md or image or local     or local/gz or local/zstd or molfile or movie or netcdf or netcdf/mpiio or vtk or xtc or xyz or xyz/gz or xyz/zstd or yaml

   N: dump on timesteps which are multiples of N

   file: name of file to write dump info to

   attribute#: list of attributes for a particular style

5. Thermo command: `thermo N`
   
   Compute and print thermodynamic info

   N: N timesteps

6. Run command: `run N keyword values ...`

   N: number of timesteps
   
7. Atom_style command: `atom_style style args`

   https://docs.lammps.org/atom_style.html

8. Pair_style + Pair_coeff command: `pair_style style args` `pair_coeff I J args`

9. Bond_style + bond_coeff command: `bond_style style args`
    
10. Angle_style + angle_coeff command: `angle_style style args`
   

B. Workflow

1. Choosing compatiable force field

2. System preparation (creating initial configuration)

3. Minimization (just like optimization)

4. Equilibration (need to choose thermo ensemble, get stable phase in the end)




References

1. https://www.compchems.com/setting-up-a-molecular-dynamics-simulation
2. https://docs.lammps.org/Manual.html
3. https://www.osti.gov/servlets/purl/1563110 (explicit atom_style) 

