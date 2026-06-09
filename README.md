# 💰 Personal Finance Analysis

> End-to-end data analysis project using Python, MySQL, and Power BI — from raw Kaggle data to actionable financial insights.

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-orange?logo=mysql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-EDA-150458?logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

## 📌 Overview

This project analyzes personal finance data to identify spending patterns, savings behavior, and financial health trends. It covers the full data analysis lifecycle: data cleaning, exploratory analysis, SQL-based querying, and visualization in Power BI.

**Key questions answered:**
- Where does income go? Which expense categories dominate?
- What is the savings rate over time?
- Are there seasonal patterns in spending?
- Which months or categories represent the biggest financial risk?

---

## 🗂️ Project Structure

```
personal-finance-analysis/
│
├── data/
│   ├── raw/                     # Original dataset from Kaggle (unmodified)
│   └── processed/               # Cleaned dataset ready for analysis
│
├── notebooks/
│   └── 01_eda.ipynb             # Exploratory Data Analysis with pandas & matplotlib
│
├── sql/
│   ├── schema.sql               # Table creation and data loading
│   └── queries.sql              # Analysis queries (KPIs, aggregations, trends)
│
├── powerbi/
│   ├── dashboard.pbix           # Power BI report file
│   └── screenshots/             # Dashboard previews (PNG)
│
├── docs/
│   └── insights.md              # Key findings and business conclusions
│
└── README.md
```

---

## 📊 Dataset

**Source:** [Kaggle — BudgetWise Personal Finance Dataset](https://www.kaggle.com/datasets/mohammedarfathr/budgetwise-personal-finance-dataset)

| Field | Description |
|---|---|
| Date | Transaction date |
| Category | Expense or income category |
| Amount | Transaction amount (USD) |
| Type | Income / Expense |
| Description | Short transaction note |

> The raw dataset is stored in `data/raw/` and must not be modified. All transformations are applied in the notebook and saved to `data/processed/`.

---

## 🔧 Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.10+ | Data cleaning & EDA |
| pandas | Data manipulation |
| matplotlib / seaborn | Exploratory visualizations |
| MySQL 8.0 | Structured querying & KPIs |
| Power BI | Interactive dashboard |
| Jupyter Notebook | Analysis documentation |

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/iamjohitan/personal-finance-analysis.git
cd personal-finance-analysis
```

### 2. Install Python dependencies
```bash
pip install pandas matplotlib seaborn jupyter
```

### 3. Run the EDA notebook
```bash
jupyter notebook notebooks/01_eda.ipynb
```

### 4. Load data into MySQL
```bash
mysql -u root -p < sql/schema.sql
```
Then open `sql/queries.sql` in MySQL Workbench or your preferred client and run the queries.

### 5. Open the Power BI dashboard
Open `powerbi/dashboard.pbix` in Power BI Desktop. If prompted, update the data source path to your local `data/processed/` directory.

---

## 📈 Analysis Highlights

### EDA (Python)
- Distribution of income vs. expenses by month
- Top 5 spending categories
- Monthly savings rate calculation
- Outlier detection in transaction amounts

### SQL (MySQL)
- Total income and expenses by category
- Monthly balance trend
- Average daily spending
- Categories exceeding budget thresholds

### Dashboard (Power BI)
- KPI cards: Total Income, Total Expenses, Net Savings, Savings Rate
- Monthly trend line (income vs. expenses)
- Category breakdown (donut chart)
- Filterable by month, category, and transaction type

> 📸 Dashboard screenshots available in `powerbi/screenshots/`

---

## 💡 Key Insights

- **Rent and Food account for 52.46%** of all expenses — over half the budget goes to basic needs
- **Global savings rate is -16.92%** — expenses exceeded income across the full period
- **2023 was the only profitable year** with a net savings of +$3.47M; all other years ran a deficit
- **Expenses grew faster than income in 2024** despite it being the highest-income year ($39.4M), resulting in a -$3.8M deficit
- **Payment methods are evenly distributed** — Card (24%), Cash (24%), Bank Transfer (24%), UPI (23%)
- Dataset originally contained **47 category variants** and **4 date formats** — cleaned to 14 normalized categories

---

## 📁 Key Files

| File | Description |
|---|---|
| `notebooks/01_eda.ipynb` | Full EDA with charts and commentary |
| `sql/queries.sql` | 10+ analytical SQL queries with comments |
| `powerbi/dashboard.pbix` | Interactive Power BI report |
| `docs/insights.md` | Written summary of findings |

---

## 🤝 About

Project developed as part of a data analytics portfolio — targeting a **Junior Data Analyst** role.

**Author:** Johan Lucumi  
**LinkedIn:** [linkedin.com/in/johanlucumi](https://linkedin.com/in/johanlucumi)  
**GitHub:** [github.com/iamjohitan](https://github.com/iamjohitan)  
**Portfolio:** [johanlucumi.me](https://johanlucumi.me)

---

## 📄 License

This project is open source under the [MIT License](LICENSE).
