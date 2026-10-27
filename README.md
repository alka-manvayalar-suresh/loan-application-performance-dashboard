# Loan Application Performance Dashboard | Power BI

## 1. Project Overview

This project involved developing an interactive Power BI dashboard to analyse loan application performance from January to March 2026.

The dashboard was created as part of a Data Analyst interview assessment for X Star Technology. The objective was to evaluate loan application progression, monitor monthly activity, compare dealer performance, and identify areas where conversion rates could be improved.

Using loan application and dealer mapping datasets, I developed a dashboard that transforms raw operational data into key performance indicators (KPIs), visual reports, and actionable business insights for management.

## 2. Business Problem

Loan applications pass through multiple stages before reaching disbursement. Monitoring the number of applications alone does not provide enough information about how effectively applications progress through the process.

The business needs to understand:
- How many applications are received, approved, taken up, and disbursed?
- At which stage do the largest drop-offs occur?
- How does application and disbursement activity change over time?
- Which dealers generate the highest application and take-up volumes?
- Which dealers have lower conversion rates and may require further investigation?

This dashboard addresses these questions by presenting the loan application process in a single, interactive reporting view.

## 3. Project Objectives

- Monitor loan application volumes and progression through the application funnel.
- Measure approval, take-up, and disbursement conversion rates.
- Compare monthly application and disbursement activity.
- Evaluate dealer-level performance.
- Identify operational trends and potential areas for further investigation.
- Present findings through a management-focused dashboard.

## 4. Tools and Technologies

- **Microsoft Power BI:** Dashboard development and data visualisation.
- **DAX:** Calculation of KPIs and conversion rates.
- **Power BI Data Modelling:** Establishing relationships between the application and dealer mapping tables.
- **Microsoft Excel:** Source data format.

## 5. Dataset and Data Model

The project uses two datasets:

**Order**
- Order number
- Application submission date
- Application state and state description
- Finance amount

**dealer_bd**
- Order number
- Dealer name
- Business development (BD) name

The two tables were connected using `order_no`, with a one-to-many relationship from `dealer_bd` to `Order`.

This relationship enables application records to be analysed by dealer and supports dealer-level performance comparisons.

## 6. Key Performance Indicators

The dashboard tracks four primary application stages:

| KPI | Result |
|---|---:|
| Total applications | 388 |
| Approved applications | 297 |
| Take-ups | 236 |
| Disbursed cases | 97 |

The dashboard also reports the following conversion metrics:

| Conversion metric | Result |
|---|---:|
| Approval rate | 76.5% |
| Take-up rate among approved applications | 79.5% |
| Take-up-to-disbursement rate | 41.1% |
| Overall application-to-disbursement rate | 25.0% |

## 7. Dashboard Components

### KPI Cards
Provide a quick overview of application volumes across the four main stages and the take-up-to-disbursement conversion rate.

### Monthly Application Volume vs Disbursed
Compares monthly application and disbursement volumes to highlight changes in activity during the reporting period.

### Loan Application Funnel
Visualises the progression from applications to approvals, take-ups, and disbursements, making conversion drop-offs easier to identify.

### Dealer Take-up vs Disbursement
Compares take-up and disbursement volumes across dealers to highlight differences in operational performance.

### Management Summary and Key Insights
Presents the main findings, highlights areas requiring attention, and communicates the limitations of the available data.

## 8. Key Findings

### Application Funnel
Of 388 applications, 297 were approved, 236 progressed to take-up, and 97 reached disbursement.

The take-up-to-disbursement conversion rate was 41.1%, indicating that this stage warrants closer monitoring.

### Monthly Performance
January recorded the highest activity, with 204 applications and 57 disbursements.

February recorded 148 applications and 35 disbursements, while March recorded 36 applications and 5 disbursements.

March data was incomplete and covered activity only through 29 March 2026. Therefore, its lower recorded volume should not be interpreted as a confirmed decline relative to the full months.

### Dealer Performance
The take-up-to-disbursement conversion rates were:

- Dealer A: 53.0%
- Dealer B: 29.7%
- Dealer C: 60.0%

Dealer B generated the highest take-up volume, with 128 cases, but had the lowest take-up-to-disbursement conversion rate.

This difference highlights an area for further investigation, although the available data does not establish the underlying reasons.

## 9. Business Recommendations

1. **Monitor disbursement progression:** Track cases moving from take-up to disbursement to better understand where additional drop-offs occur.
2. **Investigate Dealer B's performance:** Review the lower conversion rate and examine potential factors affecting case progression.
3. **Continue monthly monitoring:** Track future application and disbursement activity to determine whether the observed patterns persist.
4. **Use conversion metrics alongside volume:** Evaluate both the number of cases handled and the proportion progressing successfully to gain a more complete view of performance.

## 10. Business Questions Answered

This dashboard helps management answer the following questions:

1. What is the overall volume of loan applications?
2. How many applications progress through each stage of the loan application funnel?
3. What percentage of applications are approved, taken up, and ultimately disbursed?
4. Which stage has the largest conversion drop-off?
5. How do application and disbursement volumes vary by month?
6. Which dealers generate the highest take-up volumes?
7. Which dealers have the lowest take-up-to-disbursement conversion rates?
8. Where should management focus further investigation to improve operational visibility?

## 11. Project Outcome

The project demonstrates how Power BI can be used to transform operational loan application data into an interactive performance dashboard.

By combining KPI tracking, funnel analysis, monthly trend comparisons, and dealer-level performance analysis, the dashboard provides a consolidated view of application progression and highlights areas for further management investigation.

## 12. Limitations

- The reporting period covers January to March 2026, with March data available only through 29 March.
- The analysis identifies differences in performance but does not establish their underlying causes.
- The findings are specific to the supplied assessment dataset and reporting period.

## Disclaimer

This project was completed as part of a Data Analyst interview assessment. The dashboard and accompanying documentation describe the analysis performed on the supplied data.
