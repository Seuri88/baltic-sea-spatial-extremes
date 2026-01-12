# Supplementary Notebook

This notebook (`supplementary.ipynb`) contains all the analyses and supplementary material for:

> **A probabilistic view of spatial extreme sea level events in the Baltic Sea**  
> Authors: Seuri Basilio Kuosmanen, Magnus Hieronymus  

It is **self-contained** and will automatically:

- Load all required Python packages and repository modules  
- Read the raw CMEMS GESLA‑3 tide gauge data and metadata  
- Generate block maximas from detrended time series data
- Compute Bayesian inference objects: posterior predictive distributions and posterior distributions
- Perform Markov Chain Monte Carlo diagnostics
- Reproduce all figures and tables in the manuscript

---

## Before running the notebook

1. Download the raw CMEMS GESLA-3 data from Zenodo and extract it into data/raw/ (see main repository README for instructions). 
2. Update the two required paths at the 9th cell of the notebook:

```python
# Path to the metadata file
metafile = "/path/to/GESLA3_ALL_2.csv"

# Path to the CMEMS subset data folder
region_datapath = "/path/to/GESLA3 DATA BALTIC NORTH CMEMS/"
```

Replace /path/to/... with the location where you extracted the ZIP contents.

## Running the notebook

Open the notebook in Jupyter or JupyterLab:
```bash
jupyter notebook supplementary.ipynb
```
Run all cells from top to bottom. All figures, tables, and supplementary analyses will be generated automatically.

