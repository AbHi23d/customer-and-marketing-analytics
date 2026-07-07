# 🛍️ Customer & Marketing Analytics

> End-to-end data analytics project analyzing 10,000+ retail transactions to identify customer segments, track business performance, and surface actionable insights.

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green.svg)](https://pandas.pydata.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 📊 Project Overview

This project covers end-to-end analysis of retail transaction data — from data cleaning and exploratory analysis through to customer segmentation, cohort analysis, and dashboard creation.

### 🎯 Key Highlights

- **96.27% Repeat Customer Rate** across 1,986 customers
- **$1,078,670 Total Revenue** analyzed across 10,000 transactions
- **2 Customer Segments** identified through K-Means clustering
- **27+ Visualizations** and 9 analytical reports produced
- **27+ Visualizations** covering all analysis stages

---

## 🚀 Quick Start

### Prerequisites

```bash
Python 3.9+
pip (Python package manager)
```

### Installation

```bash
# Clone the repository
git clone https://github.com/AbHi23d/retail-marketing-analytics.git
cd retail-marketing-analytics

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook Retail_Marketing_Analytics.ipynb
```

---

## 📁 Project Structure

```
Project2_Retail_and_Marketing/
│
├── data/
│   ├── raw/                          # Original dataset (10,000 records)
│   └── processed/                    # Cleaned datasets
│       ├── cleaned_retail_sales.csv  # Main cleaned dataset (4.3 MB)
│       ├── rfm_analysis.csv          # RFM segmentation results
│       ├── customer_clv.csv          # Customer Lifetime Value data
│       ├── customer_segments.csv     # K-Means clustering results
│       └── monthly_kpis.csv          # Time-series KPIs
│
├── outputs/
│   ├── figures/                      # 27+ visualizations (PNG, HTML)
│   │   ├── 01_missing_values.png
│   │   ├── 07_sales_by_category.html
│   │   ├── 17_rfm_segments.html
│   │   ├── 20_customer_segments_3d.html
│   │   └── ...
│   │
│   └── reports/                      # Analytical reports
│       ├── executive_summary.txt
│       ├── 01_initial_inspection_report.txt
│       ├── 02_cleaning_report.txt
│       ├── 03_eda_key_findings.txt
│       └── ...
│
├── docs/                             # Data dictionary
│
├── Retail_Marketing_Analytics.ipynb  # Main analysis notebook
├── README.md                         # This file
├── requirements.txt                  # Python dependencies
└── .gitignore                        # Git ignore rules
```

---

## 🔍 Analysis Workflow

### 1️⃣ **Data Loading & Inspection**
- Loaded 10,000 retail transaction records
- Performed initial data quality assessment
- Generated data profiling reports

### 2️⃣ **Data Cleaning & Preprocessing**
- Handled missing values using median/mode imputation
- Removed duplicates
- Detected and treated outliers using IQR method
- Engineered 15+ features (time-based, revenue metrics, customer behavior)

### 3️⃣ **Exploratory Data Analysis (EDA)**
- **Univariate Analysis**: Distribution of numerical and categorical variables
- **Bivariate Analysis**: Category performance, regional analysis
- **Time Series Analysis**: Monthly trends, seasonality, quarterly comparisons
- **Customer Behavior**: Purchase frequency, top customers
- **Product Performance**: Top products, category profitability

### 4️⃣ **Advanced Analytics**

#### 🎯 RFM Analysis (Recency, Frequency, Monetary)
- Segmented customers into 7 categories:
  - Champions
  - Loyal Customers
  - Potential Loyalists
  - New Customers
  - At Risk
  - Lost Customers
  - Others

#### 🤖 K-Means Clustering
- Identified **2 primary customer segments**:
  - **At Risk**: 1,062 customers (53.5%) - $365K revenue
  - **VIP Customers**: 924 customers (46.5%) - $714K revenue

#### 📈 Cohort Analysis
- Tracked customer retention over time
- Retention rate: **89.12%**
- Churn rate: **10.88%**

#### 💰 Customer Lifetime Value (CLV)
- Average CLV: **$7,521.29**
- CLV/CAC Ratio: **150.43x** *(CAC was estimated using a fixed assumption since the dataset does not contain actual marketing spend data — this figure is inflated as a result)*

### 5️⃣ **KPI Framework**
- Defined a KPI framework covering 15+ business metrics
- Created interactive and static visualizations (Plotly HTML + PNG)
- Generated an executive summary report with findings and recommendations

---

## 📈 Key Business Findings

### Financial Performance
| Metric | Value |
|--------|-------|
| **Total Revenue** | $1,078,670.98 |
| **Total Profit** | $198,274.85 |
| **Profit Margin** | 18.38% |
| **Average Order Value** | $107.87 |

### Customer Metrics
| Metric | Value |
|--------|-------|
| **Total Customers** | 1,986 |
| **Repeat Customer Rate** | 96.27% ⭐ |
| **Customer Retention** | 89.12% |
| **Churn Rate** | 10.88% |
| **Avg Orders/Customer** | 5.04 |

### Product Performance
1. **Electronics**: $328K (30.4%)
2. **Office Supplies**: $321K (29.8%)
3. **Furniture**: $215K (19.9%)
4. **Clothing**: $214K (19.8%)

---

## 🛠️ Technical Stack

### Data Analysis & Processing
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **scipy** - Statistical analysis

### Machine Learning
- **scikit-learn** - K-Means clustering, preprocessing, PCA

### Visualization
- **matplotlib** - Static visualizations
- **seaborn** - Statistical graphics
- **plotly** - Interactive charts and dashboards

### Development Environment
- **Jupyter Notebook** - Interactive development
- **Python 3.9+** - Core programming language

---

## 💡 Key Insights & Recommendations

### 1. Customer Retention Strategy
**Insight**: 1,062 "At Risk" customers contributing $365K in revenue

**Recommendation**: 
- Launch targeted re-engagement campaigns
- Offer personalized discounts based on purchase history
- **Expected Impact**: 20-25% churn reduction

### 2. VIP Customer Program
**Insight**: 924 VIP customers (46.5%) generate $714K (66% of revenue)

**Recommendation**:
- Create exclusive loyalty program
- Provide early access to new products
- **Expected Impact**: 15-20% increase in VIP customer spend

### 3. Product Category Optimization
**Insight**: Electronics and Office Supplies dominate (60.2% of revenue)

**Recommendation**:
- Increase inventory for top categories
- Cross-sell complementary products
- **Expected Impact**: 10-15% revenue growth

### 4. Seasonal Marketing
**Insight**: Clear monthly and quarterly trends identified

**Recommendation**:
- Align marketing campaigns with peak seasons
- Prepare inventory for high-demand periods
- **Expected Impact**: 25-30% improvement in marketing ROI

---

## 📊 Sample Visualizations

### Customer Segmentation (3D View)
![Customer Segments](outputs/figures/20_customer_segments_3d.png)

### RFM Analysis
![RFM Segments](outputs/figures/17_rfm_segments.png)

### Monthly Revenue Trend
![Revenue Trend](outputs/figures/10_monthly_sales_trend.png)

### Category Performance
![Category Performance](outputs/figures/16_category_performance.png)

---

## 🎓 Skills Demonstrated

### Technical Skills
- ✅ Data Cleaning & Preprocessing
- ✅ Exploratory Data Analysis (EDA)
- ✅ Statistical Analysis
- ✅ Machine Learning (K-Means Clustering)
- ✅ Feature Engineering
- ✅ Data Visualization

### Business Skills
- ✅ Customer Segmentation
- ✅ RFM Analysis
- ✅ Cohort Analysis
- ✅ Customer Lifetime Value (CLV) Calculation
- ✅ KPI Design & Tracking
- ✅ Stakeholder Communication
- ✅ Business Recommendations

### Tools & Technologies
- ✅ Python (pandas, numpy, scikit-learn, plotly)
- ✅ Jupyter Notebook
- ✅ Git & GitHub
- ✅ Data Visualization (matplotlib, seaborn, plotly)

---

## 📧 Contact

**Abhinav Dhindsa**  
- LinkedIn: [abhidhindsa](https://www.linkedin.com/in/abhidhindsa/)
- GitHub: [AbHi23d](https://github.com/AbHi23d)
- Email: dhindsaabhinav@gmail.com

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Dataset source: [Kaggle - Retail Sales Dataset](https://www.kaggle.com/)
- Inspiration: Real-world retail analytics challenges
- Tools: Python community, scikit-learn, plotly, Power BI

