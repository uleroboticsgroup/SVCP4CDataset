# Vulnerable Source Code Collected from Open Source Repositories for Dataset Generation

[![doi: 10.3390/app10041270](https://img.shields.io/badge/DOI-10.3390/app10041270-informational)](https://doi.org/10.3390/app10041270)
[![License: CC BY-ND 4.0](https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey)](https://creativecommons.org/licenses/by-nd/4.0/)

This repository holds five datasets that list existing Buffer Overflow vulnerabilities in more than 10000 source code files written in C. Particularly, it is suitable for extracting features and creating training datasets for Machine Learning. The data was collected from open source repositories linked to [SonarCloud](https://sonarcloud.io/) using [SVCP4C](https://github.com/uleroboticsgroup/SVCP4C) on different dates.

## Datasets

| Name                     | Total Files      | Checksum |
| ------------------------ | :--------------: | -------- |
| DataSet_07032019.tar.gz  | 2305             | abc7e173fca5d1e7b22313dfade2be19297d6e6735e4d325301a2f410f488797 |
| DataSet_03062019.tar.gz  | 2378             | ba367f4c4c21e26f6de79652185758394d80998d88b14a0bcbecc299b6336a3d |
| DataSet_16082019.tar.gz  | 2262             | c12599c8412629925f09821bdf2a74970afd631a9e376cd7fd67bdc5fef9ec3f |
| DataSet_20082019.tar.gz  | 2258             | 6c69f14cf6e839955d97e48afe502914715d84d409170ea0ba499107ec902943 |
| DataSet_31082019.tar.gz  | 2257             | b3984fe3d91426b607f89222d44fef7bfcbb13af894ea2f29afadf96365da1de |

## Vulnerabilities format

Vulnerabilities are listed using comments appended at the end of each file (see [SVCP4C](https://github.com/uleroboticsgroup/SVCP4C) repository). Such comments follow the format `// starting_line,starting_offset;ending_line,ending_offset` (with offset being the column). For example, file *DataSet_03062019.tar.gz/bzip2debianstretche1.0.6/bzip2.c* has four vulnerabilities tagged like:

```c
//						↓↓↓VULNERABLE LINES↓↓↓

// 1126,3;1126,9

// 1153,9;1153,15

// 1341,9;1341,15

// 1734,6;1734,12
```

# Reference

For scientific publications, please reference this repository using:

## Plain

```
Raducu, R., Esteban, G., Rodríguez Lera, F. J., & Fernández, C. (2020). Collecting Vulnerable Source Code from Open-Source Repositories for Dataset Generation. Applied Sciences, 10 (4), 1270. DOI: https://doi.org/10.3390/app10041270
```

## BibTeX

```BibTeX
@ARTICLE{Raducu2020,
  Title     = {Collecting Vulnerable Source Code from Open-Source Repositories for Dataset Generation},
  Author    = {Raducu, Razvan and Esteban, Gonzalo and Rodr{\'\i}guez Lera, Francisco Javier and Fern{\'a}ndez, Camino},
  Journal   = {Applied Sciences},
  Volume    = {10},
  Number    = {4},
  Pages     = {1270},
  Year      = {2020},
  Publisher = {Multidisciplinary Digital Publishing Institute},
  Doi       = {https://doi.org/10.3390/app10041270}
}
```

# License

Datasets are licensed under [CC BY-ND 4.0](https://creativecommons.org/licenses/by-nd/4.0/).