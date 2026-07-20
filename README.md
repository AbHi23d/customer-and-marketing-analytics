# Customer & Marketing Analytics

[![Python](https://img.shields.io/badge/Python-3.9+-blue?style=flat-square)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square)](https://jupyter.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-Clustering-green?style=flat-square)](https://scikit-learn.org)

Hi! Thanks for stopping by. This is an end-to-end analytics project I built to answer a question that matters to any retail business: *who are your customers, how do they behave, and what should you do about it?*

I worked with a synthetic dataset of 10,000 transactions across 1,986 customers and ran it through the full analytics pipeline, taking it from raw data all the way to customer segments, retention analysis, and a KPI framework with actionable recommendations.

---

## 🔍 What I found

The headline number is that **46.5% of customers generate 66% of total revenue**. That's not unusual in retail, but it has a very specific implication. If you can identify those high-value customers early and keep them, the business impact is disproportionate.

Here are the key findings from the analysis:

**Revenue picture**
- $1,078,670 in total revenue across 10,000 orders
- $107.87 average order value, 18.38% profit margin
- Electronics and Office Supplies make up 60% of revenue, while Furniture and Clothing contribute roughly equally for the remaining 40%

**Customer behavior**
- A 96.27% repeat purchase rate indicates a highly loyal customer base
- RFM segmentation identified 7 distinct behavior groups ranging from Champions to At-Risk
- K-Means clustering condensed this into 2 actionable segments: **VIP Customers** (924 customers, $714K revenue) and **At Risk** (1,062 customers, $365K revenue)

**Retention**
- 89.12% of customers remain active overall (haven't churned), while month-over-month cohort retention holds in a tighter 27–35% band — the first measures the whole customer base, the second tracks how consistently a given month's new customers keep coming back
- Average recency: 81.6 days overall — VIP customers average ~46 days between purchases, while the At Risk cluster averages 113 days

---

## 📋 Inside the analysis

The analysis runs in a single Jupyter notebook (`Retail_Marketing_Analytics.ipynb`). Here's what each section is actually trying to answer:

- **Data Cleaning & Feature Engineering**: I built a clean, analysis-ready dataset from raw transaction records. This involved engineering 15+ features (such as delivery performance tiers, repeat customer flags, and sales quartiles) to provide the derived signals needed for meaningful downstream segmentation.
- **Exploratory Analysis**: Establishing a baseline was the first step to understanding how revenue distributes across categories, regions, and time. Because sales are relatively stable month-over-month, any segment-level differences we find are much more telling.
- **RFM Analysis**: Every customer received a score based on how recently they bought, how often, and how much. The result was a granular 7-group view of the customer base.
- **K-Means Clustering**: To determine exactly who we should focus on to protect and grow revenue, I condensed the complex RFM picture into 2 actionable segments.
- **Cohort Analysis**: I tracked whether customers acquired in a given month kept coming back. Retention stabilizes around 27–35% after the first month, showing us exactly where the loyalty floor sits.
- **CLV Modeling**: Estimating the long-term value of each customer makes it easy to prioritize who is worth investing in through loyalty programs or win-back campaigns.
- **KPI Framework**: The final output pulls everything into a set of 15+ business metrics and an executive summary tailored for non-technical stakeholders.

---

## 💾 The data

I used a synthetic retail dataset modeled on real-world transaction structures. The raw data isn't included in the repo due to size constraints. However, all processed outputs (cleaned CSVs, RFM scores, segment labels, and KPI tables) are available in `data/processed/`.

---

## 💻 Running it locally

```bash
git clone https://github.com/AbHi23d/customer-and-marketing-analytics.git
cd customer-and-marketing-analytics
pip install -r requirements.txt
jupyter notebook Retail_Marketing_Analytics.ipynb
```

---

## 🛠️ Tech stack

Python · pandas · numpy · scikit-learn · matplotlib · seaborn · plotly

---

## 📧 Contact

**Abhinav Dhindsa**
- LinkedIn: [abhidhindsa](https://www.linkedin.com/in/abhidhindsa/)
- GitHub: [AbHi23d](https://github.com/AbHi23d)
- Email: dhindsaabhinav@gmail.com
