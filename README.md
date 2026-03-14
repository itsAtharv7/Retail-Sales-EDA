Retail Analytics: End-to-End Data Engineering & Business Intelligence Dashboard
This repository contains a comprehensive data analytics project focused on a retail sales dataset. The project covers the full data lifecycle—from handling "messy" raw data and performing advanced Exploratory Data Analysis (EDA) in Python to building an interactive Business Intelligence (BI) dashboard in Power BI.

🚀 Project Overview
The objective of this project is to transform raw retail transaction data into actionable business insights. By cleaning inconsistent data and applying statistical visualization techniques, we identify key drivers of profitability, sales performance across regions, and customer behavior patterns.

🛠 Tech Stack
Data Engineering: Python (Pandas, NumPy)

EDA & Visualization: Matplotlib, Seaborn

Business Intelligence: Microsoft Power BI

Environment: Jupyter Notebook / Anaconda

📂 Project Structure
Plaintext
Retail-Sales-Analysis/
│
├── data/
│   ├── messy_retail_dataset.csv     # Original raw data with inconsistencies
│   └── clean_retail_dataset.csv     # Exported after messeyretail.ipynb
│
├── notebooks/
│   ├── messeyretail.ipynb           # Data Cleaning & Preprocessing pipeline
│   └── cleanretaiEDA.ipynb          # Exploratory Data Analysis & Viz
│
├── EDA Plots/                       # Exported statistical visualizations
│   ├── sales_distribution.png
│   ├── profit_vs_discount.png
│   └── category_performance.png
│
├── dashboard/
│   └── retail_dashboard.pbix        # Interactive Power BI Dashboard
│
├── requirements.txt                 # Project dependencies
└── README.md

⚙️ Data Pipeline & Workflow

1. Data Cleaning & Preprocessing (messeyretail.ipynb)
The raw data was subjected to a rigorous cleaning pipeline to ensure integrity for downstream analysis:

Imputation Strategies: Handled missing values in Country and Region using mode-based imputation localized by geographical groups.

Data Type Standardization: Converted date fields into standardized datetime formats and ensured numerical consistency for Sales and Profit.

Inconsistency Resolution: Replaced "Unknown" placeholders with analytical nulls (NaN) for better statistical handling.

Constraint Validation: Removed duplicate records and filtered out erroneous data points.

2. Exploratory Data Analysis (cleanretaiEDA.ipynb)
Statistical analysis was performed to uncover hidden trends:

Profitability Drivers: Analyzed the inverse relationship between high discount rates and net profit margins.

Category Performance: Segmented sales and profit by product category (Accessories, Electronics, etc.) to determine top contributors.

Customer Segmentation: Identified top 5 high-frequency customers and tracked recent buyer behavior (recency analysis).

Correlation Matrix: Generated heatmaps to identify strong linear relationships between Quantity, Sales, and Profit.

3. Interactive Power BI Dashboard (retail_dashboard.pbix)
Developed a multi-dimensional dashboard providing:

Executive Summary KPIs: Total Sales, Total Profit, and Average Discount.

Regional Geospatial Analysis: Performance tracking across different global regions and countries.

Product Deep-Dive: Interactive filters to drill down into specific categories and products.

Shipping Mode Efficiency: Comparison of Standard, Express, and Same Day shipping on cost and delivery volume.

📊 Key Business Insights
Discount Optimization: Data indicates that aggressive discounting (above a certain threshold) leads to diminishing profit returns, particularly in the Electronics category.

Geographic Focus: The South and East regions show the highest volume of high-margin transactions.

Category Dominance: The Accessories category contributes significantly to the total profit percentage (approx. 50.15% in specific samples).

🛠 Installation & Usage
Clone the Repository:

Bash
git clone https://github.com/itsAtharv7/Retail-Sales-Analysis.git
cd Retail-Sales-Analysis
Install Dependencies:

Bash
pip install -r requirements.txt
Run the Analysis:

Execute notebooks/messeyretail.ipynb to regenerate the clean data.

Execute notebooks/cleanretaiEDA.ipynb to view the detailed visualization reports.

View Dashboard:

Open dashboard/retail_dashboard.pbix using Microsoft Power BI Desktop.

👤 Author
Atharv Kathar AI Engineer Intern | Rubixe AI [(https://www.linkedin.com/in/atharv-kathar)] 