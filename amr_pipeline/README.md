# AMR standardization pipeline (Tunisian hospitals)

Notebook: `notebooks/AMR_standardization_pipeline.ipynb`. English dictionaries: `dictionaries_en/`.

## Run
```bash
export AMR_DATA=/path/to/copie_files_no_patient   # raw CSVs (NOT versioned)
export AMR_DICT=./dictionaries_en
export AMR_OUT=./outputs
export AMR_SALT='<secret>'                        # salt for patient-ID hashing
# optional smoke test on ~30 files: export AMR_MAX_FILES=30
jupyter lab notebooks/AMR_standardization_pipeline.ipynb
```
Requires the `AMR` Python package (rpy2 + R). Raw data and outputs are git-ignored (patient-level data).
