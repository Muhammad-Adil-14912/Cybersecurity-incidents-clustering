# Temporal Clustering of Cybersecurity Incidents

This project explores historical cybersecurity incidents using Python, pandas, NumPy, Matplotlib, Seaborn, and scikit-learn. The notebook focuses on temporal trends, incident categories, affected industries and countries, financial loss, and correlations among incident attributes.

## Repository contents

```text
.
├── IBM_int_proj.ipynb
└── README.md
```

## Dataset requirement

The notebook loads a CSV file named `Time_Based_Cybersecurity_Incidentscsv.csv` from the repository root:

```python
filesdf = pd.read_csv('Time_Based_Cybersecurity_Incidentscsv.csv')
```

**The CSV dataset is not currently included in this repository.** Obtain the dataset from its authorized source and place it beside the notebook using that exact filename before running the data-loading cell. The notebook will not run end-to-end until the dataset is available.

## Setup

```bash
git clone https://github.com/Muhammad-Adil-14912/Cybersecurity-incidents-clustering.git
cd Cybersecurity-incidents-clustering
python -m venv .venv
```

Activate the virtual environment, then install dependencies:

**Windows PowerShell**
```powershell
.venv\Scripts\Activate.ps1
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook
```

**macOS / Linux**
```bash
source .venv/bin/activate
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook
```

Open `IBM_int_proj.ipynb` and run the cells after adding the required dataset.

## Analysis workflow

- Data inspection, cleaning, missing-value checks, and duplicate handling
- Date parsing and year/month feature extraction
- Exploratory analysis by country, attack type, source, and industry
- Time-based incident counts and financial-loss trends
- Correlation analysis for financial loss, affected users, and resolution time

## Important note

Results depend on the dataset supplied at runtime. Verify its provenance, schema, and license before use, and do not treat historical correlations as proof of causation.
