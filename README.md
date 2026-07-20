# Customer & Marketing Analytics

[![Python](https://img.shields.io/badge/Python-3.9+-blue?style=flat-square)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square)](https://jupyter.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-Clustering-green?style=flat-square)](https://scikit-learn.org)

Hi! Thanks for stopping by. This is an end-to-end analytics project I built to answer a question that matters to any retail business: *who are your customers, how do they behave, and what should you do about it?*

I worked with a synthetic dataset of 10,000 transactions across 1,986 customers and ran it through the full analytics pipeline — from raw data all the way to customer segments, retention analysis, and a KPI framework with actionable recommendations.

---

## 🔍 What I found

The headline number is that **46.5% of customers generate 66% of total revenue**. That's not unusual in retail, but it has a very specific implication: if you can identify those high-value customers early and keep them, the business impact is disproportionate.

Here are the key findings from the analysis:

**Revenue picture**
- $1,078,670 in total revenue across 10,000 orders
- $107.87 average order value, 18.38% profit margin
- Electronics and Office Supplies make up 60% of revenue — Furniture and Clothing contribute roughly equally for the remaining 40%

**Customer behaviour**
- 96.27% of customers made more than one purchase — strong signal of a loyal base
- RFM segmentation identified 7 distinct behaviour groups, from Champions to At-Risk
- K-Means clustering condensed this into 2 actionable segments: **VIP Customers** (924 customers, $714K revenue) and **At Risk** (1,062 customers, $365K revenue)

**Retention**
- Cohort analysis showed an 89.12% retention rate with a 10.88% churn rate
- Average days since last purchase: 81.6 days — the At Risk cluster averaged 113 days

---

## 📋 What's in the notebook

The analysis runs in a single Jupyter notebook (`Retail_Marketing_Analytics.ipynb`). Here's what each section is actually trying to answer:

- **Data Cleaning & Feature Engineering** — Built a clean, analysis-ready dataset from raw transaction records. Engineered 15+ features including delivery performance tiers, repeat customer flags, and sales quartiles — the kind of derived signals that make downstream segmentation meaningful.
- **Exploratory Analysis** — Established the baseline: how revenue is distributed across categories, regions, and time. Identified that sales are relatively stable month-over-month, which makes the segment-level differences more telling.
- **RFM Analysis** — Scored every customer on how recently they bought, how often, and how much. This gave a granular 7-group view of the customer base — useful for targeting, but too many segments to act on at once.
- **K-Means Clustering** — Condensed the RFM picture into 2 actionable segments. The business question this answers: *who do we focus on to protect revenue, and who do we focus on to grow it?*
- **Cohort Analysis** — Tracked whether customers acquired in a given month kept coming back. Retention stabilises around 27–35% after the first month, which tells you where the loyalty floor is.
- **CLV Modelling** — Estimated the long-term value of each customer to prioritise who's worth investing in through loyalty programmes or win-back campaigns.
- **KPI Framework** — Pulled everything into a set of 15+ business metrics with an executive summary — the kind of output you'd hand to a stakeholder who doesn't open notebooks.

---

## 💾 The data

I used a synthetic retail dataset modelled on real-world transaction structures. The raw data isn't included in the repo (too large), but all processed outputs — cleaned CSVs, RFM scores, segment labels, and KPI tables — are in `data/processed/`.

---

## 💻 Running it locally

```bash
git clone https://github.com/AbHi23d/retail-and-marketing-analytics.git
cd retail-and-marketing-analytics
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
