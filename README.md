# 🏠 Smart Real Estate Price Analysis

An end-to-end data analytics project that cleans a real-world housing dataset with missing values, explores it visually, and extracts business insights about what drives house prices in King County, USA.

---

## 📌 Project Overview

**Domain:** Real Estate Analytics | Data Analysis | Business Intelligence

**Objective:** Analyze housing market data to identify the key factors influencing house prices, handle missing values in messy real-world data, and present visual insights that support data-driven decisions for real-estate businesses, buyers, and investors.

---

## 📂 Dataset

| Item | Details |
|------|---------|
| **Name** | King County House Sales Dataset (with injected missing values) |
| **File** | `kc_house_data_NaN.csv` |
| **Records** | 21,613 |
| **Columns** | 22 |
| **Target variable** | `price` |
| **Sale period** | May 2014 – May 2015 |

**Key attributes**

- **Property size:** `sqft_living`, `sqft_lot`, `sqft_above`, `sqft_basement`
- **Structure:** `bedrooms`, `bathrooms`, `floors`
- **Quality:** `grade`, `condition`
- **Location:** `zipcode`, `lat`, `long`, `waterfront`, `view`
- **History:** `yr_built`, `yr_renovated`

---

## 🛠️ Tools & Skills

- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Skills:** Data Cleaning & Preprocessing, Missing Value Treatment, Exploratory Data Analysis (EDA), Data Visualization, Business Insight Generation

---

## 🔄 Project Workflow

### 1. Data Loading & Understanding
- Loaded the dataset and inspected shape, data types, and summary statistics.
- Identified numerical and categorical columns and detected missing values.

### 2. Data Cleaning
- Dropped the irrelevant index column `Unnamed: 0`.
- Found missing values in `bedrooms` (13) and `bathrooms` (10).
- Filled the missing values with the **mean** of each column.
- Converted the `date` column to proper `datetime` format.

### 3. Exploratory Data Analysis
Questions answered through visualizations:

1. What is the distribution of house prices? (histogram)
2. How does living area affect price? (scatter plot)
3. What is the relationship between bedrooms and price? (box plot)
4. Do bathrooms impact price? (scatter plot)
5. Does a waterfront view increase price? (box plot)
6. How do key variables correlate? (correlation heatmap)

---

## 📊 Key Findings

- **Prices are right-skewed.** Most homes fall in the low-to-mid range (median ≈ $450K), with a small number of very expensive properties (up to ≈ $7.7M).
- **Living area is the strongest price driver** among the variables analyzed (correlation with price ≈ 0.70).
- **Grade (build quality) matters a lot** (correlation ≈ 0.67).
- **Bathrooms matter more than bedrooms** (correlation ≈ 0.53 vs. ≈ 0.31).
- **Waterfront homes command a large premium.** Median price is about $1.4M for waterfront vs. $450K for non-waterfront.
- Views and renovations also tend to be associated with premium properties.

---

## 💡 Business Insights

- **Sellers / agencies:** Price listings primarily by living area, build grade, and location features such as waterfront.
- **Buyers:** Compare homes on size and quality rather than bedroom count alone.
- **Investors:** Waterfront and high-grade properties sit in the premium segment and show the highest prices.

---

## 📁 Repository Structure

```
├── Real_Estate_Price_Analytics.ipynb   # Main analysis notebook
├── kc_house_data_NaN.csv               # Dataset
└── README.md                           # Project documentation
```
