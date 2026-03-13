# McDonald's South America Sales Dashboard

## 1. Project Background

This project was built to address a visibility gap common in regional sales operations: performance data existed across multiple markets, but there was no unified view that allowed leadership to assess progress against targets, compare country-level results, and understand customer satisfaction alongside financial outcomes — all in one place.

The dashboard consolidates sales, profit, customer volume, and satisfaction data across **seven South American markets** — Argentina, Colombia, Brazil, Ecuador, Peru, Chile, and Bolivia — into a single interactive Excel-based reporting tool. It is designed to give regional general managers and executive stakeholders an immediate read on where the business stands and which markets are driving or lagging performance.

The reporting scope covers **full-year 2022 actuals** alongside **2021 historical comparisons**, tracking progress toward annual targets across three core KPIs:

- **Sales:** $2,543.9M actual vs. $3,000M target (84.8% complete)
- **Profit:** $890.4M actual vs. $1,000M target (89.0% complete)
- **Customers:** 87M actual vs. 100M target (87.0% complete)

Insights and recommendations are structured around four key areas:

- **KPI Progress:** Where the business stands against annual targets
- **Sales Trajectory:** Year-over-year monthly trends and growth signals
- **Country Performance:** Which markets are leading and which need attention
- **Customer Satisfaction:** How operational quality scores map to revenue outcomes

---

## 2. Data Structure & Initial Checks

The workbook is structured across three sheets that together power the full dashboard view:

| Sheet | Description | Contents |
|---|---|---|
| **Dashboard** | Interactive visualization layer | Charts, KPI gauges, slicers, and summary visuals |
| **Inputs** | Core data model | KPI targets and actuals, monthly sales by year, sales by country, customer satisfaction scores |
| **Contacts** | Regional directory | General Manager names and email contacts for all 7 markets |

**Data Inventory — Inputs Sheet:**

```
KPI Tracking                     Monthly Sales Trend              Country Breakdown
─────────────────                ─────────────────────────        ─────────────────────────
Sales: Actual vs Target          Jan–Dec 2021 (Figures in $M)     Argentina     $953.3M
Profit: Actual vs Target         Jan–Dec 2022 (Figures in $M)     Colombia      $432.4M
Customers: Actual vs Target      YoY monthly comparison           Brazil        $553.2M
% Complete & Remainder           MoM pattern analysis             Ecuador       $445.1M
                                                                  Peru          $425.1M
Customer Satisfaction                                             Chile         $253.6M
─────────────────────────                                         Bolivia       $387.5M
Speed:        54%
Quality:      86%
Hygiene:      93%
Service:      53%
Availability: 95%
```

**Structural Notes:**
- Monthly sales figures are recorded in $M (millions) for both 2021 and 2022, enabling direct YoY comparison at every period
- KPI completion rates are formula-driven (Actual ÷ Target), ensuring the dashboard updates automatically when actuals are refreshed
- The Contacts sheet provides a direct escalation path by country — useful when dashboard metrics flag underperformance in a specific market
- Customer satisfaction scores are captured as decimals (0–1 scale) and displayed as percentages in the dashboard

