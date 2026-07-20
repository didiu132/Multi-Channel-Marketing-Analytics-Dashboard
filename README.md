# Multi-Channel Marketing Analytics Dashboard & Synthetic Data Engine

## 📌 Project Overview
This repository contains an end-to-end data analytics pipeline that generates a highly realistic, two-year (2023–2024) synthetic marketing dataset across multiple digital ad ecosystems. The generated data was used to architect a fully interactive executive marketing dashboard in Looker Studio, providing directors with real-time performance tracking and actionable data storytelling.

### 🔗 Live Resources
* **Interactive Dashboard:** [👉 Click Here to View My Looker Studio Dashboard](https://datastudio.google.com/s/pm7nM72pxNg)

---

## 🛠️ Data Engineering & Methodology
To mirror authentic corporate digital marketing data, the core Python generation engine bypasses simple randomized noise and simulates complex, cross-functional performance characteristics:

* **Temporal Seasonality:** Models structural real-world performance drops on weekends (-25% volume) alongside massive retail surges during Q4 holiday flights (Nov/Dec).
* **Multi-Channel Architecture:** Splits data tracking cleanly across four distinct mediums: Programmatic, Paid Search, Paid Social, and Organic layers.
* **Deterministic Campaign Profiling:** Weights metrics based on campaign intent. For example, high-intent Retargeting flights systematically yield vastly superior Conversion Rates (CVR) compared to broad top-of-funnel Awareness initiatives.
* **Financial Isolation:** Isolates organic discovery data (Google Search Console, Organic Social) from media expenditure algorithms, maintaining a strict $0.00 cost metric baseline.

---

## 📋 Schema Design & Architecture

| Dimension/Metric Name | Data Type | Behavioral Logic Included |
| :--- | :--- | :--- |
| **Date / Year / Month** | Temporal | Maps exactly 731 unique dates from Jan 1, 2023 to Dec 31, 2024. |
| **Channel / Data_Source**| Categorical | Structural mapping (e.g., StackAdapt mapped directly to Programmatic). |
| **Campaign_Name** | Categorical | Houses targeted strategies including Brand Core, Non-Brand, and DPA. |
| **Impressions** | Integer | Modelled utilizing a negative binomial distribution to replicate organic variance. |
| **Clicks / CTR** | Int / Float | Anchored to performance benchmarks (Search ~4.5% vs. Programmatic ~0.15%). |
| **Spend / CPC** | Float / Float | Dynamic micro-auctions dictate paid channel cost spikes. |
| **Conversions / CVR** | Int / Float | Highly optimized down-funnel scaling tied to high-intent targeting profiles. |
| **Revenue / ROAS** | Float / Float | Derived utilizing a standard baseline average transaction value of $85.00. |

---

## 📈 Key Business Insights Discovered
1. **Efficiency vs. Volume:** Paid Search commands a higher financial premium (higher CPC), yet its down-funnel conversion rate significantly outperforms top-of-funnel Programmatic awareness channels, resulting in a cleaner return on ad spend (ROAS).
2. **Seasonal Pacing:** Data structures clearly track and confirm aggressive Q4 scalability, allowing marketing teams to easily spot when to heavily shift budgets to maximize year-over-year growth.

---
