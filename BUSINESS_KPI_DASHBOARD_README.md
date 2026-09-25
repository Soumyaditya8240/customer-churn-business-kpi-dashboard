# Business KPI Dashboard — Customer Churn

## Objective
Build an interactive dashboard explaining **churn, retention, revenue risk, and customer segments** using the supplied cleaned customer churn dataset.

## KPI definitions
- **Churn Rate:** churned customers ÷ customers in the selected filter context.
- **Retention Rate:** 1 − churn rate.
- **Revenue at Risk:** monthly recurring charges (`MonthlyCharges`) belonging to customers whose `Churn` value is `Yes`.
- **Average Tenure:** average `TenureMonths` for customers in the selected filter context.
- **Customer Count:** number of customers in the selected filter context.

## Dashboard controls
The Excel dashboard provides dropdown filters for:
1. Contract type
2. Tenure band (0–12, 13–24, 25+ months)
3. Payment method

The KPI cards update from these selections.

## Visuals
- Churn rate by contract type
- Churn rate by payment method
- Churn rate by tenure band
- Monthly revenue at risk by contract type

## Sample-level findings
- Customers: **15**
- Churned customers: **7**
- Overall churn rate: **46.7%**
- Overall retention rate: **53.3%**
- Monthly revenue at risk: **₹409.93**
- Average tenure: **18.8 months**

### Contract breakdown
| ContractType   |   Customers |   Churned |   ChurnRate |   MonthlyRevenueAtRisk |
|:---------------|------------:|----------:|------------:|-----------------------:|
| Month-to-Month |           7 |         7 |           1 |                 409.93 |
| One Year       |           4 |         0 |           0 |                   0    |
| Two Year       |           4 |         0 |           0 |                   0    |

### Payment-method breakdown
| PaymentMethod   |   Customers |   Churned |   ChurnRate |   MonthlyRevenueAtRisk |
|:----------------|------------:|----------:|------------:|-----------------------:|
| Bank Transfer   |           3 |         0 |    0        |                   0    |
| Credit Card     |           6 |         2 |    0.333333 |                  99.98 |
| Debit Card      |           2 |         2 |    1        |                 159.98 |
| UPI             |           4 |         3 |    0.75     |                 149.97 |

### Tenure breakdown
| TenureBand   |   Customers |   Churned |   ChurnRate |   MonthlyRevenueAtRisk |
|:-------------|------------:|----------:|------------:|-----------------------:|
| 0–12 months  |           6 |         6 |         1   |                 329.94 |
| 13–24 months |           5 |         1 |         0.2 |                  79.99 |
| 25+ months   |           4 |         0 |         0   |                   0    |

## Interpretation notes
The sample contains only 15 records, so these are **descriptive sample patterns**, not population-level conclusions. Small segment sizes can produce extreme percentages; the dashboard therefore shows customer counts alongside rates.

## Submission contents
- `Customer_Churn_Business_KPI_Dashboard.xlsx` — interactive spreadsheet dashboard
- `customer_churn_sample.csv` — supplied dataset
- `BUSINESS_KPI_DASHBOARD_README.md` — definitions, methodology, and findings
