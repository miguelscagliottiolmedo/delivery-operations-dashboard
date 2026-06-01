# Delivery Operations Dashboard

An operational dashboard for a delivery business, tracking SLA compliance, delivery volumes, and fulfillment funnels across **scheduled** and **on-demand** orders.

> *MealFlow is a fictional company created for this portfolio piece. All data is synthetic — no real or proprietary data is used.*

## What it shows
- **Top-line KPIs:** total deliveries, overall SLA met, average delivery time, active couriers — each with period-over-period change.
- **Volume + SLA by weekday:** combined bar (delivery count) and line (SLA %) charts, split by order type, to spot patterns across the week.
- **SLA breakdown:** scheduled vs. on-demand vs. overall, so operations can see where service levels slip.
- **Fulfillment funnels:** delivered on time / late / rescheduled / cancelled, per order type — to quantify where volume is lost.

## Why it's built this way
The design separates **scheduled** from **on-demand** orders because they behave differently operationally: scheduled deliveries are planned and hit higher SLA, while on-demand is more volatile and is usually where service levels drop. Surfacing both side by side lets an operations team target the right problem instead of looking at a blended average that hides it.

## Files
- `dashboard.html` — the dashboard preview (open in any browser)
- `dashboard_preview.png` — static image of the dashboard
- `mealflow_deliveries.csv` — granular synthetic dataset (delivery-level: date, order type, region, status, delivery time, SLA flag)
- `mealflow_summary_by_day.csv` — pre-aggregated summary by weekday and order type

## Tech
HTML/CSS preview · synthetic data generated in Python. A Power BI (.pbix) version built from the same dataset is in progress.

## About this piece
This dashboard recreates the *structure and design approach* of operational reporting I've built professionally, rebuilt from scratch with synthetic data so it can be shared freely. The skill on display is the dashboard design and the operational thinking behind it — not any specific company's data.

---
*By Miguel Scagliotti Olmedo · Product & Data Analyst*
