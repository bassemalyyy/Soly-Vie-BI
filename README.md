# Soly Vie | Real Estate Sales Dashboard

A Power BI dashboard for **Soly Vie**, a residential compound in New Borg El Arab, Egypt, developed by **Seif Developments**. It tracks sales, units and customers in one interactive report.

## Features
- **Landing page:** a project image background with headline KPIs and page navigation
- **Overview:** customers, paid customers, booked units, total revenue, revenue by unit type and a daily paid-customers trend
- **Units:** inventory pipeline, booking rate per unit type and unsold revenue potential
- **Customers:** collection rate, client type breakdown (customers vs. employees) and a VIP investors leaderboard
- **Interactive design:** KPI cards flip on hover to explain each metric, and rows and bars highlight on hover

## Data Model
| Table | Type | Description |
|---|---|---|
| `fact_sales` | Fact | Payments: amount, payment date, payment ID and status |
| `dim_customer` | Dimension | Customer name, client type, employee ID and interest status |
| `dim_units` | Dimension | Unit type per customer |
| `calendar` | Dimension | Date table (day, month, year) |

## Project Files
| File | Purpose |
|---|---|
| `Soly_Vie_DAX_Query.dax` | All base DAX measures (customers, revenue, units, pipeline, time intelligence) |
| `Page0_Landing.dax` | HTML measure for the landing page |
| `Page1_Overview.dax` | HTML measure for the Overview page |
| `Page2_Units.dax` | HTML measure for the Units page |
| `Page3_Customers.dax` | HTML measure for the Customers page |

## How to Use
1. Open the report in **Power BI Desktop**.
2. Install the **HTML Content** visual from AppSource.
3. In the DAX query view, run `Soly_Vie_DAX_Query.dax` first, then each page file, and click **Update model with changes**.
4. On each page, add one HTML measure to an HTML Content visual and size it to fill the page.
5. Put your logos in the logo placeholders at the top of each page file.

## Tools
Power BI · DAX · HTML/CSS · SVG
