# 🌊 Plastics Pollution Explorer

**Course:** Exploratory Data Analysis  
**Instructor:** Ali Hassan Sherazi  
**Submission Date:** 05-June-2026  
**Dataset:** `plastics.csv` (Break Free From Plastic audit data, 2019–2020)

---

## 📋 Project Overview

An interactive data visualization dashboard analyzing global plastic waste collected during
Break Free From Plastic brand audit campaigns. The dataset covers **69 countries**, **2 years**
(2019–2020), and **13,380 records** identifying plastic pollution by type and corporate brand.

---

## 🚀 How to Run

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Make sure the dataset is in place

The file must be named **exactly** `plastics.csv` inside the `data/` folder:

```
dashboard_project/
├── data/
│   └── plastics.csv        ← EXACT filename, do NOT rename
├── app.py
├── charts.py
├── filters.py
├── requirements.txt
└── README.md
```

### 3. Launch the dashboard

```bash
streamlit run app.py
```

The dashboard will open at `http://localhost:8501` in your browser.

---

## 📊 Charts Included (All 10 Required)

| # | Chart | Insight |
|---|-------|---------|
| 1 | Pie Chart | Proportional split of plastic types (PET dominates) |
| 2 | Histogram | Right-skewed distribution of plastic counts |
| 3 | Line Chart | Year-over-year trend in total plastic collected |
| 4 | Bar Chart | Top 10 countries by plastic collected |
| 5 | Scatter Plot | Correlation between volunteers and plastic found |
| 6 | Box Plot | Spread and outliers in annual collection data |
| 7 | Heatmap | Feature correlation matrix |
| 8 | Area Chart | Cumulative plastic types stacked over years |
| 9 | Count Plot | Record frequency per year |
| 10 | Violin Plot | PET plastic distribution shape by year |
| ★ | Bonus Bar | Top 10 identified corporate polluters |

---

## 🔍 Filter Controls

- **Year** — Multi-select filter (2019 / 2020)
- **Country** — Multi-select across all 69 countries
- **Plastic Count Range** — Numerical slider on grand_total
- **Search** — Keyword filter on company or country name
- **Reset** — One-click reset to defaults

All filters update every chart simultaneously.

---

## 💡 Key Insights

1. **PET is the most common plastic type** — drink bottles and food containers dominate waste.
2. **Philippines leads in data collection** due to strong audit participation in 2019.
3. **The Coca-Cola Company is the top identified brand** after unbranded items.
4. **2019 has more records** than 2020, likely due to COVID-19 disrupting events.
5. **Volunteers and plastic found are positively correlated** — bigger teams collect more.
6. **Unbranded plastics account for the majority**, making corporate attribution challenging.

---

## 🛠️ Tech Stack

| Library | Role |
|---------|------|
| Python 3.x | Core language |
| Pandas | Data loading, cleaning, filtering |
| NumPy | Numerical operations |
| Matplotlib | Core chart rendering |
| Seaborn | Statistical charts & styling |
| Streamlit | Interactive frontend |

---

## 🚀 Deployment

### Option 1: Streamlit Cloud (Recommended ✨)

**Easiest & Free** — Deploy directly from GitHub in 2 minutes:

1. **Push to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Plastic Pollution Dashboard"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/plastic-pollution-dashboard.git
   git push -u origin main
   ```

2. **Deploy on Streamlit Cloud:**
   - Go to https://share.streamlit.io
   - Click **"New app"**
   - Select:
     - **GitHub repo:** `YOUR_USERNAME/plastic-pollution-dashboard`
     - **Branch:** `main`
     - **Main file path:** `dashboard_project/app.py`
   - Click **Deploy**

3. **Your live link:** `https://share.streamlit.io/YOUR_USERNAME/plastic-pollution-dashboard`

---

### Option 2: Heroku (Free tier may be deprecated)

1. Install Heroku CLI: https://devcenter.heroku.com/articles/heroku-cli
2. Login: `heroku login`
3. Create app: `heroku create your-app-name`
4. Deploy: `git push heroku main`

---

### Option 3: Railway / Render (Free alternatives)

Both support Streamlit apps with `requirements.txt`. Simply connect your GitHub repo.

---

## 📦 Project Structure

```
Plastic-Pollution-Dashboard/
├── .gitignore                    ← Git ignore rules
├── .streamlit/                   ← Streamlit config
│   └── config.toml
├── Procfile                      ← Heroku deployment config
├── pyproject.toml                ← Package metadata
├── README.md                     ← This file
└── dashboard_project/
    ├── app.py                    ← Main Streamlit app
    ├── charts.py                 ← Chart functions
    ├── filters.py                ← Data filtering functions
    ├── image_cards.py            ← Info card generation
    ├── requirements.txt          ← Python dependencies
    └── data/
        └── plastics.csv          ← Dataset (required)
```

---

## 🔐 Environment Variables (if needed)

For sensitive data in production, create `.streamlit/secrets.toml`:

```toml
# .streamlit/secrets.toml (DO NOT commit to GitHub)
[database]
url = "your_secret_db_url"
```

Access in code:
```python
import streamlit as st
db_url = st.secrets["database"]["url"]
```

---

## ⚠️ Troubleshooting

| Issue | Solution |
|-------|----------|
| `ModuleNotFoundError` | Ensure `requirements.txt` is in repo root or `dashboard_project/` |
| Data not loading | Verify `data/plastics.csv` is committed to GitHub |
| Port already in use | `streamlit run app.py --server.port 8502` |
| Slow dashboard | Try filtering to fewer countries/years first |

---

## 📝 License

MIT License — Feel free to use & modify for your projects.

---

## 👨‍💻 Author

**Ali Hassan Sherazi**  
Course: Exploratory Data Analysis  
Submission: 05-June-2026

For questions or issues, open a GitHub issue on the repo.
