# GLB-extremes

Code and analysis workflow for:

“Intercomparison of reanalysis datasets’ performance in capturing precipitation and temperature extremes over the Great Lakes Basin.”

---

## Structure

### config/
- `params.yaml` – Study configuration

### figures/ (final manuscript figures)
- Bias-spatial-maps/
- Boxplots prcp/
- Boxplots temperature/
- CDF plots prcp/
- CDF plots temperature/
- Seasonal boxplots prcp/
- Seasonal boxplots temperature/
- Station Locations/
- Study area map/
- Taylor Diagrams/

### notebooks/
- `Datasets-Download-Scripts.ipynb` – Dataset download scripts

### src/ (analysis code)
- `data_prep/` – Dataset preparation  
- `emdna_tests/` – EMDNA ensemble evaluation  
- `indices/` – ETCCDI index calculation  
- `statistical metrics/` – Performance metrics  
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

Reanalysis datasets (EMDNA, PRISM, ERA5, MERRA-2, etc.) are obtained from their original providers and are not included.

A versioned release will be archived via Zenodo (DOI to be added).

---

## License

## License

Code: MIT License

Derived data products (if distributed separately) are released under CC-BY-4.0.
