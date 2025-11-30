# Insurance Claim Prediction

Brief notebook + basic training pipeline to explore and model insurance claim data.

## Repo layout

- insurancee_pred.ipynb — main EDA & modeling notebook
- train_Insurance.csv — raw dataset (keep out of VCS; add to .gitignore)
- requirements.txt — Python dependencies
- .gitignore — recommended ignores (virtualenv, data, artifacts)

## Quick setup (Linux)

1. Create & activate virtualenv

```bash
python3 -m venv .venv
source .venv/bin/activate
```

2. Install dependencies

```bash
pip install -U pip
pip install -r requirements.txt
# if no requirements.txt:
pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyterlab
```

## Run

- Start Jupyter and open the notebook:

```bash
jupyter lab
# or
jupyter notebook
```

- Run cells in order. Data is read from `train_Insurance.csv` (place it in project root or update path in notebook).

## Common commands

- Initialize repo / push

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin <remote-url>
git push -u origin main
```

- Check the remote you pushed to:

```bash
git remote -v
git branch -vv
```

## Notes

- Do not commit raw data or virtual environments. Add `train_Insurance.csv` and `.venv/` to `.gitignore`.
- Imputation and preprocessing are handled in the notebook; check cells under "Phase 3 : Data Preparation".
- Add `requirements.txt` before sharing for reproducibility.

License: add if needed.
