# Customer Retention & Churn Analysis

A business analysis identifying the strongest drivers of customer churn for a subscription-based telecom company, using real customer data, and translating findings into targeted retention recommendations.

## Business Problem

Leadership needs to understand why customers are leaving, which segments are highest-risk, and what actions could reduce churn and protect recurring revenue. This project answers that with a data-driven analysis, a visual dashboard, and a set of concrete recommendations.

## Approach

- Analyzed a dataset of 7,043 customers, including contract type, tenure, payment method, and service add-ons.
- Validated data quality (no missing values, no duplicate records) before analysis.
- Established an overall churn baseline of **26.5%** and measured key customer segments against it.
- Built a four-panel dashboard in Excel (PivotTables + PivotCharts) to visualize churn drivers.
- Synthesized findings into a one-page executive summary with prioritized recommendations.

## Key Findings

| Driver | Finding |
|---|---|
| **Contract Type** | Month-to-month customers churn at **42.7%**, vs. 11.3% (one-year) and 2.8% (two-year). This segment accounts for **88.5%** of all churned customers despite being only ~55% of the customer base — the single strongest churn driver identified. |
| **Customer Tenure** | New customers (0–6 months) churn at **52.9%** — roughly double the overall average — with churn risk declining steadily as tenure increases. |
| **Payment Method** | Customers paying by electronic check churn at **45.3%**, nearly 3x the rate of customers on automatic payment methods (bank transfer: 16.7%, credit card: 15.2%). |
| **TechSupport Enrollment** | Customers without TechSupport churn at **41.6%**, nearly 3x the rate of those who have it (15.2%) — suggesting TechSupport functions as a retention lever, not just a service add-on. |

**Highest-risk profile:** a new (0–6 month), month-to-month customer, paying by electronic check, without TechSupport.

## Dashboard

![Churn Analysis Dashboard](dashboard/dashboard_screenshot.png)

*Overall churn rate (26.5%) benchmarked against churn by contract type, tenure, payment method, and TechSupport enrollment.*

## Recommendations

1. **Target month-to-month customers** with incentives (discounted pricing, bundled services) to convert them to one- or two-year contracts — prioritizing customers in their first 6 months.
2. **Encourage automatic payment enrollment** at signup, and run targeted outreach to existing electronic-check customers.
3. **Promote/bundle TechSupport** for new and month-to-month customers as a low-cost retention lever.
4. **Build a proactive retention workflow** for the first 6 months of the customer lifecycle, when churn risk is highest.

## Assumptions & Limitations

- Churn is measured at a single point in time (a snapshot), not tracked longitudinally — this analysis does not capture seasonality or time-based trends.
- Revenue-at-risk was not quantified in dollar terms in this phase; a follow-on model could translate churn rate into revenue impact using average monthly charges.
- Findings are based on a public dataset intended for analysis practice and may not directly reflect any single company's live customer base.

## Tools Used

Excel (PivotTables, PivotCharts, data cleaning)

## Files in This Repository

```
├── data/
│   └── telco_customer_churn.csv          # Raw dataset
├── analysis/
│   └── churn_analysis.xlsx               # Full working file: pivot tables + dashboard
├── dashboard/
│   └── dashboard_screenshot.png          # Dashboard image (for this README)
└── Project1-Executive-Summary.docx       # Full write-up: problem, findings, recommendations
```

## Full Write-Up

See [Project1-Executive-Summary.docx](Project1-Executive-Summary.docx) for the complete business case, including detailed findings and recommendations.
