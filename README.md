# Hospitality Domain Dashboard

An interactive Power BI analytics project for the hospitality domain, built to track revenue, occupancy, booking behavior, platform performance, and property-level business health across Atliq hotel properties.

[![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Dataset](https://img.shields.io/badge/Dataset-Hospitality%20Bookings-2E86AB?style=for-the-badge)](#dataset)
[![Live Dashboard](https://img.shields.io/badge/View-Live%20Dashboard-00A36C?style=for-the-badge)](https://app.powerbi.com/view?r=eyJrIjoiZGQ0ZTBmYzgtMDZiNy00YTdiLWI5NjAtYTlhMjVhZjA1ZDc5IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## Quick Links

| Action | Link |
| --- | --- |
| Open the Power BI report | [Hospitality Domain Dashboard.pbix](./Hospitality%20Domain%20Dashboard.pbix) |
| View the PDF export | [Hospitality Domain Dashboard.pdf](./Hospitality%20Domain%20Dashboard.pdf) |
| Explore the live dashboard | [Power BI Live Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZGQ0ZTBmYzgtMDZiNy00YTdiLWI5NjAtYTlhMjVhZjA1ZDc5IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9) |
| Review the DAX cleaning notes | [Data cleaning using DAX](./Data%20cleaning%20using%20DAX) |

## Table of Contents

- [Project Overview](#project-overview)
- [Dashboard Focus](#dashboard-focus)
- [Key Insights](#key-insights)
- [Dataset](#dataset)
- [Tools Used](#tools-used)
- [How to Use](#how-to-use)
- [Repository Structure](#repository-structure)

## Project Overview

This dashboard helps hotel stakeholders monitor performance across multiple properties and cities. It combines booking, capacity, hotel, room, and date data into a Power BI model that highlights revenue trends, occupancy patterns, average daily rate, cancellation behavior, realization percentage, and customer ratings.

The report is designed for quick business review: users can compare properties, cities, room categories, booking platforms, and weekly performance to identify where revenue is growing, where occupancy is weak, and where operational attention is needed.

## Dashboard Focus

<details open>
<summary><strong>Revenue and Pricing</strong></summary>

- Total revenue and realized revenue
- RevPAR, ADR, and realization percentage
- Revenue split by city, property, room class, and platform

</details>

<details>
<summary><strong>Occupancy and Capacity</strong></summary>

- Occupancy percentage by property and category
- Successful bookings against available capacity
- Weekly performance movement

</details>

<details>
<summary><strong>Booking Behavior</strong></summary>

- Checked out, cancelled, and no-show bookings
- Cancellation percentage
- Platform-wise booking contribution
- Guest counts and booking status analysis

</details>

<details>
<summary><strong>Customer Experience</strong></summary>

- Ratings given by guests
- Property-level performance comparison
- City and category-level quality signals

</details>

## Key Insights

| Metric | Value |
| --- | ---: |
| Total Revenue | 1,688M |
| Average RevPAR | 7,337 |
| Average Occupancy | 58% |
| Average ADR | 12,696 |
| Realization | 70% |
| Cancellation Rate | 24%-26% |

**Top performing properties**

| Property | City | Revenue | ADR | Occupancy |
| --- | --- | ---: | ---: | ---: |
| Atliq Exotica | Mumbai | 117M | 16,141 | 66% |
| Atliq Palace | Mumbai | 100M | 16,016 | 66% |

**Lowest performing properties**

| Property | City | Revenue | ADR | Occupancy |
| --- | --- | ---: | ---: | ---: |
| Atliq Exotica | Hyderabad | 47M | 9,111 | 45% |
| Atliq Bay | Mumbai | 51M | 15,167 | 45% |

## Dataset

<details open>
<summary><strong>CSV files included in this project</strong></summary>

| File | Purpose |
| --- | --- |
| [fact_bookings.csv](./fact_bookings.csv) | Individual booking records with booking status, guests, platform, revenue, and ratings |
| [fact_aggregated_bookings.csv](./fact_aggregated_bookings.csv) | Property, date, and room-category capacity with successful bookings |
| [dim_hotels.csv](./dim_hotels.csv) | Hotel property metadata including property name, category, and city |
| [dim_rooms.csv](./dim_rooms.csv) | Room category definitions |
| [dim_date.csv](./dim_date.csv) | Calendar and weekly date mapping |

</details>

<details>
<summary><strong>Important columns analyzed</strong></summary>

- `revenue_generated`
- `revenue_realized`
- `booking_status`
- `booking_platform`
- `ratings_given`
- `successful_bookings`
- `capacity`
- `property_name`
- `category`
- `city`
- `room_category`

</details>

## Tools Used

| Tool | Use |
| --- | --- |
| Power BI | Dashboard design, data modeling, and visualization |
| Power Query | Data cleaning and transformation |
| DAX | Measures, calculated fields, and KPI logic |
| Excel/CSV | Source data preparation |

## How to Use

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Clone this repository.
3. Open [Hospitality Domain Dashboard.pbix](./Hospitality%20Domain%20Dashboard.pbix).
4. Use filters and visuals to explore revenue, occupancy, ADR, RevPAR, cancellations, ratings, and platform performance.

## Repository Structure

```text
.
|-- Hospitality Domain Dashboard.pbix
|-- Hospitality Domain Dashboard.pdf
|-- Data cleaning using DAX
|-- dim_date.csv
|-- dim_hotels.csv
|-- dim_rooms.csv
|-- fact_aggregated_bookings.csv
|-- fact_bookings.csv
`-- README.md
```

## Author

Created by [rutika-oss](https://github.com/rutika-oss) as a Power BI hospitality analytics project.
