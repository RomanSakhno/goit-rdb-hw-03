# HW3 — UCI Adult: Data Loading, Quality Audit & SQL EDA

## Dataset
- **Name:** Adult (Income Prediction)
- **Official source:** https://archive.ics.uci.edu/dataset/2/adult
- **Download method:** `ucimlrepo` (`fetch_ucirepo(id=2)`) in the notebook.
- **Sampling:** the full dataset returned by the package; exact row count is printed during execution.

## Implemented
1. Start PostgreSQL in Colab with `pgserver` and print server version.
2. Fetch the dataset reproducibly and write a controlled CSV.
3. Load raw columns as `TEXT` into `hw3_adult_staging` using `COPY FROM STDIN`.
4. Create typed `hw3_adult_clean` with identity primary key, domain checks, and indexes.
5. Audit row counts, duplicate signatures, null rates, and source sentinel markers.
6. Analyze target distribution, numeric statistics, and domain-specific anomalies.
7. Run ten SQL DQL/EDA queries with business questions and interpretations.
8. Include a 200–250-word reflection about quality, features, leakage, and pipeline improvements.

## Run
Open `HW3_UCI_Adult_Data_Quality_EDA.ipynb` in Google Colab and choose **Runtime → Restart session and run all**. The notebook installs dependencies and downloads the dataset; no manual data download is needed.

## Files
- `HW3_UCI_Adult_Data_Quality_EDA.ipynb` — executable notebook.
- `README.md` — project overview and run instructions.
