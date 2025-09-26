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
