<p align="center">
  <img
    src="https://readme-typing-svg.demolab.com?font=Space+Grotesk&weight=700&size=36&pause=1500&color=D1ECFC&center=true&vCenter=true&width=950&lines=MavenTech+Sales+Analysis"
    alt="MavenTech Sales Analysis"
  />
</p>

<p align="center">
  CRM insights for sales managers through an interactive Power BI dashboard.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-D1ECFC?style=for-the-badge&logo=powerbi&logoColor=262626" />
  <img src="https://img.shields.io/badge/Power%20Query-D1ECFC?style=for-the-badge&logoColor=262626" />
  <img src="https://img.shields.io/badge/DAX-C298C9?style=for-the-badge&logoColor=262626" />
  <img src="https://img.shields.io/badge/CRM%20Analytics-F1B4DF?style=for-the-badge&logoColor=262626" />
</p>

---

### Dashboard Preview

https://github.com/user-attachments/assets/5a904c9a-2333-44a6-a549-7937fd73afe8

> The dashboard supports quarterly sales reviews, team comparisons and open-opportunity follow-up.

---

## About the Project

MavenTech is a fictional B2B computer hardware company.

I built an interactive Power BI dashboard to simulate a quarterly sales review, giving managers a way to track their team’s performance, compare results with other teams and explore which products and customers drove sales.

A dedicated pipeline page lets managers review open opportunities and identify deals for follow-up.

---

## Key Assumptions

I used the quarterly sales review as the starting point. Since MavenTech is fictional, I based the design on five questions a sales manager might ask:

- **How is my team doing this quarter?**
- **Which agents might need support, and where?**
- **Where did our sales come from?**
- **How does my team compare with the rest of the company?**
- **Which open deals should I review first?**

These questions guided the dashboard’s filters, KPIs and comparisons.

---

## Dataset

I downloaded the **CRM Sales Opportunities** dataset from Kaggle.

It contains **8,800 sales opportunities**, with dates spanning **2016–2017**, plus lookup tables for customer accounts, products and sales teams.


| Table | Contents |
| --- | --- |
| Sales pipeline | Opportunity IDs, accounts, products, sales agents, deal stages, engagement dates, close dates, close values and estimated deal values |
| Accounts | Account names, sectors, revenue, employee counts, office locations, parent companies and years established |
| Products | Product names, series and sales prices |
| Sales teams | Sales agents, managers and regional offices |
| Data dictionary | Source table names, field names and descriptions |