![Sales Dashboard](https://github.com/YSayaovong/McDonald-South-America-Sales-Dashboard/blob/main/assets/Sales_Dashboard.png?raw=true)

---

## 3. Executive Summary

The 2022 South America sales dashboard shows a region tracking ahead of 2021 on an annual basis, with all three core KPIs within range of their targets. Total sales of **$2,543.9M** represent 84.8% of the $3,000M annual target. Profit of **$890.4M** is tracking at 89.0% of the $1,000M goal. Customer count sits at **87M**, or 87.0% of the 100M target.

| KPI | Actual | Target | % Complete |
|---|---|---|---|
| Sales | $2,543.9M | $3,000.0M | 84.8% |
| Profit | $890.4M | $1,000.0M | 89.0% |
| Customers | 87M | 100M | 87.0% |

**Country Performance — Sales by Market (2022):**

| Country | Sales ($M) | Share of Total |
|---|---|---|
| Argentina | $953.3 | 37.5% |
| Brazil | $553.2 | 21.8% |
| Ecuador | $445.1 | 17.5% |
| Colombia | $432.4 | 17.0% |
| Peru | $425.1 | 16.7% |
| Bolivia | $387.5 | 15.2% |
| Chile | $253.6 | 10.0% |

> **The core finding:** The region is performing solidly across all three KPI dimensions, but two dynamics deserve leadership attention. First, **Argentina alone accounts for 37.5% of total regional sales** — a concentration risk if that market softens. Second, **customer satisfaction scores show a significant split between operational dimensions**: hygiene (93%) and availability (95%) are strong, while speed (54%) and service (53%) are underperforming. These low scores on the two most customer-facing dimensions represent a brand risk and a likely ceiling on customer growth.

---

## 4. Insights Deep Dive

### 4a. 2022 Revenue Grew Across Every Month vs. 2021 — Strongest Gains in H2

**Metric:** Monthly Sales 2021 vs. 2022 (Figures in $M)

**Finding:** Full-year 2022 sales outpaced 2021 in every single month, with the YoY advantage growing in the second half of the year. The weakest months — May and June — still showed positive growth. The largest gains appeared in November ($222.3M vs. $205.2M, +$17.1M) and December ($225.8M vs. $204.3M, +$21.5M), suggesting strong seasonality in Q4.

| Period | 2021 ($M) | 2022 ($M) | YoY Change |
|---|---|---|---|
| Jan | 201.9 | 215.3 | +$13.4M |
| Feb | 204.2 | 217.6 | +$13.4M |
| Mar | 198.6 | 220.1 | +$21.5M |
| Apr | 199.2 | 206.4 | +$7.2M |
| May | 206.4 | 204.3 | −$2.1M |
| Jun | 195.3 | 203.0 | +$7.7M |
| Jul | 192.4 | 201.5 | +$9.1M |
| Aug | 186.3 | 200.6 | +$14.3M |
| Sep | 194.2 | 210.6 | +$16.4M |
| Oct | 199.0 | 216.4 | +$17.4M |
| Nov | 205.2 | 222.3 | +$17.1M |
| Dec | 204.3 | 225.8 | +$21.5M |

May is the one exception to the growth trend — 2022 dipped slightly below 2021 ($204.3M vs. $206.4M). Understanding whether this was a regional supply issue, a market-specific softness, or a promotional calendar gap would be worth investigating before 2023 planning.

---

### 4b. Argentina Drives More Than a Third of Regional Revenue — Concentration Risk Is Real

**Metric:** 2022 Sales by Country ($M)

**Finding:** Argentina generated **$953.3M** — more than Brazil ($553.2M) and Colombia ($432.4M) combined. At 37.5% of total regional sales, this level of market concentration means that any significant headwind in Argentina (currency volatility, regulatory change, demand softness) would materially impact regional performance even if all other markets hold their numbers.

The remaining six markets cluster between $253.6M (Chile) and $553.2M (Brazil), suggesting a relatively balanced mid-tier with Chile as a potential growth opportunity given its lower base.

For 2023 planning, a scenario that stress-tests regional performance under a 10–15% Argentina sales decline would clarify how much growth the other six markets would need to absorb to keep the region on target.

---

### 4c. Speed and Service Satisfaction Scores Are Critically Low — at 54% and 53%

**Metric:** Customer Satisfaction Scores by Dimension

**Finding:** Two of five customer satisfaction dimensions are underperforming significantly:

| Dimension | Score | Status |
|---|---|---|
| Availability | 95% | ✅ Strong |
| Hygiene | 93% | ✅ Strong |
| Quality | 86% | ✅ Acceptable |
| Speed | 54% | ⚠️ Critical |
| Service | 53% | ⚠️ Critical |

Availability (95%) and hygiene (93%) reflect well-managed operational standards. But speed and service — the two dimensions customers most directly experience in the transaction — are both below 55%. These scores indicate that nearly half of customers are leaving interactions dissatisfied on the dimensions most likely to influence repeat visit decisions.

This creates a specific risk: high availability draws customers in, but low speed and service scores create churn at the point of experience. Customer growth targets (87M vs. 100M target, 87% complete) may be harder to achieve if these scores are not addressed — it is easier to retain a customer than to acquire a new one in a market where the experience is inconsistent.

---

## 5. Recommendations

- **Conduct a country-level sales decomposition for Argentina.** Argentina's 37.5% share of regional revenue is a concentration that warrants its own risk analysis. Breaking down Argentina's $953.3M by quarter, product category, and store format would identify whether the dominance is structural (market size) or driven by factors that may not persist — and quantify how much buffer the other six markets provide if Argentina contracts.

- **Investigate the May 2022 dip before Q2 2023 planning.** May is the only month where 2022 sales fell below 2021 ($204.3M vs. $206.4M). Understanding the driver — whether promotional, operational, or demand-related — would prevent a repeat and clarify whether Q2 seasonality should be factored into 2023 targets differently than H1.

- **Prioritize speed and service improvement as a near-term operational initiative.** Satisfaction scores of 54% and 53% on the two most customer-facing dimensions are not rounding errors — they represent a structural experience gap. A focused initiative targeting order throughput times and front-line service quality, piloted in two or three high-volume markets, would provide a measurable test of whether score improvement translates to repeat customer growth.

- **Build a country-level target tracking tab into the dashboard.** The current KPI view tracks regional totals only. Adding a breakdown that shows each country's contribution toward the $3,000M sales target and $1,000M profit target — with running completion percentages — would give general managers direct accountability visibility and allow the regional team to identify which markets need intervention before year-end.

- **Set satisfaction score thresholds to trigger GM escalation.** Speed and service scores should carry alert flags in the dashboard: any dimension falling below a defined threshold (e.g., 60%) should automatically surface the relevant country GM contact from the Contacts sheet. This converts the dashboard from a passive report into an active management tool.

- **Model a Chile growth scenario for 2023.** With $253.6M in 2022 sales, Chile is the lowest-revenue market in the region — but also the market with the most headroom if unit economics are sound. A targeted review of Chile's store count, average check, and traffic trends relative to peers like Bolivia ($387.5M) and Peru ($425.1M) would determine whether Chile represents an underinvestment opportunity or a structurally smaller market.

---

## Tools Used

- Microsoft Excel (dashboard design, KPI gauges, data visualization, YoY comparisons)
- Power Query / Data Modeling (input normalization, structured data layer)
- Data visualization (donut charts, bar charts, line charts, satisfaction scorecards)
- Regional performance analysis (market concentration, YoY trend analysis, satisfaction benchmarking)

---

## Regional Contacts

| Country | General Manager | Email |
|---|---|---|
| Argentina | Facundo Gonzalez | f.gonzalez@mcdonalds.com |
| Colombia | Radamel Lopez | r.lopez@mcdonalds.com |
| Brazil | Joao Silva | j.silva@mcdonalds.com |
| Ecuador | Jaime Lomo | j.lomo@mcdonalds.com |
| Peru | Samuel Armando | s.armando@mcdonalds.com |
| Chile | Alvaro Sanchez | a.sanchez@mcdonalds.com |
| Bolivia | Angel Garcia | a.garcia@mcdonalds.com |
