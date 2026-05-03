# 📊 Credit Risk Intelligence Dashboard

An interactive dual-dataset credit risk dashboard built with Python and Panel,
designed to analyze borrower behavior, loan default patterns, and demographic
risk profiles across two independent datasets.

![Dashboard Preview](assets/dashboard_preview.png)

---

## 🔍 Overview

This project builds a fully interactive browser-based dashboard that lets you
explore credit risk data through real-time filters and visualizations. It
combines two independent datasets — a modern Kaggle credit risk dataset and
the classic German Credit dataset — to provide a comparative view of financial
risk across different borrower profiles.

All charts update live as you adjust the filters — no need to re-run any code.

---

## 📁 Project Structure

credit-risk-dashboard/
│
├── credit_risk_dashboard.ipynb   # Main notebook — run this
├── credit_risk_dataset.csv       # Dataset 1 (Kaggle)
├── german_credit_data.csv        # Dataset 2 (German Credit)
├── requirements.txt              # Python dependencies
├── DATASET_INFO.md               # Column descriptions for both datasets
├── HOW_TO_RUN.md                 # Step by step setup guide
├── CHANGELOG.md                  # Version history
└── README.md

---

## 📊 Dashboard Features

### Filters (Sidebar)
- **Age Range Slider** — applies to both datasets simultaneously
- **Loan Intent** — filter by purpose of loan (Education, Medical, etc.)
- **Loan Grade** — filter by credit grade (A through G)
- **Loan Status** — toggle between Healthy and Default loans

### KPI Metrics (Top Row)
- Total number of loans in the filtered view
- Total loan exposure (sum of all loan amounts)
- Default rate as a percentage
- Average interest rate

### Visualizations — Dataset 1 (Credit Risk Dataset)
| Chart | What it shows |
|-------|---------------|
| Income vs Home Ownership | Income distribution across RENT, OWN, MORTGAGE |
| Default % by Credit Grade | How default rate climbs from Grade A to G |
| Loan Burden vs Default | Whether high loan-to-income ratio drives defaults |
| Risk Heatmap | Default rate by loan intent × loan grade combination |

### Visualizations — German Credit Dataset
| Chart | What it shows |
|-------|---------------|
| Default % by Gender | Demographic breakdown of default rates |
| Duration vs Credit Amount | Scatter of loan size vs duration, coloured by outcome |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| `pandas` | Data loading and manipulation |
| `panel` | Interactive dashboard framework |
| `matplotlib` | Base chart rendering |
| `seaborn` | Statistical visualizations |
| `Jupyter Notebook` | Development environment |

---

## 🚀 Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/Aryankumar16/credit-risk-dashboard.git
cd credit-risk-dashboard

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch the notebook
jupyter notebook credit_risk_dashboard.ipynb
```

Then go to **Kernel → Restart & Run All** and the dashboard will open
automatically in your browser.

> For detailed setup instructions see [HOW_TO_RUN.md](HOW_TO_RUN.md)

---

## 📂 Datasets

| Dataset | Source | Rows | Features |
|---------|--------|------|----------|
| Credit Risk Dataset | Kaggle | ~32,000 | 12 |
| German Credit Dataset | UCI ML Repository | 1,000 | 20 |

> For full column descriptions see [DATASET_INFO.md](DATASET_INFO.md)

---

## 📌 Academic Context

This dashboard was built as part of an academic data science project focused
on credit risk analysis and financial data visualization. It demonstrates
practical application of exploratory data analysis, interactive dashboard
design, and multi-dataset integration using Python.

---

## 👤 Author

**Aryan Kumar**
Lovely Professional University
