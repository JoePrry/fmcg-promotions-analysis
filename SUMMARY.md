# FMCG Promotions, Demand & Inventory Analytics

End‑to‑end commercial analytics project on a realistic synthetic FMCG dataset
(1.1M daily transactions, 5 countries, 2021–2023) from Kaggle. The work is
structured in **three parts**: pricing, demand planning, and inventory.

## Part 1 – Promotion Profitability

**Question:** Which discount levels actually create profit, by category and
country?

- Analyse units, revenue, margin and profit by discount bucket
  (no discount, 5–10%, 10–20%, 20–30%).
- Segment by country and category to find the profit‑maximising discount per
  segment.

**Output:** A concise discount playbook showing where deep discounts destroy
value despite higher volumes.


## Part 2 – Demand Forecasting for Promotions

**Question:** Can we forecast promotional demand accurately enough to plan
stock and avoid over/under‑ordering?

- Build SKU‑level daily demand features (lags, moving averages, calendar,
  promotion flags).
- Compare naïve baselines with a **Random Forest** model using time‑based
  train/test splits.

**Output:** Random Forest delivers ~**47% lower forecast error** than naïve
methods on high‑volume SKUs, providing a practical demand signal for
promotion planning.


## Part 3 – Inventory & Service Levels

**Question:** Where do stock‑outs and lead times stop promotions from
delivering their full uplift?

- Measure service levels (1 − stock‑out rate) by country, channel and SKU.
- Compare stock‑out rates on promo vs. non‑promo days to find
inventory‑critical segments.

**Output:** A targeted list of **high‑risk SKUs/channels** where stock‑out
probability more than doubles during promotions, with recommendations to
raise safety stock or adjust replenishment.

