# vineyard_prefactor

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## About

This code calculates the Vineyard prefactor<sup>[1](#vineyard)</sup> for a process generated by a climbing-image NEB<sup>[2](#neb)</sup> calculation in LAMMPS<sup>[3](#lammps_paper)</sup> <sup>[4](#lammps_link)</sup> <sup>[5](#lammps_neb)</sup>.

The main script is `vineyard.sh`, which performs various calculations in and out of LAMMPS using an input `.json` config file.

To run an example, run:

```bash
./vineyard.sh config.json
```

This will perform an NEB run for vacancy hopping in Si, writing both the Vineyard prefactor and energy barrier to `rate.txt`. Details about the calculation of the prefactor calculation are in [vineyard.pdf](https://github.com/jwjeffr/vineyard_prefactor/blob/main/vineyard.pdf).

##

<a name="vineyard">1</a>: https://doi.org/10.1016/0022-3697(57)90059-8

<a name="neb">2</a>: https://doi.org/10.1063/1.1329672

<a name="lammps_paper">3</a>: https://doi.org/10.1016/j.cpc.2021.108171

<a name="lammps_link">4</a>: https://lammps.org/

<a name="lammps_neb">5</a>: https://docs.lammps.org/neb.html