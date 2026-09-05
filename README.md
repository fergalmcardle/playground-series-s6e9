# Playground Series S6E9

Kaggle competition: https://www.kaggle.com/competitions/playground-series-s6e9/overview

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Kaggle API credentials

Download `kaggle.json` from https://www.kaggle.com/settings (Account > API > Create New Token), then:

```bash
mkdir -p ~/.kaggle
mv ~/Downloads/kaggle.json ~/.kaggle/kaggle.json
chmod 600 ~/.kaggle/kaggle.json
```

## Download competition data

```bash
kaggle competitions download -c playground-series-s6e9 -p data
unzip data/playground-series-s6e9.zip -d data
```

## Project structure

- `data/` — competition data (gitignored)
- `notebooks/` — exploratory analysis
- `src/` — reusable pipeline code
- `submissions/` — generated submission CSVs (gitignored)
