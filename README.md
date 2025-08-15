# 💰 NY Budget Spent Dashboard (Tableau)

**Goal:** Provide a clear, interactive view of **New York State budget allocations vs. actual spending** across departments, programs, and time periods, enabling stakeholders to identify spending patterns, underspending, and overspending.

---

## 🔎 Problem Statement

Public budgets are large and complex, making it difficult to track whether allocated funds are used efficiently.  
This dashboard aims to:

1. Visualize **budget allocations vs. actual expenditures** across departments and categories.
2. Highlight **overspending and underspending** trends.
3. Enable **filter-driven exploration** by year, department, and spending category.

---

## 🎯 Objectives

- Integrate **budget and spending datasets** for the State of New York.
- Create **interactive dashboards** with filters for easy navigation.
- Provide KPIs, charts, and tables that make budget performance **transparent** and **actionable**.

---

## 🧩 Data Sources

| Source | Description | Format | Key Columns |
|--------|-------------|--------|-------------|
| NY State Budget Data | Budget allocations by department and year | CSV / Excel | Department, Year, Budget Amount |
| NY State Expenditure Data | Actual spending by department and year | CSV / Excel | Department, Year, Actual Spend |

> Data was sourced from New York's official **Open Data** portal.

---

## 🏗️ Workflow

1. **Data Cleaning & Preparation**  
   - Merged budget and expenditure data on `Department` + `Year`  
   - Calculated `% Utilization = (Actual Spend / Budget Amount) * 100`  
   - Flagged **overspending (>100%)** and **underspending (<90%)**

2. **Tableau Dashboard Development**  
   - Imported prepared data into Tableau  
   - Built views for:
     - Budget vs. Actual by Department
     - Year-over-Year trends
     - Top overspending and underspending departments
   - Added filters for **Year**, **Department**, and **Spending Category**

---

## 📈 Dashboard Features

### 1) **Budget vs. Actual Spend Overview**
- **KPI Cards** for:
  - Total Budget
  - Total Spend
  - % Utilization
- **Bar Chart**: Budget vs. Actual Spend by Department

---

### 2) **Trend Analysis**
- **Line Chart**: Year-over-Year spend trends
- **Highlight Table**: Departments with overspending/underspending trends

---

### 3) **Overspending / Underspending Insight**
- **Scatter Plot**: Budget vs. Spend with threshold lines
- Color-coded points for:
  - Overspending (Red)
  - Underspending (Blue)
  - On-target spending (Green)

---

## 🔧 Data Preparation Details

- **Standardization**
  - Unified Department names across budget and spending datasets
  - Ensured consistent date/year formatting
- **Derived Metrics**
  - % Utilization
  - Spending Variance (`Actual Spend - Budget Amount`)

---

## ▶️ How to Run / Use

1. Download the `.twbx` file from this repo.
2. Open in **Tableau Desktop** or **Tableau Public**.
3. Interact with:
   - **Year filter**
   - **Department filter**
   - **Spending Category filter**
4. Hover over bars or points to view detailed metrics.

---

## ✅ Early Insights

- Several departments showed **consistent underspending**, potentially due to unutilized project funds.
- A small number of programs exceeded their budgets, requiring **reallocation or review**.
- Year-over-year patterns reveal **spikes in certain years** tied to specific policy changes or funding boosts.

---

## ⚠️ Limitations

- Data covers only **reported budget and spending**; unreported adjustments are not included.
- Inflation adjustments not applied (future enhancement).
- Department name changes over time were harmonized but may not reflect historical naming.

---

## 🧭 Roadmap

- Add **forecasting models** to project next year’s spending trends.
- Include **per-capita spending analysis**.
- Integrate **interactive storytelling** with explanations of budget shifts.

---

## 📚 References

- New York State Open Data Portal – [https://data.ny.gov/](https://data.ny.gov/)

---

## 🧑‍💻 Contributors

- Leena Balagalu (https://github.com/LeenaBalagalu)


---

**Tip:** Add a screenshot of the dashboard at the top of this README for better recruiter impact.
