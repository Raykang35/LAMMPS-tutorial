# LAMMPS tutorial




Minimize command: `minimize etol ftol maxiter maxeval` 

etol: stopping tolerance for energy (unitless)

ftol: stopping tolerance for force

maxiter: max number of iterations

maxeval: max number of force/energy evaluations

Fix command: `fix ID group-ID style args`

ID: users name this "fix" by themselves

group-ID: ID of the group of atoms to apply the fix to

style:  one of a list of possible style names https://docs.lammps.org/Commands_fix.html#

args: arguments used by the style

Dump command: `dump ID group-ID style N file attribute1 attribute2 ...`

style: atom or atom/adios or atom/gz or atom/zstd or cfg or cfg/gz or cfg/zstd or cfg/uef or custom or custom/gz or custom/zstd or custom/adios or dcd or grid or grid/vtk or h5md or image or local or local/gz or local/zstd or molfile or movie or netcdf or netcdf/mpiio or vtk or xtc or xyz or xyz/gz or xyz/zstd or yaml

N: dump on timesteps which are multiples of N

file: name of file to write dump info to

attribute#: list of attributes for a particular style


