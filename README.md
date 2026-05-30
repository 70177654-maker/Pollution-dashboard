# 🌊 Plastics Pollution Explorer

**Course:** Exploratory Data Analysis  
**Instructor:** Ali Hassan Sherazi  
**Submission Date:** 05-June-2026  
**Dataset:** `plastics.csv` (Break Free From Plastic audit data, 2019–2020)

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/)

---

## 📋 Project Overview

An interactive data visualization dashboard analyzing global plastic waste collected during
Break Free From Plastic brand audit campaigns. The dataset covers **69 countries**, **2 years**
(2019–2020), and **13,380 records** identifying plastic pollution by type and corporate brand.

**Live Demo:** [Deploy on Streamlit Cloud](#-deployment)

---

## 🚀 Quick Start (Local)

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/plastic-pollution-dashboard.git
cd plastic-pollution-dashboard
```

### 2. Install dependencies
```bash
pip install -r dashboard_project/requirements.txt
```

### 3. Run the dashboard
```bash
streamlit run dashboard_project/app.py
```

The dashboard opens at `http://localhost:8501` 🌊

---

## 📊 Features

### 📈 17 Interactive Charts
- Pie Chart (Plastic Types)
- Histogram (Distribution)
- Line Chart (Time Trends)
- Bar Chart (Top Countries)
- Scatter Plot (Volunteers vs. Plastic)
- Box & Violin Plots (Statistics)
- Heatmap (Feature Correlations)
- Area Chart (Stacked Trends)
- Count Plot (Records per Year)
- Nested Donut (Type-Year Analysis)
- Country Pie Chart
- Efficiency Ranking
- Top Corporate Polluters ⭐

### 🎛️ Live Filters
- 📅 Year (2019 / 2020)
- 🌍 Country (69 countries)
- ♻️ Plastic Count Range
- 🙋 Volunteers Range
- 🧪 Plastic Type Focus
- 📊 Top N Results
- 🔎 Search (Company/Country)

### 💡 6 Analysis Tabs
1. **Overview** — Plastic types breakdown
2. **Trends** — Time-series analysis
3. **Geography** — Country performance
4. **Statistics** — Box plots, heatmaps, distributions
5. **Corporate** — Brand accountability
6. **Data** — Raw table explorer + CSV download

---

## 💡 Key Insights

1. **PET dominates** — Single-use bottles are the #1 plastic waste type globally
2. **Philippines leads** — Strong volunteer networks + high pollution levels
3. **Coca-Cola #1 brand** — Most frequently identified corporate polluter
4. **2019 > 2020** — COVID-19 disrupted audit campaigns worldwide
5. **Positive correlation** — More volunteers = more plastic collected
6. **Unbranded majority** — >50% of plastics lack corporate attribution

---

## 🚀 Deployment

### ⭐ Option 1: Streamlit Cloud (Recommended)

**Free, Fast, 2 Minutes**

1. **Push to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/plastic-pollution-dashboard.git
   git push -u origin main
   ```

2. **Go to:** https://share.streamlit.io
   - Click "New app"
   - Select your repository
   - Set main file path to: `dashboard_project/app.py`
   - Click "Deploy"

3. **Your live link:** `https://share.streamlit.io/YOUR_USERNAME/plastic-pollution-dashboard`

---

### Option 2: Heroku
```bash
heroku create your-app-name
git push heroku main
```

### Option 3: Railway / Render
- Connect GitHub repo directly
- Auto-deploys on push

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| Python 3.8+ | Core language |
| Pandas | Data processing |
| NumPy | Numerical computations |
| Matplotlib | Chart rendering |
| Seaborn | Statistical visualization |
| Streamlit | Web framework |

---

## 📦 Project Structure

```
plastic-pollution-dashboard/
├── .gitignore
├── .streamlit/
│   └── config.toml
├── Procfile
├── pyproject.toml
├── README.md
└── dashboard_project/
    ├── app.py              ← Main app
    ├── charts.py           ← 17 chart functions
    ├── filters.py          ← Data processing
    ├── image_cards.py      ← Info visualizations
    ├── requirements.txt
    └── data/
        └── plastics.csv    ← Dataset
```

---

## 📊 Dataset Info

**Break Free From Plastic (2019–2020)**
- **Records:** 13,380
- **Countries:** 69
- **Years:** 2 (2019, 2020)
- **Plastic Types:** 8 (PET, HDPE, LDPE, PP, PS, PVC, Other, Empty)
- **Columns:** 14 (country, year, parent_company, grand_total, volunteers, num_events, + plastic types)

---

## ⚠️ Troubleshooting

| Issue | Fix |
|-------|-----|
| `ModuleNotFoundError` | `pip install -r dashboard_project/requirements.txt` |
| `FileNotFoundError` (CSV) | Ensure `data/plastics.csv` exists in correct path |
| Port 8501 in use | `streamlit run dashboard_project/app.py --server.port 8502` |
| Streamlit stuck | Clear cache: `streamlit cache clear` |

---

## 📄 License

MIT License — Open for personal & educational use.

---

## 👤 Author

**Ali Hassan Sherazi**  
*Course: Exploratory Data Analysis*  
*Submission: June 5, 2026*

---

## 🤝 Contributing

Found a bug? Want to improve the dashboard?
1. Fork the repo
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📞 Support

- 📖 **Streamlit Docs:** https://docs.streamlit.io
- 🐛 **Issues:** Open an issue on GitHub
- 💬 **Discussions:** Start a discussion on GitHub

---

**Made with ❤️ for the environment** 🌍
