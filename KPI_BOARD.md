# Olist Project — KPI Board
Last updated: Day 1

---

## Business Question
"Where exactly is revenue leaking — and which customers are worth saving?"

---

## Hypothesis
Revenue plateau is driven by repeat purchase failure, not acquisition failure.
Delivery delays explain the 1-star concentration.

## Proof:"Day 1 I noticed total orders and unique customers were almost identical — only 3,345 difference across 2 years of data. In a healthy e-commerce business that gap should be much larger. That told me retention was broken before I wrote a single SQL query."

**Evidence from Day 1:**
- 99,441 total orders
- 96,096 unique customers
- Difference = 3,345 repeat orders
- Estimated repeat purchase rate = ~3.5%

**Translation:** 96.5% of customers buy once and never return.
This is the core business problem.

---

## KPIs

### Scale
| Metric | Value | Status |
|--------|-------|--------|
| Total orders | 99,441 | ✅ |
| Unique customers | 96,096 | ✅ |
| Delivered orders | 96,478 (97.0%) | ✅ |
| Total revenue | R$19,881,945 | ✅ |
| Average order value | R$206.08 | ✅ |

### Retention
| Metric | Value | Status |
|--------|-------|--------|
| Repeat purchase rate | ~3.5% (estimated) | ⬜ confirm in SQL |
| Month-2 cohort retention | TBD | ⬜ Day 4 |
| At-Risk RFM % | TBD | ⬜ Day 4 |
| At-Risk RFM revenue | TBD | ⬜ Day 4 |

### Operations
| Metric | Value | Status |
|--------|-------|--------|
| Late delivery rate | 6.8% | ✅ |
| Avg delay when late | 10.6 days | ✅ |
| Delay vs review score | TBD | ⬜ Day 2 SQL |

### Satisfaction
| Metric | Value | Status |
|--------|-------|--------|
| 5-star rate | 57.8% | ✅ |
| 1-star rate | 11.5% | ✅ |
| Avg review score | TBD | ⬜ Day 2 SQL |

### Revenue
| Metric | Value | Status |
|--------|-------|--------|
| MoM revenue trend | TBD | ⬜ Day 2 SQL |
| Top category by revenue | TBD | ⬜ Day 2 SQL |
| Funnel drop-off % | TBD | ⬜ Day 2 SQL |
| Checkout conversion rate | TBD | ⬜ Day 2 SQL |

---

## Resume Bullets Progress

- [ ] Bullet 1 — funnel drop-off number
- [ ] Bullet 2 — At-Risk RFM revenue number  
- [ ] Bullet 3 — delivery vs review score number
- [ ] Bullet 4 — repeat purchase rate confirmed

---

## Daily Log
- Day 1 ✅ — Data loaded, cleaned, master df built (119K rows, 37 cols)
- Day 2 ⬜ — SQL analysis
- Day 3 ⬜ — Python EDA + funnel
- Day 4 ⬜ — RFM segmentation
- Day 5 ⬜ — Power BI dashboard
- Day 6 ⬜ — Recommendations + README