# Two-temperature model parameters
__Electron-temperature dependent parameters: electron-phonon coupling, electron heat capacity, and electron heat conductivity, calculated with `XTANT-3` code__

The electron-ion (electron-phonon) coupling parameters, electronic heat capacity, and electronic heat conductivity as functions of the electronic temperature (Te) were calculated with the help of the nonperturbative dynamical coupling formalism, and Kubo-Greenwood method. The method was implemented in the `XTANT-3` code (https://github.com/N-Medvedev/XTANT-3).
When using this dataset, please, cite the corresponding papers listed below.

## Electronic heat capacity

The electronic heat capacity, Ce(Te),  as a function of the electronic temperature (Te), is in the files named
* Ce_[El]_[data].txt
with [El] being the chemical element; [data] being additional information such as the structure of the material, or the tight-binding parametrization used (e.g., DFTB) (if the parametrization is not listed, the default NRL parametrization is used).

First two or three lines, starting with the symbol '#' are commenting the columns and the units of the variables in them.
The columns contain:
1) Electron temperature in [K]
2) Electronic heat capacity [J/(m^3 K)]

The data for metals, semiconductors [1], and 2d-carbon materials [2], are stored in the following directories, respectively:
* Ce_metals
* Ce_semiconductors
* Ce_2d_materials

_Note #1: not all materials, for which the coupling parameter is present, may have a file with the electron heat capacity. A separate set of heat capacities is present in the files with the heat conductivity, see below._

_Note #2: for 2d-materials, the two-dimensional electronic heat capacity is in the units of [J/(m^2 K)]. The heat capacity may be converted into 3d units, if needed, assuming the layer thickness of 3.35 A._


## Electron-phonon coupling

The electron-ion (electron-phonon) coupling parameters, G_e-ph(Te), as a function of the electronic temperature (Te), are in the files are named as follows:
* G_e-ph_[El]_[data].txt
with [El] being the chemical element; [data] being additional information, such as the structure of the material, or the tight-binding parametrization used (e.g., DFTB) (if the parametrization is not listed, the default NRL parametrization is used).

The data for elemental metals [3] (and SiAl alloy [4]), semiconductors [1], and 2d-carbon materials [2], are stored in the directories named, respectively:
* G_e-ph_metals
* G_e-ph_semiconductors
* G_e-ph_2d_materials

The files use the following format:
First two or three lines, starting with the symbol '#' are commenting the columns and the units of the variables in them.
The columns contain:
1) Electron temperature in [K]
2) Electron-ion coupling in [W/(m^3 K)]

_Note #3: in some files there are multiple columns for various atomic temperatures, listed in the third commentary line_

_Note #4: the start and end of the grid of the electronic temperature are not fixed but differ in various files_

_Note #5: For 2d materials, the two-dimensional electron-ion coupling parameter is in the units of [W/(m^2 K)]. It may be converted into 3d units, if needed, assuming the layer thickness of 3.35 A._


## Electronic heat conductivity

The electronic heat conductivity data are stored in the files named:
* K_[El]_[data].txt
with [El] being the chemical element; [data] being additional information, such as the structure of the material, or the tight-binding parametrization used (e.g., DFTB) (if the parametrization is not listed, the default NRL parametrization is used).

The data for metals and semiconductors [5] are stored in the directories named, respectively:
* K_metals
* K_semiconductors
 
First two lines, starting with the symbol '#' are commenting the columns and the units of the variables in them.
The columns column contain:
1) Electron temperature in [K]
2) Total electronic heat conductivity in [W/(m K)]
3) Electron-phonon term in electronic heat conductivity in [W/(m K)]
4) Electron-electron term in electronic heat conductivity in [W/(m K)]
5) Electronic chemical potential [eV]
6) Electronic heat capacity in [J/(m^3 K)]

_Note #6: the electronic heat capacity in these files is calculated differently from that in the files Ce_[El]_[data].txt above. In the former, it is calculated for the ideal crystal structure averaged over 7x7x7 k-points [5]; whereas the latter was obtained in dynamical simulations at a given atomic temperature in the gamma-point [1,2].


## Disclaimer

Although we endeavour to ensure that the code XTANT and results delivered are correct, no warranty is given as to their accuracy. We assume no responsibility for possible errors or omissions. We shall not be liable for any damage arising from the use of these dataset, or from any action or decision taken as a result of using it or any related material.

This dataset is distributed _as is_ for non-commercial peaceful purposes only, such as research and education. It is __explicitly prohibited__ to use it for military-related or other than peaceful purposes.

By using this repository, you agree with these terms and conditions.


## References

> [1] N. Medvedev, "_Electron-phonon coupling in semiconductors at high electronic temperatures_" (2023). https://arxiv.org/abs/2307.13554 

> [2] N. Medvedev, I. Milov, B. Ziaja, "_Structural stability and electron‐phonon coupling in two‐dimensional carbon allotropes at high electronic and atomic temperatures_" Carbon trends 5, 100121 (2021). https://doi.org/10.1016/j.cartre.2021.100121

> [3] N. Medvedev, I. Milov, "_Electron-phonon coupling in metals at high electronic temperatures_", Phys. Rev. B. 102 (2020) 064302. https://doi.org/10.1103/PhysRevB.102.064302 

> [4] M. Medvedev, I. Milov, "_Contribution of inter- and intraband transitions into electron–phonon coupling in metals_", Eur. Phys. J. D 75, 212 (2021). https://doi.org/10.1140/epjd/s10053-021-00200-w

> [5] N. Medvedev, F. Akhmetov, I. Milov, "_Electronic heat conductivity in two-temperature state_" (2023).


