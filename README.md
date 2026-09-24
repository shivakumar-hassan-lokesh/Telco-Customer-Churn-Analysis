# Telco Customer Churn Analysis

Interactive Tableau dashboard analyzing customer churn for a telecom provider — covering 
churn drivers, financial impact, and the underlying reasons customers leave.

🔗 **[View Interactive Dashboard on Tableau Public](https://public.tableau.com/app/profile/shivakumar.hassan.lokesh/viz/TelcoCustomerChurnAnalysis_17612636787000/CustomerProfileAnalysis#3)**


## Overview

Customer churn directly erodes recurring revenue, and acquiring a replacement customer 
costs far more than retaining an existing one. This project analyzes 7,043 telecom 
customer records to identify who churns, why, and what it costs — with an interactive 
dashboard for drilling into any segment.

**Headline numbers:**
| Metric | Value |
|---|---|
| Total Customers | 7,043 |
| Churn Count | 1,869 (~26.5%) |
| Total Revenue | $21.37M |
| Total Charges | $16.06M |
| Average Monthly Charge | $64.76 |

## Dashboard Views

### 1. Overview
High-level KPIs plus churn rate broken down by contract type and payment method, a 
customer segmentation scatter (CLTV vs. contract vs. tenure), and a geographic view 
of churn by zip code across California.

- **Contract type is the single strongest churn signal:** Month-to-month customers churn at **42.71%**, vs. **11.27%** for one-year and just **2.83%** for two-year contracts.
- **Payment method matters:** Electronic check users churn at **45.29%** — nearly 3x the rate of automatic bank transfer (16.71%) or credit card (15.24%) users.

### 2. Customer Profile Analysis
Churn broken down by demographics (gender, senior citizen, partner, dependents), 
churn rate vs. tenure, and a monthly-vs-total-charges customer segmentation.

- Churn is fairly even by **gender** (939 female vs. 930 male) but skews toward customers **without dependents** (884 vs. 46) and **without a partner** (580 vs. 350).
- **Churn rate is highest in the first few months** of tenure and drops sharply as tenure increases — new customers are the highest-risk group.

### 3. Churn Reasons
A breakdown of *stated* reasons for churning, grouped into categories and ranked 
individually.

- **Competitor activity is the dominant driver**, accounting for 841 of all churn cases — more than double the next category (Attitude, 314).
- Top individual reasons: **competitor had better devices** (313), **competitor made a better offer** (311), and **attitude of the support person** (220).

### 4. Financial Impact
Revenue lost to churn, extra data/long-distance charge exposure, and how churn 
relates to customer lifetime value (CLTV) and churn-risk score.

- Churned customers represent **$3.68M** in revenue vs. **$17.69M** retained — roughly **17% of total revenue is tied to churned accounts**.
- **Fiber optic** internet service customers show a disproportionately high churn share compared to DSL, cable, or no internet service — worth flagging as a service-quality area to investigate.

## Key Insights

- **Contract length is the biggest lever for retention** — moving month-to-month customers to annual contracts could meaningfully cut churn.
- **Payment friction correlates with churn** — electronic check users churn far more than customers on autopay, suggesting a push toward automatic payment methods.
- **Churn is a "first year" problem** — retention efforts should concentrate on the first few months of the customer lifecycle.
- **Competitors, not price, are the main threat** — "competitor had better devices/offer" outweighs "price too high" as a stated reason, pointing to a device/offer competitiveness gap rather than a pure pricing issue.
- **Fiber optic churn deserves a service-quality review**, given its outsized share of churn relative to other internet service types.

## Tools Used

- **Tableau Public** — dashboard design and visualization
- SQL / Python — data cleaning and preparation

## How to Use

1. Click the Tableau Public link above to explore the live, interactive dashboard
2. Use the **Churn Label** filter (top right of each tab) to isolate churned vs. retained customers
3. Navigate between tabs using the left-hand icon rail (Overview, Customer Profile, Churn Reasons, Financial Impact)
4. Hover over any chart for detailed tooltips

## Author

**Shivakumar Hassan Lokesh** — MS Data Analytics Engineering, Northeastern University
