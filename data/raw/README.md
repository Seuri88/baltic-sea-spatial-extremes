# Raw GESLA‑3 Data (CMEMS subset)

This folder contains instructions for accessing the CMEMS subset of the raw GESLA‑3 tide gauge dataset used in this study.

The raw data are **not included** in this repository due to file size, but they can be freely used for **research purposes** under the GESLA‑3 license.

---

## Downloading the data

The CMEMS subset of the raw GESLA‑3 data (~236 MB) used in this study is available on Zenodo:

https://doi.org/10.5281/zenodo.15024220

The ZIP file contains:

- `GESLA3 DATA BALTIC NORTH CMEMS/` — the subset of tide gauge data used in the article  
- `GESLA3_ALL_2.csv` — metadata describing each station  
- `LoadingGesla.py` — the official GESLA‑3 loader script to read the raw files  
- `README.txt` — instructions included in the ZIP

**Instructions:**

1. Download the ZIP file from the Zenodo link above.  
2. Extract its contents into this folder (`data/raw/`).  
3. Update any file paths in notebooks/scripts to point to the extracted location.  
4. Use the provided loader script or your own code to generate *block maxima* and *detrended time series* for analysis.

---

## GESLA‑3 Official Page

The raw GESLA‑3 dataset and documentation can be found here:

https://gesla787883612.wordpress.com/

This site includes:

- Description of the GESLA‑3 dataset  
- Download links for the full dataset and individual subsets  
- Licensing and usage information

Please consult that page for more detailed guidance on the data formats and original sources.

---

## License

- The CMEMS data are part of the GESLA‑3 dataset.  
- Research use is allowed without restriction.  
- Users intending to use the data for consultancy or commercial purposes must contact the original data providers per the GESLA‑3 licensing terms.

---

## Notes

- The ZIP file contains **raw, unprocessed data only**; it does not include derived products such as block maxima or detrended series.  
- The Python file (`LoadingGesla.py`) is provided to help load the raw data as a **pandas DataFrame** or **xarray object**.  
- **Path setup:** Notebooks and scripts currently reference local paths. Users must **update the paths manually** to where they extract the ZIP files.  
- Once paths are set, the processing scripts in `notebooks/` or `src/` can be run to generate the derived data used in the manuscript.
