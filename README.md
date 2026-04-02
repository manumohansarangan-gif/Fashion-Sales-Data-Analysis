# 👗 Fashion Sales Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

## 📌 Project Overview
This project analyzes dress attributes and predicts whether a dress will be recommended based on sales data. The dataset contains attributes of dresses such as style, price, rating, season, material, and fabric type, along with customer recommendation data.

## 📁 Dataset Information
- **Source Format:** ARFF (Attribute-Relation File Format)
- **Tool Origin:** Weka Machine Learning Tool
- **Total Columns:** 13 (after renaming)
- **Target Variable:** Recommendation (1 = Recommended, 2 = Not Recommended)

### Columns
`Style` `Price` `Rating` `Size` `Season` `NeckLine` `SleeveLength` `Waistline` `Material` `FabricType` `Decoration` `PatternType` `Recommendation`

## 🛠️ Tools & Libraries Used
| Library | Usage |
|---------|-------|
| `scipy.io (arff)` | Loading the raw ARFF dataset |
| `NumPy` | Numerical operations, NaN handling |
| `Pandas` | Data cleaning, manipulation, aggregation |
| `Matplotlib` | Static visualizations |
| `Seaborn` | Statistical plots with KDE |
| `Plotly` | Interactive charts & heatmaps |

## 🔄 Project Workflow
- ✅ Data Loading & Decoding
- ✅ Data Cleaning (Missing values, spelling fixes, duplicates)
- ✅ Feature Engineering (RatingCategory, PriceLevel, IsRecommended)
- ✅ Filtering & Aggregation
- ✅ Univariate, Bivariate & Multivariate Analysis
- ✅ Correlation Analysis
- ✅ Outlier Detection & Removal

## 📈 Key Insights
- Ratings are concentrated between **4.5 – 4.8**
- **Casual style** is the most popular dress style
- Higher price does NOT guarantee higher ratings
- Seasonal combinations significantly influence recommendation

- 📁 Fashion-Sales-Data-Analysis/
├── Fashion_Sales_data.ipynb
├── fashions.csv
├── fashion_sales_cleaned.csv
└── README.md

## 👩‍💻 Author
> Data Analytics Assignment | Python | Pandas | Seaborn | Matplotlib | Plotly
