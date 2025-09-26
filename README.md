# datafun-06-eda

## Overview
Exploratory Data Analysis (EDA) project per module spec:  
https://github.com/denisecase/datafun-06-spec

## Setup (Windows / PowerShell)
git clone https://github.com/larrygold18/datafun-06-eda.git

cd datafun-06-eda
py -3 -m venv .venv
..venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install jupyterlab numpy pandas pyarrow matplotlib seaborn
pip freeze > requirements.txt

## Project Structure
datafun-06-eda/
├─ data/
│ ├─ raw/
│ └─ processed/
├─ notebooks/
├─ src/
├─ reports/
├─ figures/
├─ .gitignore
├─ requirements.txt
└─ README.md

## Commands Log
git status
git add .
git commit -m "Initialize EDA project per Dr. Denise"
git push origin main
## Dataset

**Name:** Iris (Fisher’s Iris Dataset)  
**Source (clickable):** https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv  

**Why this dataset:**  
It’s small, tidy, and has **no missing values**, which matches CC6’s focus on exploration and visualization (not heavy cleaning).

**Local path (if stored):** `data/raw/iris.csv`

### First-load snippet
```python
import pandas as pd
df = pd.read_csv("data/raw/iris.csv")  # or read directly from the URL
df.info()
df.describe(numeric_only=True)

---

### 2. Stage, commit, and push
```powershell
git add README.md
git add data/raw/iris.csv
git commit -m "CC6.2: Add Iris dataset description, link, and raw CSV"
git push origin main
```