# ESG-Financial-Performance-Analytics-Project


This project combines **Python** and **Power BI** to analyze the Environmental, Social, and Governance (ESG) performance of global companies and their correlation with financial metrics. It provides insights into sustainability leadership, ESG risks, and regional ESG patterns.

---

## 📊 Overview

We analyzed ESG scores and financial performance data for over 1,000 companies using:

- Python for data preprocessing, categorization, and exploratory analysis
- SQL for structured queries and performance aggregation
- Power BI for an interactive ESG dashboard

---

## 🧾 Dataset Description

- **`company_esg_financial_dataset.csv`**: Contains fields such as CompanyID, CompanyName, Industry, Region, Year, Revenue, ProfitMargin, MarketCap, GrowthRate, ESG_Overall, ESG_Environmental, ESG_Social, ESG_Governance, CarbonEmissions, WaterUsage, EnergyConsumption
- Data spans multiple years and covers global regions and industries.

---

## 📂 Project Structure
esg-financial-analysis
├── data/
|── company_esg_financial_dataset.csv
├── esg.ipynb # Python notebook for data analysis
├── ESG_Dashboard # Power BI dashboard
├── README.md

## 🛠 Technologies Used

- **Python**: pandas, matplotlib, seaborn
- **SQL**: data slicing, aggregation, and ESG metrics logic
- **Power BI**: KPI visuals, slicers, maps, charts
- **Excel** (initial data inspection)


## 📈 Python Analysis (Highlights)
In `esg.ipynb`:
- Categorized companies by ESG Score using `pd.cut`
- Generated ESG score distributions and box plots
- Performed correlation analysis between ESG scores and Profit Margin, Market Cap, Growth Rate
- Analyzed ESG scores across industries and regions

Example ESG categorization:
```python
df['ESG_Category'] = pd.cut(
    df['ESG_Overall'],
    bins=[0, 50, 75, 100],
    labels=['Low', 'Medium', 'High']
)


💡 Power BI Dashboard Features
ESG score trends by year and region
ESG category filters (Low / Medium / High)
ESG vs Revenue, Profit, Market Cap scatter plots
Industry-wise ESG comparison

