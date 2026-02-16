# GLB-extremes

[![DOI](https://zenodo.org/badge/1036960348.svg)](https://doi.org/10.5281/zenodo.18664699)

Code and analysis workflow for:

Firouzi, M., and Coulibaly, P. (2026).  
**Intercomparison of reanalysis datasets performance in capturing precipitation and temperature extremes over the Great Lakes Basin.**  
Journal of Climate (submitted).

### Mohammadmehdi Firouzi¹ and Paulin Coulibaly¹,²,³  

¹ Department of Civil Engineering, McMaster University, 1280 Main Street West, Hamilton, ON L8S 4L7, Canada  
² School of Earth, Environment and Society, McMaster University, 1280 Main Street West, Hamilton, ON L8S 4L7, Canada  
³ United Nations University Institute for Water, Environment and Health, Richmond Hill, ON, Canada  

Corresponding author: Mohammadmehdi Firouzi  
Email: firouzim@mcmaster.ca  

---

This repository contains the code and minimal reproducible workflow associated with the Journal of Climate submission.

---

## Structure

### config/
- `params.yaml` – Study configuration

### figures/ (final manuscript figures)

- `bias-spatial-maps/`
- `boxplots_prcp/`
- `boxplots_temperature/`
- `cdf_plots_prcp/`
- `cdf_plots_temperature/`
- `seasonal_boxplots_prcp/`
- `seasonal_boxplots_temperature/`
- `station_locations/`
- `study_area_map/`
- `taylor_diagrams/`
- `Workflow-Chart/`


### notebooks/
- `Datasets-Download-Scripts.ipynb` – Dataset download scripts

### src/ (analysis code)
- `data_prep/` – Dataset preparation  
- `emdna_tests/` – EMDNA ensemble evaluation  
- `indices/` – ETCCDI index calculation  
- `statistical_metrics/` – Performance metrics  
- `lwr/` – Locally Weighted Regression  
- `taylor-diagrams/` – Taylor diagram generation  
- `figures/` – Figure-generation scripts  

---

## Reproducibility

Clone the repository and create the environment:

```bash
git clone https://github.com/MehdiFirouzi/GLB-extremes.git
conda env create -f environment.yml
conda activate glb-extremes
```

Before running the analyses:

- Update dataset paths in `config/params.yaml`
- Adjust local input/output paths in the scripts or notebooks as needed

---

## Data

Reanalysis datasets (PRISM, EMDNA, RDRS v2.1, ERA5, MERRA-2, and CHIRPS v2.0) are obtained from their original providers and are not included in this repository due to file size constraints.

A versioned release of this repository will be archived via Zenodo (DOI to be added).

---

## License

Code: MIT License
