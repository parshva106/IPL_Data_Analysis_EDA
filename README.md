# IPL Data Analysis — Exploratory Data Analysis (EDA)

**Project name:** IPL - Data Analysis (Exploratory Data Analysis)

**Short description:**
This project performs a comprehensive exploratory data analysis (EDA) on the Indian Premier League (IPL) datasets (matches and deliveries). It answers multiple statistical and cricket‑analytics questions (match counts per season, toss behaviour, team & player statistics, boundary contributions, high-scoring matches, venues, and more), and provides visualizations and notebooks that reproduce the results.

---

## Table of contents

* Project overview
* Dataset
* Data analysis questions (covered)
* Repository structure
* Setup & requirements
* How to run (step-by-step)
* Reproducible analysis notes
* Outputs / visualizations
* Good practices
* Contributing
* License & contact

---

## Project overview

This repository contains code (Jupyter notebooks and helper scripts) used to explore and analyze the IPL matches and deliveries datasets. The goal is to extract insights about teams, players, venues, toss/decision impacts, scoring patterns (powerplay vs death overs), and more.

## Dataset

The analysis uses two datasets (place these CSVs in the `data/` folder):

1. **Deliveries dataset** — ball-by-ball data (ball-level deliveries). Download link used in the project brief: `https://drive.google.com/file/d/1O6E5DBDSFYSK4D9kandO-ELgFV23GVyi/view?usp=sharing`.
2. **Matches dataset** — match-level metadata. Download link used in the project brief: `https://drive.google.com/file/d/1tfdKTH39s8bhpRbY_Sz5FYO6IRPoFoeG/view?usp=sharing`.

> Place the unzipped/CSV files as `data/deliveries.csv` and `data/matches.csv` respectively.

---

## Data analysis questions (covered)

This project attempts to answer the set of analysis questions provided in the project brief, for example:

* Count of matches played in each season
* Total runs scored in each season
* Runs per match across seasons
* Umpire who umpired the most
* Team that won the most tosses and toss decisions
* Relationship between toss win and match win
* Teams that have won the tournament and their counts
* Teams with the most matches and highest winning percentage
* Lucky venue analysis for teams
* Innings-wise comparisons and 200+ scores
* Highest team totals and largest win margins
* Leading batsmen and bowlers (most runs, most balls, most 4s/6s, highest strike rate)
* Stadium with most matches hosted
* Most MOM (Player of the Match) awards
* Seasonal boundary counts and boundary-run contributions
* Powerplay (first 6 overs) and death overs (last 4 overs) comparisons

(Full, exact list of questions and phrasing are preserved in the project brief/notes.)

---

## Repository structure (recommended)

```
IPL-EDA/
├─ data/                    # store (or link to) raw CSVs (do NOT commit large raw data if not necessary)
│   ├─ matches.csv
│   └─ deliveries.csv
├─ notebooks/                # jupyter notebooks for exploratory work
│   └─ 01-ipl-eda.ipynb
├─ src/                      # helper scripts (data loading, cleaning, plotting)
│   ├─ data_utils.py
│   └─ analysis.py
├─ outputs/                  # generated figures, csv summaries, charts
├─ requirements.txt
├─ .gitignore
└─ README.md
```

---

## Setup & requirements

A minimal Python environment is recommended. Example packages used:

* Python 3.8+
* pandas
* numpy
* matplotlib
* seaborn
* plotly (optional)
* jupyter / notebook or jupyterlab
* scikit-learn (optional, if doing modeling)

Create `requirements.txt` with these packages so others can reproduce the environment.

---

## How to run (local)

1. Clone the repository (after you push it to GitHub) or copy the code locally.
2. Create and activate a virtual environment:

```bash
python -m venv venv
# macOS / Linux
source venv/bin/activate
# Windows (PowerShell)
venv\Scripts\Activate.ps1
```

3. Install requirements:

```bash
pip install -r requirements.txt
```

4. Prepare data: put `matches.csv` and `deliveries.csv` inside `data/` (or change paths in notebook/config).

5. Launch the Jupyter notebook and run cells in order:

```bash
jupyter notebook
# open notebooks/01-ipl-eda.ipynb and run
```

6. Alternatively run helper scripts (if included):

```bash
python src/analysis.py --input data/ --output outputs/
```

---

## Reproducible analysis notes

* Keep raw data in `data/` but do not commit large datasets to GitHub. Instead include a short sample or provide download instructions and dataset links in this README.
* Use `outputs/` to store generated images or CSV summaries. These can be committed if small.
* Record exact versions of packages in `requirements.txt` to reduce reproducibility issues.

---

## Outputs & Visualizations

The notebooks generate visual assets such as:

* Matches per season bar chart
* Runs per season and runs-per-match trends
* Toss-outcome and decision analyses
* Team-wise scoring patterns (powerplay vs death overs)
* Top batsmen and bowlers visualizations
* Venue-wise match counts and team success heatmaps

All final charts are saved to `outputs/figures/` by the notebooks/scripts.

---

## Good practices and notes

* Add `.gitignore` ignoring `venv/`, `data/` (if large), `.ipynb_checkpoints/`, `__pycache__/`.
* If datasets are large and you want to keep them in the repo, use Git LFS.
* Provide a `requirements.txt` and brief `CONTRIBUTING.md` if you expect collaborators.

---

## Contributing

Feel free to open issues or PRs. If you add new analyses, put them in `notebooks/` and export final charts to `outputs/`.

---

## License

Add a license file (e.g., MIT) to the repository. If unsure, consider `MIT` for permissive use.

---

## Contact

Author / maintainer: *Parshva Mehta*.

*README created for the IPL Data Analysis EDA project.*
# IPL_Data_Analysis_EDA
Exploratory Data Analysis (EDA) on IPL data using Python. The project covers data cleaning, preprocessing, and visualization to answer structured problem statements. Insights include team and player performance, toss impact, match outcomes, and seasonal trends, with reproducible Colab workflows.
