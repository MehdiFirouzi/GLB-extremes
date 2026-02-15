# GLB-extremes

Code and analysis workflow for:

“Intercomparison of reanalysis datasets’ performance in capturing precipitation and temperature extremes over the Great Lakes Basin.”

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

git clone https://github.com/MehdiFirouzi/GLB-extremes.git

conda env create -f environment.yml
conda activate glb-extremes


Update dataset paths in `config/params.yaml` before running analyses.

---

## Data

Reanalysis datasets (PRISM, EMDNA, RDRS v2.1, ERA5, MERRA-2, and CHIRPS v2.0.) are obtained from their original providers and are not included.

A versioned release will be archived via Zenodo (DOI to be added).

---


## License

Code: MIT License

Derived data products (if distributed separately) are released under CC-BY-4.0.
