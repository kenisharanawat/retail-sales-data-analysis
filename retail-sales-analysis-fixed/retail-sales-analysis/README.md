# Retail Sales Analysis – 2023 Dataset

An exploratory data analysis project on a retail store's 2023 sales data covering 1,000 transactions across three product categories — Beauty, Clothing, and Electronics.

This is my third EDA project. I wanted to focus on understanding customer demographics and seasonal patterns this time, rather than just looking at revenue numbers.

---

## Questions I wanted to answer

- Which product category generates the most revenue?
- Do male and female customers shop differently?
- Is there a seasonal pattern — do certain months spike?
- Does age group affect what people buy?
- Which season drives the most sales?
- Is there a relationship between quantity bought and price per unit?

---

## Dataset

**Source:** [Retail Sales Dataset – Kaggle](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset)  
**File:** `data/retail_sales_dataset.csv`  
**Size:** 1,000 rows × 9 columns  
**Period:** January 2023 – January 2024

Columns: `Transaction ID`, `Date`, `Customer ID`, `Gender`, `Age`, `Product Category`, `Quantity`, `Price per Unit`, `Total Amount`

---

## Project structure

```
retail-sales-analysis/
│
├── data/
│   └── retail_sales_dataset.csv
│
├── notebooks/
│   └── retail_sales_analysis.ipynb
│
├── outputs/
│   └── (charts saved here when you run the notebook)
│
├── requirements.txt
└── README.md
```

---

## Key findings

1. **Electronics and Clothing are neck and neck** — Electronics ($156,905) just edges out Clothing ($155,580), with Beauty trailing at $143,515. No single category dominates.

2. **Female customers spend slightly more overall** — $232,840 vs $221,160 for males, and also purchase more items (1,298 vs 1,216). The gender split is almost 50/50 (51% female, 49% male).

3. **May is the strongest month by far** — $53,150 in sales, well above the monthly average of ~$38,000. September is the weakest at $23,620.

4. **Summer drives the most seasonal revenue** — Summer months consistently outperform Fall and Winter.

5. **Age doesn't strongly predict spending** — The average age is similar across all three product categories (~40–42 years). Young and old customers spend similar amounts.

6. **No outliers in Age** — IQR analysis showed the valid age range is −7 to 89, meaning all 1,000 customer ages (18–64) are within normal bounds.

---

## How to run

```bash
git clone https://github.com/kenisha-ranawat/retail-sales-analysis
cd retail-sales-analysis
pip install -r requirements.txt
jupyter notebook notebooks/retail_sales_analysis.ipynb
```

---

## Requirements

```
pandas
numpy
matplotlib
seaborn
jupyter
```

---

## What I'd explore next

- Add a profit margin column to see which category is actually most valuable, not just highest revenue
- Build a simple sales forecast for the next 3 months using moving averages
- Investigate why September is so weak — is it a data issue or a genuine seasonal dip?

---

*Learning project — part of my data science practice.*
