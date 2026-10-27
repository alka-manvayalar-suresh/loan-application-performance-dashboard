# Loan Application Performance Dashboard | Power BI

## 1. Project Overview

An interactive Power BI dashboard developed to analyse loan application performance from January to March 2026.

The dashboard evaluates loan application progression, monitors monthly activity, compares dealer performance, and identifies stages where conversion rates may require further investigation.

Using loan application and dealer mapping datasets, this project transforms operational data into key performance indicators (KPIs), visual reports, and actionable business insights to support management decision-making.

## 2. Business Problem

Loan applications progress through several stages before reaching disbursement. Monitoring application volumes alone does not provide sufficient insight into how effectively applications move through the process.

This analysis focuses on understanding application progression, identifying conversion drop-offs, monitoring monthly trends, and comparing dealer performance.

### Key Business Questions

- How many loan applications are received, approved, taken up, and disbursed?
- What percentage of applications progress through each stage?
- At which stage does the largest conversion drop-off occur?
- How do application and disbursement volumes change over time?
- Which dealers generate the highest take-up volumes?
- Which dealers have lower take-up-to-disbursement conversion rates?
- Where should management focus further investigation?

## 3. Project Objectives

- Monitor loan application volumes and progression through the application funnel.
- Measure approval, take-up, and disbursement conversion rates.
- Compare monthly application and disbursement activity.
- Evaluate dealer-level performance.
- Identify operational trends and areas for further investigation.
- Present findings through an interactive, management-focused dashboard.

## 4. Tools and Technologies

- **Microsoft Power BI:** Dashboard development and data visualisation.
- **DAX:** Calculation of KPIs and conversion rates.
- **Power BI Data Modelling:** Establishing relationships between application and dealer mapping tables.
- **Microsoft Excel:** Source data format.

## 5. Dataset and Data Model

The project uses two datasets.

### Order
Contains loan application information, including:
- Order number
- Application submission date
- Application state and state description
- Finance amount

### dealer_bd
Contains dealer mapping information, including:
- Order number
- Dealer name
- Business development (BD) name

The tables are connected using `order_no`, with a one-to-many relationship from `dealer_bd` to `Order`. This enables application records to be analysed by dealer.

## 6. Key Performance Indicators

The dashboard tracks four primary application stages.

| KPI | Result |
|---|---:|
| Total applications | 388 |
| Approved applications | 297 |
| Take-ups | 236 |
| Disbursed cases | 97 |

### Conversion Metrics

| Metric | Result |
|---|---:|
| Approval rate | 76.5% |
| Take-up rate among approved applications | 79.5% |
| Take-up-to-disbursement rate | 41.1% |
| Overall application-to-disbursement rate | 25.0% |

## 7. Dashboard Components

### KPI Cards
Summarise application volumes across the four main stages and display the take-up-to-disbursement rate.

### Monthly Application Volume vs Disbursed
Compares application and disbursement volumes over the reporting period.

### Loan Application Funnel
Visualises progression from applications to approvals, take-ups, and disbursements, highlighting conversion drop-offs.

### Dealer Take-up vs Disbursement
Compares take-up and disbursement volumes across dealers to highlight differences in performance.

### Management Summary and Key Insights
Highlights the main findings, areas requiring attention, and relevant data limitations.

## 8. Key Findings

### Application Funnel

Of 388 applications, 297 were approved, 236 progressed to take-up, and 97 reached disbursement.

The take-up-to-disbursement conversion rate was 41.1%, making this stage an important area for further investigation.

### Monthly Performance

- **January:** 204 applications and 57 disbursements.
- **February:** 148 applications and 35 disbursements.
- **March:** 36 applications and 5 disbursements.

March data covers activity only through 29 March 2026. Its lower recorded volume should therefore not be interpreted as a confirmed decline compared with the completed months.

### Dealer Performance

Take-up-to-disbursement conversion rates were:

- **Dealer A:** 53.0%
- **Dealer B:** 29.7%
- **Dealer C:** 60.0%

Dealer B generated the highest take-up volume, with 128 cases, but had the lowest take-up-to-disbursement conversion rate.

This highlights an opportunity to investigate differences in case progression. The available data does not establish the underlying causes.

## 9. Business Recommendations

1. **Monitor disbursement progression:** Track cases moving from take-up to disbursement to identify where additional drop-offs occur.
2. **Investigate dealer performance:** Examine potential factors contributing to Dealer B's lower conversion rate.
3. **Continue monthly monitoring:** Track future application and disbursement activity to determine whether the observed patterns persist.
4. **Evaluate volume and conversion together:** Consider both the number of cases handled and the proportion progressing successfully through the application process.

## 10. Project Outcome

This project demonstrates the use of Power BI to transform operational loan application data into an interactive performance dashboard.

By combining KPI tracking, funnel analysis, monthly trend comparisons, and dealer-level performance analysis, the dashboard provides a consolidated view of loan application progression and highlights areas for further management investigation.

## 11. Limitations

- The reporting period covers January to March 2026, with March data available only through 29 March.
- The analysis identifies performance differences but does not establish their underlying causes.
- The findings reflect the supplied dataset and reporting period.