**Sources:** [Kaggle dataset](https://www.kaggle.com/datasets/innocentmfa/crm-sales-opportunities) · [Original Maven Analytics challenge](https://mavenanalytics.io/challenges/maven-sales-challenge)

---

## Main Features

- Quarterly sales KPIs and performance comparisons
- Team and sales-agent performance analysis
- Product and customer contribution analysis
- Company benchmarks for team comparisons
- Dedicated open-pipeline review
- Interactive filters for exploring results

---

## Tech Stack

<p>
  <img src="https://img.shields.io/badge/Dashboard-C298C9?style=for-the-badge&logoColor=262626" />
  &nbsp;&nbsp;&nbsp;:&nbsp;&nbsp;&nbsp; Power BI
</p>

<p>
  <img src="https://img.shields.io/badge/Data%20Preparation-F1B4DF?style=for-the-badge&logoColor=262626" />
  &nbsp;&nbsp;&nbsp;:&nbsp;&nbsp;&nbsp; Power Query
</p>

<p>
  <img src="https://img.shields.io/badge/Calculations-D1ECFC?style=for-the-badge&logoColor=262626" />
  &nbsp;&nbsp;&nbsp;:&nbsp;&nbsp;&nbsp; DAX · KPIs · Quarterly Comparisons · Benchmarks
</p>

<p>
  <img src="https://img.shields.io/badge/Analytics-C298C9?style=for-the-badge&logoColor=262626" />
  &nbsp;&nbsp;&nbsp;:&nbsp;&nbsp;&nbsp; Data Modelling · Sales Analysis · Interactive Visualisation
</p>

---

## Data Preparation and Modelling

I used **Power Query** to prepare the source data and **DAX** to calculate KPIs, quarterly comparisons and benchmarks.

### Data preparation

- Promoted headers, checked column names and standardised inconsistent names across tables
- Assigned appropriate data types to identifiers, dates and values
- Reviewed blank values in the context of each opportunity’s deal stage
- Prepared the pipeline and lookup tables for analysis

### Data model

The sales pipeline acts as the central fact table, connected to lookup tables for accounts, products and sales teams.

<img width="756" height="467" alt="Screenshot 2026-11-05 at 11 04 05" src="https://github.com/user-attachments/assets/7aa712d4-ba55-4b6a-9c41-12c8fc3438ff" />


---

## Dashboard Analysis

### Sales Opportunity Overview

This is the main page for sales managers. Users select a manager, year, and quarter to review their team’s performance. KPI cards show revenue, wins, average sale value, time to close, and engaged opportunities. Prior-quarter figures and company benchmarks appear beneath the relevant KPIs to give managers context for their results.
The agent heatmap helps managers spot differences in performance across their team. The product table shows sales and win rates side by side, so managers can see which products bring in the most revenue and which convert most often.

<img width="1004" height="559" alt="Screenshot 2026-11-05 at 11 13 09" src="https://github.com/user-attachments/assets/04a19b97-b14c-4a02-afb1-b4a566985558" />


### Open Opportunities Report

Users select a manager to view their team’s engaged opportunities. The table shows the sales agent, product, account where available, engagement date, and estimated value. Managers can sort by engagement date to find older opportunities that may need follow-up, or by estimated value to review the largest opportunities first.

<img width="1004" height="559" alt="Screenshot 2026-11-05 at 11 08 06" src="https://github.com/user-attachments/assets/47f739a7-52f6-44f1-b6ad-1792f9565312" />


### Current Quarter Sales

This page lets managers explore where their won revenue came from in the selected quarter. They can compare customer sectors, hover over countries to view sales, and see which products and accounts contributed most. The sales detail table lets them review individual wins, including who closed each deal, how long it took, and its sale value.

<img width="1004" height="559" alt="Screenshot 2026-11-05 at 11 06 42" src="https://github.com/user-attachments/assets/bc1f7da5-4b94-4a00-9725-a14b408f24fe" />


### Performance Over Time

Users select a manager and year to follow the team’s quarterly revenue against the company’s average team revenue, shown as a dotted line. The new opportunities chart groups deals by when they were first engaged and shows their recorded stage. Managers can also use the product heatmap to see where win rates rose or fell across quarters.

<img width="1004" height="559" alt="Screenshot 2026-11-05 at 11 10 34" src="https://github.com/user-attachments/assets/cb97a3e0-0724-461b-8d37-42f46f6ff69c" />


### Quarterly Performance by Team

Users select a year and quarter to compare managers across four measures: won revenue, win rate, average sale value, and days to close. Dotted benchmark lines help readers see where each team sits relative to the company and whether the teams that lead in revenue also lead in conversion or closing speed.

<img width="1004" height="559" alt="Screenshot 2026-11-05 at 11 06 06" src="https://github.com/user-attachments/assets/3ec1f437-27b7-485d-b113-42521f63ebee" />


---

## Key Metrics

| Metric | Definition |
| --- | --- |
| Total sales | Total close value of won opportunities |
| Won Deals | Number of opportunities marked as Won |
| Lost Deals | Number of opportunities marked as Lost |
| Win Rate | Won deals divided by won and lost deals |
| Average Won Deal Value | Won revenue divided by won deals |
| New Opportunities | Opportunities grouped by engagement date |
| Estimated Pipeline Value | Product list prices associated with open opportunities |

> Win rate considers closed outcomes only. Open opportunities are excluded from its denominator.

---

## Conclusion

This project turns CRM opportunity data into an interactive sales review tool.

Power Query supports data preparation, while DAX provides the calculations needed to compare results and explore performance. The dashboard brings these elements together to help managers review sales outcomes, investigate their drivers and prioritise open opportunities.
