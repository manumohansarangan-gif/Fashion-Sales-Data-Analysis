👗Fashion Sales Data Analysis
<p align="center"> <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the￾badge&logo=python"/> <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?
style=for-the-badge&logo=jupyter"/> <img src="https://img.shields.io/badge/Status￾Completed-brightgreen?style=for-the-badge"/> </p>
📌Project Overview
This project analyzes dress attributes and predicts whether a dress will be recommended based
on sales data. The dataset contains attributes of dresses such as style, price, rating, season,
material, and fabric type, along with customer recommendation data.
Sales are monitored on the basis of alternate days. The project focuses on data cleaning,
exploratory data analysis (EDA), and visualization to uncover patterns in customer
preferences, pricing trends, and product recommendations.
📁Dataset Information
Detail Info
Source Format ARFF (Attribute-Relation File Format)
Tool Origin Weka Machine Learning Tool
Total Columns 13 (after renaming)
Target Variable Recommendation (1 = Recommended, 2 = Not Recommended)
📋Columns
Style , Price , Rating , Size , Season , NeckLine , SleeveLength , Waistline , Material ,
FabricType , Decoration , PatternType , Recommendation
🛠Tools & Libraries Used
Library Usage
scipy.io (arff) Loading the rawARFF dataset
NumPy Numerical operations, NaN handling
Library Usage
Pandas Data cleaning, manipulation, aggregation
Matplotlib Static visualizations (bar, histogram, scatter)
Seaborn Statistical plots with KDE
Plotly Interactive multivariate charts & heatmaps
🔄Project Workflow
✅Step 1: Data Loading
Loaded dataset from ARFF format using scipy.io.arff
Converted to Pandas DataFrame
Saved a copy as CSV for reference
✅Step 2: Data Cleaning
Decoded byte strings to UTF-8
Renamed columns to meaningful names
Replaced ? placeholders with NaN
Filled missing text columns with Mode
Replaced zero ratings (120 found) with Median
Fixed text casing and whitespace inconsistencies
Corrected spelling errors in Season , SleeveLength , Material , FabricType
Removed duplicate rows
Corrected data types for all columns
✅Step 3: Feature Engineering
Created 3 new derived columns:
RatingCategory — Poor / Good / Very Good / Excellent
PriceLevel — Numeric mapping of Price (1–5)
IsRecommended — Text label from Recommendation column
✅Step 4: Filtering & Aggregation
Filtered Recommended, Not Recommended, High Rated, Casual, and Summer dresses
Aggregated average ratings by Style and Season
Counted dress distribution by Style
✅Step 5: Exploratory Data Analysis (EDA)
📊Univariate Analysis
Rating distribution histogram
Recommendation, Style, Price, Season, Size bar charts
📊Bivariate Analysis
Rating vs Recommendation
Rating vs Season (line chart)
Rating vs Price (scatter chart)
Season vs Recommendation
Style vs Recommendation
📊Multivariate Analysis (Interactive — Plotly)
Style + Season vs Recommendation
Price + Season vs Average Rating
Style + Price vs Recommendation (heatmap)
✅Step 6: Correlation Analysis
Computed correlation matrix for Rating , Recommendation , Price_num
Visualized using an interactive Plotly heatmap
✅Step 7: Outlier Treatment
Used IQR method to detect outliers in the Rating column
Applied threshold-based removal (Rating < 3.5)
Verified dataset after removal
✅Step 8: Final Visualization
Plotted Rating Distribution after outlier removal using Seaborn histplot with KDE
📈Key Insights
📌Ratings are heavily concentrated between 4.5 – 4.8, showing overall positive customer
reception
📌Casual style is the most frequently occurring dress style
📌Higher price does not guarantee higher ratings — style and quality matter more
📌Seasonal combinations significantly influence recommendation rates
📌Rating and Recommendation show a weak-to-moderate positive correlation
📌After outlier removal, the dataset became cleaner and more consistent for analysis
✅Conclusion
This project successfully performed end-to-end data cleaning, feature engineering, and
exploratory data analysis on a Fashion Sales dataset. Starting from a rawARFF file with noisy,
inconsistent data, the dataset was transformed into a clean, analysis-ready format.
The EDA revealed that customer ratings are concentrated in the high range (4.5–4.8), suggesting
overall positive reception of the fashion catalog. However, recommendation is not solely driven
by rating or price — factors like style preference, season, and fabric play equally important roles.
This analysis provides a strong foundation for building a recommendation prediction model or
guiding inventory and design decisions based on actual customer preferences.
📂Project Structure
📁 Fashion-Sales-Data-Analysis/
├── Fashion_Sales_data.ipynb # Main Jupyter Notebook
├── fashions sales.csv # Raw dataset (CSV copy)
├── fashion_sales_cleaned.csv # Final cleaned dataset
└── README.md # Project documentation
👩‍💻Author
Final Year Data Analytics Assignment
Tools: Python | Pandas | Seaborn | Matplotlib | Plotly | Jupyter Notebook
