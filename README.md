# Opposing BOLD signals and oxygen metabolism largely arise from statistical uncertainty in metabolic estimates

Ole Goltermann, Alexander Huth, & Christian Büchel

![Last update](https://img.shields.io/badge/last_update-March_19,_2026-green)


## Overview

This repository contains the full analysis code used in:

**Goltermann, Huth, & Büchel — *Opposing BOLD signals and oxygen metabolism largely arise from statistical uncertainty in metabolic estimates*.**

The project provides a reanalysis of the openly available dataset used in:

**[Epp et al. (2025), *Nature Neuroscience*](https://www.nature.com/articles/s41593-025-02132-9).**

The original study reported widespread voxel-wise **sign discordance** between BOLD signal changes and estimated changes in cerebral metabolic rate of oxygen (ΔCMRO₂). The authors reported that roughly **40% of voxels with significant BOLD changes showed opposing oxygen metabolism**, challenging the canonical interpretation of BOLD signals.

In our reanalysis we show that:

- ΔCMRO₂ estimates exhibit **substantial variability across participants**
- **77.2% of reported voxels in Epp et al. cannot be robustly classified** as concordant or discordant
- Where classification is possible, **positive BOLD responses are largely concordant with metabolism**
- Reported concordance and discordance in Epp et al. mainly reflects **statistical uncertainty in CMRO₂ estimates**


## Requirements

This project was developed in **Python 3.9+** and depends on the following Python packages:

- numpy
- pandas
- scipy
- nibabel
- nilearn
- matplotlib
- statsmodels

### Optional external software

The full reanalysis from the original dataset additionally requires:

- **DataLad**
- **git-annex**
- **FSL** (`flirt`)
- **ANTs** (`antsApplyTransforms`)

These external tools are only needed if you set `download = True` and want to download original data from Epp et al.

## Installation

Install the Python dependencies with:

```bash
pip install -r requirements.txt
```

## Contact
For questions or issues, please contact [o.goltermann@uke.de].





