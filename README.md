# Minimising Revenue Leakage: Hotel Booking Cancellation Analysis

## 📌 The Business Challenge
In recent years, our client (a hospitality group managing both City Hotels and Resort Hotels) experienced a significant spike in booking cancellations [01.1350, 01.1351]. This directly resulted in vacant, unsold inventory, high upkeep costs, and reduced daily revenue [01.1355, 01.1356]. 

Instead of treating this as a simple, mechanical data exercise, this project centres around a core problem statement: **Why are customers cancelling, what macro-factors drive these decisions, and how can the business dynamically adjust operations to stabilise its bottom line?** [01.1285, 01.1360, 01.1364]

---

## 🛠️ The Technical Blueprint & Pipeline
Following corporate data practices, I structured the analysis into an end-to-end processing pipeline [01.1278]:

1. **Data Discovery & Cleaning (Python/Pandas):** 
   * Stripped out compromised PII (Personally Identifiable Information) columns to maintain strict data privacy compliance [01.1936, 01.1938].
   * Fixed critical formatting issues, explicitly casting standard string objects into proper `datetime` variables for chronological tracking [01.2137, 01.2154].
   * Handled massive missing metrics within agent and company fields [01.2652, 01.2693], and dropped minor null entries to prevent skewed calculations downstream [01.2727, 01.2735].
   * Isolated and removed extreme pricing outliers (such as single-day ADR values exceeding $5,000) that would warp our statistical aggregates [01.3008, 01.3032].

2. **Exploratory Visual Analysis (Matplotlib & Seaborn):**
   * Built dimensional distributions analysing the distinct correlation between price hikes and transaction cancellations [01.3216, 01.3346].
   * Generated multi-tier group visualisation plots to contrast seasonal fluctuations across business locations [01.4327, 01.4400].

3. **Strategic Business Reporting:**
   * Synthesised complex script logic into a structured executive brief designed directly for non-technical leadership and key stakeholders [01.1669, 01.1675].

---

## 📈 Commercial Findings & Data-Driven Insights

### 1. The Pricing Trap
Our visual trends explicitly validated that **Average Daily Rate (ADR) is the primary driver of cancellations** [01.1701, 01.1704]. When hotel rates peak, consumer second-guessing spikes, causing a domino effect of last-minute transaction drops [01.1601, 01.1603].

### 2. Debunking the Agent Hypothesis
Our baseline commercial assumption was that offline third-party travel agencies generated the majority of our booking volatility [01.1405, 01.1617]. **The data proved this wrong.** Over **56%** of our total guest volume originates from online travel portals, which simultaneously retain a **47%** cancellation share [01.5159, 01.5333]. This indicates an expectation gap where online platform imagery may not perfectly align with the on-site physical experience [01.5348, 01.5414].

### 3. Geographical Volatility
When aggregating cross-border data via targeted pie metrics, **Portugal** stood out immediately as our highest-risk market, accounting for **70% of total booking cancellations** [01.4947, 01.5019].

---

## 💡 Recommended Actions for Stakeholders
Based directly on the patterns uncovered, I proposed a three-pronged revenue defence strategy to management [01.1299]:

* **Dynamic Weekend Tiering:** Introduce rational, competitive promotional discounts during historic holiday or weekend price spikes to curb high cancellation tendencies [01.1711, 01.1712].
* **Winter Marketing Interventions:** Since January encounters peak cancellations alongside record-low general demand, launch targeted, early-bird marketing campaigns with flexible, non-refundable deposit terms specifically for winter cycles [01.4505, 01.1712].
* **Localized Infrastructure Investments:** Prioritise service quality controls, local marketing spending, and seasonal promotions specifically within the Portugal property portfolio to systematically drive down its 70% risk rate [01.5114, 01.5115].
