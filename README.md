# Football-Matches-Analysis-using-Sheets-Tableau-and-Prediction-Model-using-Python
Analyzed 100+ football matches using custom-built entertainment, stat, and tension scores. Project includes a prediction model for match hype and Tableau dashboards for visualization. Built using Excel, Python, and Tableau to demonstrate data analytics, feature engineering, and ML fundamentals.
# ⚽ What Makes a Football Match Legendary?  
### 📊 A Data Analytics + ML Project on Football Match Hype & Drama

![License](https://img.shields.io/badge/license-MIT-green) ![Status](https://img.shields.io/badge/status-active-brightgreen) ![Made with](https://img.shields.io/badge/Made%20with-Python-blue)

> *"Some matches are forgettable, some live forever — this project finds out why."*

---

## 📌 Overview

This project explores **why certain football matches become iconic**, while others are instantly forgettable. By creating a **custom dataset** of 100+ matches and evaluating them on drama, dominance, and pre-match hype, we aim to answer:

> 🧠 *What makes a football match truly unforgettable?*

---

## 🧮 Scoring System

Each match is evaluated using **three original scores**:

- 🎬 **Entertainment Score**: Comebacks, late goals, VAR, penalties, red cards, etc.
- 📊 **Stat Score**: Possession, shots, passes, and other statistical dominance
- 🔥 **Tension Score**: Rivalries, derbies, stage of tournament, star players, etc.

Each score is calculated using logic-based rules in Excel/Sheets, with further modeling in Python.

---

## 🧠 Machine Learning Model

- **Model Goal**: Predict the match's **Tension Label** (e.g., *Ultra Hyped*, *Dead Fixture*)  
- **Approach**: Classification using `RandomForestClassifier`  
- **Input Features**: Rivalry, stage, past knockout encounters, leg info, team status, etc.  
- **Accuracy**: ~90% with 100+ matches (and improving with dataset growth)

---

## 📊 Visualizations

Interactive **Tableau Dashboards** highlight:
- Score distributions (ENT, STAT, TENSION)
- What contributes most to high/low tension
- Match classification summaries

> 🔗 https://public.tableau.com/views/FootballMatchAnalysis/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

---

## 🛠️ Tools & Tech

- **Excel / Google Sheets** – Data creation, scoring logic  
- **Python (Pandas, scikit-learn)** – ML modeling  
- **Matplotlib / Seaborn** – Visual exploration  
- **Tableau** – Final dashboards for insights

---

## 📁 Project Structure

```plaintext
📂 football-match-analysis/
├── data/
│   └── Main_dataset.csv                # Dataset with Statistic Score
│   └── Tension_context.csv              # Dataset with Tension score
│   └── Entertainment_context.csv        # Dataset with Entertainment Score
│   └── Comparison.csv                   # Dataset comparing Entertainment and Tension Scores to see if matches lived up to the hype
│   └── Tension_label.csv                # Match Metadata for Tension Score ML Model
├── notebooks/
│   └── football match tension prediction model.ipynb    # Google Colab for making a match hype prediction model
├── visualizations/
│   └── tableau_screenshots/            # Tableau dashboard exports
│   └── matplotlib_graphs/              # EDA and plots for individual features
├── README.md                           # Project description and documentation
├── model/
│   └── tension_model.pkl               # Trained model file for predicting tension labels
└── LICENSE                             # MIT license
