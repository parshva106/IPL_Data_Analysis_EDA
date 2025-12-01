# 🏏 IPL Data Analysis — Exploratory Data Analysis (EDA)

### 📌 **Project Name:** IPL - Data Analysis (Exploratory Data Analysis)

A deep dive into statistics, patterns, and insights of the **Indian Premier League (IPL)** using real match and ball-by-ball datasets.

---

## 🔍 **Project Overview**

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on IPL datasets — uncovering hidden insights related to **teams, players, venues, toss decisions, scoring patterns, and outcomes**.
Using Python and Jupyter Notebooks, the analysis walks through structured problem statements supported by **visualizations and reports**.

---

## 📂 **Dataset Used**

The analysis is based on two core datasets (**place inside `data/` folder**):

| Dataset             | Description                   |
| ------------------- | ----------------------------- |
| 🏏 `deliveries.csv` | Ball-by-ball delivery dataset |
| 📄 `matches.csv`    | Match-level information       |

Download links (used in this project):
🔗 Deliveries — *Google Drive Link*
🔗 Matches — *Google Drive Link*

> After download, rename and save files as:
> `data/deliveries.csv` and `data/matches.csv` ✓

---

## ❓ **Key Data Analysis Questions Answered**

This project answers a wide range of IPL analytics questions including:

* 📅 Matches played per season
* 🏆 Tournament winners year-wise & total wins
* 🪙 Most toss-winning team & toss decision behaviour
* 🎯 Toss vs match win correlation
* 🦸 Most Player of the Match (MOM) awards
* 🏟 Stadium with the highest match count
* 💥 Highest team totals & biggest winning margins
* 🚀 Batsmen stats — most runs, 4s, 6s, strike rates
* 🎳 Bowler performance comparisons
* 🎇 Boundary contribution trends
* 🔥 Powerplay vs Death overs analysis
* 📍 Lucky venue analysis for teams

...and many more visual insights! 📊

---

## 🗂 **Repository Structure**

```
IPL-EDA/
├─ data/
│   ├─ matches.csv
│   └─ deliveries.csv
├─ notebooks/
│   └─ 01-ipl-eda.ipynb
├─ src/
│   ├─ data_utils.py
│   └─ analysis.py
├─ outputs/
├─ requirements.txt
├─ .gitignore
└─ README.md
```

---

## ⚙️ **Setup & Requirements**

### 🐍 Recommended Environment

* **Python 3.8+**
* pandas
* numpy
* matplotlib
* seaborn
* plotly *(optional, interactive charts)*
* jupyter / notebook / jupyterlab

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ **How to Run**

```bash
# create environment
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\Activate.ps1 # Windows

# open notebook
jupyter notebook
```

Open & run:

```
notebooks/01-ipl-eda.ipynb
```

Alternatively:

```bash
python src/analysis.py --input data/ --output outputs/
```

---

## 📈 **Outputs & Visualizations**

This project generates:

📊 Matches per season bar-charts
📊 Toss decision & impact plots
📊 Top batsmen & bowlers comparison graphs
📊 Venue-wise heatmaps
📈 Runs trend analysis across seasons

All visual results are saved to:

```
outputs/figures/
```

---

## 🧠 **Good Practices Followed**

✨ Clean modular notebook workflow
✨ Raw data separated & ignored in `.gitignore`
✨ Version locking via `requirements.txt`
✨ Reproducible analytics pipeline

---

## 🤝 Contributing

Contributions are always welcome!
Submit a PR or open an issue if you’d like to add more analyses.

---

## 📜 License

`MIT License` (recommended) — add `LICENSE` file in repo.

---

## 📬 Contact

👤 **Author / Maintainer:** *Parshva Mehta*
💼 *B.Tech — Electronics & Telecommunication Engineering*

---

## ⭐️ Final Note

If you like this project, don’t forget to **star ⭐ the repository** on GitHub —
it motivates further improvements and advanced analytics!

---

