# Electron-ion (electron-phonon) coupling
__Electron-phonon coupling and related parameters calculated with XTANT-3 code__

This is the (updated) dataset for materials reported in 
N. Medvedev, I. Milov, "_Electron-phonon coupling in metals at high electronic temperatures_", Phys. Rev. B. 102 (2020) 064302. https://doi.org/10.1103/PhysRevB.102.064302 

The electron-ion (electron-phonon) coupling parameters and the electronic heat capacity as functions of the electronic temperature (Te) were calculated with the help of the nonperturbative dynamical coupling formalism. The method was implemented in the XTANT-3 code (https://github.com/N-Medvedev/XTANT-3) on the basis of tight-binding (TB) molecular dynamics (MD) (https://doi.org/10.48550/arXiv.2307.03953).

The data are saved in the following directories:

## G_e-ph : electron-ion (electron-phonon) coupling parameter

The electron-ion (electron-phonon) coupling parameters are stored in this directory. The files are named as 
* G_e-ph_[El]_[data].txt

with [El] being the chemical element; [data] being additional information, such as the structure of the material, or the tight-binding parametrization used (e.g., DFTB) (if the parametrization is not listed, the default NRL parametrization is used).

The files use the following format:

First two or three lines, starting with the symbol '#' are commenting the columns and the units of the variables in them.
The columns contain:
1) Electron temperature in [K]
2) Electron-ion coupling in [W/(m^3 K)]

_Note #1: in some files there are multiple columns for various atomic temperatures, listed in the third commentary line_

_Note #2: the start and end of the grid of the electronic temperature are not fixed but differ in various files_

## Ce : electronic heat capacity

The electronic heat capacity as the function of the electron temperature are storred in the files:
* Ce_[El]_[data].txt

First two or three lines, starting with the symbol '#' are commenting the columns and the units of the variables in them.
The columns contain:
1) Electron temperature in [K]
2) Electronic heat capacity [J/(m^3K)]

_Note #3: not all materials, for which the coupling parameter is present, may have a file with the electron heat capacity_


## Disclaimer

If you use the data from this repository, please cite the following paper:
* N. Medvedev, I. Milov, "_Electron-phonon coupling in metals at high electronic temperatures_", Phys. Rev. B. 102 (2020) 064302. https://doi.org/10.1103/PhysRevB.102.064302


Although we endeavour to ensure that the code XTANT and results delivered are correct, no warranty is given as to their accuracy. We assume no responsibility for possible errors or omissions. We shall not be liable for any damage arising from the use of these dataset, or from any action or decision taken as a result of using it or any related material.

This dataset is distributed _as is_ for non-commercial peaceful purposes only, such as research and education. It is __explicitly prohibited__ to use it for military-related or other than peaceful purposes.

By using this repository, you agree with these terms and conditions.