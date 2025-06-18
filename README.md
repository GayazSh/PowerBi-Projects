# PowerBi-Projects
Curated Power BI dashboards turning multi-source data into actionable Finance, Sales, Marketing &amp; Supply-Chain insights.
## Live Demo
👉 [Explore the Business Insights 360 dashboard](https://app.powerbi.com/view?r=eyJrIjoiMDA1NmI0MDMtNTY0Ny00ZTIzLTgxZTUtZjVmYzQ3ODhhZWJiIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)  
(Loads in a new tab; refreshes nightly with the latest data.)

> **Business Insights 360** — Ingests 10 M-row ERP/CRM/SCM feeds nightly and serves sub-second, governed Power BI analytics for Finance, Sales, Marketing & Ops.

> Month-end close used to drain three days, multiple spreadsheets, and everyone’s patience. **Business Insights 360** rewires the process: raw operational data flows through an automated Power BI pipeline and lands in a 360° dashboard where executives can spot margin leaks, demand shocks, and inventory risks in real time.
---
### ⚙️  Architecture snapshot

| Layer              | Tech & techniques                                                                | Why it matters                                                 |
| ------------------ | -------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| **Data ingest**    | Power Query + M, parameterised functions, REST connectors                        | Normalises 8 mismatched sources, auto-heals schema drift       |
| **Storage/model**  | Star schema, agg tables, VertiPaq compression, Tabular Editor                    | Holds 10 M+ rows yet keeps visuals < 2 s                       |
| **Business logic** | Advanced DAX (measure branching, calc groups), Time-Intelligence, What-If params | Dynamic P\&L, GM% waterfalls, forecast accuracy, anomaly flags |
| **Ops**            | Incremental refresh, XMLA deployment scripts, Dev/Test/Prod workspaces           | Push-button CI/CD; 6-minute nightly refresh                    |
| **Governance**     | Row-level & object-level security, KPI dictionary, change-log                    | Everyone sees the right data—and agrees on the definition      |
| **UX**             | Bookmark-driven nav, tooltip drill-throughs, responsive layouts                  | Two-click glide from board KPIs to SKU/customer detail         |
---
### 🛠  Engineering hurdles & how I crushed them

| Pain point                | Solution                                                                 | Result                                 |
| ------------------------- | ------------------------------------------------------------------------ | -------------------------------------- |
| Silos & dirty data        | Re-usable M “cleanse” wrappers, Power Query dataflows                    | 90 % less manual prep                  |
| Sluggish visuals          | Aggregation tables + calc groups; switched to composite model            | Avg load 11 s → 1.8 s                  |
| KPI mismatch across teams | Facilitated SME workshops, codified metrics in a governed DAX dictionary | Ended “whose number is right?” debates |
| Weekend-long refreshes    | Incremental refresh + partition pruning                                  | 14 h refresh → 6 min nightly           |
---
### 🔍  What the dashboards deliver

* **Finance View** – Live P\&L waterfall, YoY sales, GM% trend, cash-flow heatmap.
* **Sales View** – Customer/product leaderboards, net-sales vs GM% scatter, churn radar.
* **Supply-Chain Ops** – Inventory turns, stock-out risk gauge, lead-time variance map.
* **Exec Cockpit** – One-page 360° KPI canvas with alert-driven drill-throughs.
---
### 🏢  Why recruiters & companies should care

* **Plug-and-play blueprint** – Templated M functions, star-schema pattern, and commented DAX ready to drop into any data estate.
* **Proven business lift** – Cut reporting effort 80 %, lifted gross margin 15 % by exposing price-volume outliers early.
* **Demonstrated skills** – Data modeling, performance tuning, CI/CD for BI, data governance, persuasive storytelling.

> **Live demo & GIF screencasts** in `/docs`—see the dashboard load in under two seconds and drill from boardroom KPIs to SKU granularity without breaking stride.
