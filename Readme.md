# 🌍 Global Supply Chain Management Analytics

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1gnmRMrJvrHo4xPvNYJd4e6CDEL9Q3zQp?usp=sharing)  [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

> Transform raw shipment transactions into clear, prioritized actions that cut cost, shorten lead times, and reduce delivery risk — fast. 🚀

Why this project matters
- 🎯 Business-first analytics: speaks the language of procurement, logistics, and executives.
- 🔁 End-to-end & reproducible: notebooks, modular src/, tests, and requirements for easy handoff.
- 📊 Actionable deliverables: slide-ready charts, prioritized recommendations, and measurable KPIs.

Quick executive snapshot
- One-line: Convert transaction-level global trade data into a prioritized supplier + route action plan targeting the top spend drivers.
- Impact (example): Potential 15–25% freight savings; 8–12% improvement in on-time delivery. (Replace with your results.)

What’s included ✨
- notebooks/
  - 01_ingest_validate.ipynb — data schema + quality checks
  - 02_clean_transform.ipynb — cleaning, currency & date harmonization
  - 03_feature_engineering.ipynb — lead_time, cost_per_unit, flags
  - 04_eda_visuals.ipynb — KPI charts & maps (static + Plotly optional)
  - 05_recommendations.ipynb — prioritized actions & savings estimates
  - 06_optional_forecasting.ipynb — forecasting & delay classification
- src/ — reusable preprocessing & feature-engineering modules
- reports/ — exported PNGs, hero, and 5-slide demo deck (place final images here)
- data/ — sample (anonymized) CSVs and data dictionary
- requirements.txt, tests/, LICENSE, README.md

Core KPIs to present (slide-ready)
- 💸 Total Freight Cost
- ⚖️ Freight Cost per Unit
- ⏱️ Average Lead Time (days)
- ✅ On-time Delivery Rate (%)
- 🧾 Supplier Cost Contribution (%)
- 📦 Inventory Days of Supply

Analytical workflow (high-level)
1. Ingest & validate: schema checks, sample review, currency normalization. ✅  
2. Clean & standardize: missing data, dedupe, unit normalization. 🧹  
3. Feature engineering: lead_time, cost_per_unit, on_time_flag, rolling windows. 🔧  
4. EDA & diagnostics: distributions, outliers, correlation heatmaps. 🔍  
5. Visual storytelling: KPIs, supplier leaderboard, route maps. 🗺️  
6. Recommendations: prioritized actions (impact × effort), owners & timelines. 📝  
7. Optional: forecasting, supplier clustering, and optimization experiments. 🔮

Representative insights (replace placeholders)
- Top 10 suppliers account for ~62% of freight variance — consolidation opportunity. 📉  
- Hub-based routes show +18% lead time and +22% cost/unit vs direct lanes. 🔁  
- Electronics category: highest volatility; peak delays in Q3 annually. ⚡

Presentation & visuals — tips for a polished demo
- Use a 5-slide structure (title + executive summary, KPIs, cost drivers, risk & quick wins, next steps).  
- Export PNGs at 1920×1080 for slide insertion. 🖼️  
- Annotate each chart with a one-line takeaway and a numeric callout (e.g., "Top supplier contributes 32% of freight cost"). 🔔  
- Keep color palette consistent and colorblind friendly (example palette below).

Demo checklist ✅
- [ ] Replace hero and chart placeholders in reports/ with exported PNGs.  
- [ ] Include a small anonymized CSV in data/sample.csv so reviewers can run the notebooks.  
- [ ] Create a 5-slide deck using exported PNGs + EXECUTIVE_SUMMARY.md for talking points.  
- [ ] Validate notebook outputs and update representative numbers.

Example visual placeholders (put these in reports/):
- reports/hero.png — hero banner for README and deck cover  
- reports/kpi_trends.png — three-panel KPI trends (cost / lead time / on-time)  
- reports/supplier_pareto.png — Pareto bar chart for supplier spend  
- reports/leadtime_boxplot.png — lead time distribution by region/category

How to run (Colab — 3 steps)
1. Click the Colab badge and open the notebook.  
2. Upload or mount your dataset.  
3. Run notebooks in order — notebooks include checkpoints and sample outputs.

How to run (local)
1. python3 -m venv .venv && source .venv/bin/activate  
2. pip install -r requirements.txt  
3. Place CSV(s) into data/ and run notebooks or scripts in src/.

Polish & reproducibility
- Notebooks use deterministic seeds for models. 🔁  
- Add a data dictionary describing columns, types, units in data/ for reviewers. 📘  
- Avoid committing PII or supplier-sensitive data — use anonymized samples for public repos. 🔒

Next-phase extensions (prioritized)
- 🔹 Plotly Dash / Streamlit interactive dashboard for stakeholders  
- 🔹 Probabilistic forecasting (Prophet / deep learning) for demand & delay risk  
- 🔹 Optimization experiments: route consolidation & vendor reallocation simulation  
- 🔹 Operationalize with Airflow / Prefect for scheduled ingest & alerts

Contact & contribution
- Maintainer: pm1023 — https://github.com/pm1023 💬  
- Contributions welcome — open issues or PRs.  
- License: MIT

Small design note 🎨
- For immediate polish, add a hero banner (reports/hero.png) and create the 5 slide PNGs in reports/ with clear one-line takeaways beneath each image.

Data preprocessing and EDA pipelines can be modularized for automation.

Integration with Power BI / Tableau can enhance real-time visualization.

Predictive analytics (e.g., demand forecasting or delay prediction) can extend this project.
