# Lysosomal polygenic risk score in Parkinson’s disease across populations.

`GP2 ❤️ Open Science 😍`
[![DOI](https://zenodo.org/badge/DOI/nnnnn/zenodo.nnnnn.svg)](https://doi.org/nnnnn/zenodo.nnnnn) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 

**Last updated:** August 2026

## Summary
This is the online repository for the manuscript titled "Lysosomal polygenic risk score in Parkinson’s disease across populations". This study focuses on 1) evaluation of lysosomal polygenic risk score (lyso-PRS) performance for PD risk across populations using the GP2 Neurobooster genotyping array. 2) Comparison of the lyso-PRS across idiopathic PD (iPD), GBA1-PD, non-manifesting GBA1 carriers (NMC), and healthy controls (HC) in the European population and assessment of the lyso-PRS association with GBA1-PD status. 3) Regression analysis of the lyso-PRS and clinical outcomes in the PD patients of European population.

## Data statement
All GP2 data are hosted in collaboration with the Accelerating Medicines Partnership in Parkinson’s disease, and are available via application on the website (https://amp-pd.org/register-for-amp-pd). For up-to-date information on GP2 data acquisition, access, and policies, visit https://gp2.org/. 

All data was using GP2 release 11 (https://zenodo.org/records/17753486). Genotyping imputation, quality control, ancestry prediction, and processing were performed using GenoTools (v1.0.0), publicly available on GitHub.

Data of European Tuebingen Parkinson cohort dataset are available in an anonymized format on request to: kathrin.brockmann[at]uni-tuebingen.de

## Helpful Links

- [GP2 Website](https://gp2.org/)
  - [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
- [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
  - [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)

## Repository Orientation

- The `analyses/` directory contains all analyses described in the manuscript.
- The `GP2/` directory contains three Jupyter notebooks for processing and analyzing GP2 NeuroBooster Array data from Release 11, along with two R Markdown files for clinical data analyses.

```text
THIS_REPO/
├── LICENSE
├── README.md
└── analyses/
    └── GP2/
        ├── 00_Cohort_def_r11.ipynb
        ├── 01_PRScalculation_r11.ipynb
        ├── 02_PRScal_GBA1_r11.ipynb
        ├── 03_META_NBA.Rmd
        └── 04_TUEPAC.Rmd
```

# Analysis Notebooks
## Languages: Python, bash, and R
| Notebooks   | Description | 
|----------------|--------|
| Cohort_def_r11         | Genetic status cohort definition analysis with GP2 Neurobooster array|
| PRScalculation_r11         | lysosomal polygenic risk score analysis across populations with GP2 Neurobooster array|
| PRScal_GBA1_r11        | lyso-PRS comparisons across GBA1-PD vs HC/NMC/iPD with GP2 Neurobooster array|
| META_NBA         | Meta analysis of demographics and clinical outcomes in European-GP2 cohort|
| TUEPAC         | regression analysis of demographics and clinical outcomes in European-TUEPAC cohort|

# Software

| Software | Version(s) | Resource URL | RRID | Notes |
|----------|------------|--------------|------|-------|
| PLINK | 1.9 and 2.0 | http://www.nitrc.org/projects/plink | SCR_001757 | Used for general genetic data manipulation and association testing |
| PRSice | 2.3.5 | https://github.com/choishingwan/PRSice | SCR_017057 | Used for PRS analyses|
| metafor | 4.8-0 | https://cran.r-project.org/web/packages/metafor/index.html | SCR_003450 | Meta-analysis |
| Python Programming Language | 3.10.15 | http://www.python.org/ | SCR_008394 | General data wrangling and visualization ; pandas; numpy; pathlib; sci-kit learn; scipy; matplotlib; seaborn |
| R Project for Statistical Computing | 4.3.3 | http://www.r-project.org/ | SCR_001905 | General data wrangling and visualization; readxl; dplyr; ggplot2; broom; |

