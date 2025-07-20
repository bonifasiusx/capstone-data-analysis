# BRT Passenger Flow Analysis

## Project Overview

This capstone project analyzes **TransJakarta** passenger flow data (April 2023) to identify **critical routes and time periods** based on **travel duration** and **passenger volume**. The goal is to support efficient **fleet allocation and scheduling decisions.**

Tools used:

* Python (pandas, seaborn, folium)
* Tableau (interactive dashboard)

---

## Objective

> Identify the **most congested time slots and longest-duration routes** to optimize fleet deployment and improve service quality.

---

## Repository Structure

```
├── cleaned_dataset/           # Cleaned dataset (.xlsx)
├── raw_dataset/               # Raw dataset
├── tableau_dashboard/         # .twbx file (Tableau)
├── capstone_m2_data_analysis.ipynb  # Main EDA notebook
└── README.md
```

---

## Key Analysis

* **Rush Hour Impact**

  Significant increase in travel time during **06:00–08:00** and **17:00–19:00** (Mann-Whitney test, p < 0.05)
* **Top 10 Longest Routes**

  Routes with the highest average travel duration
* **Top 10 Most Crowded Routes**

  Based on passenger transaction volume
* **Critical Route Identification**

  Combined top 10 from both metrics → **risky & high-load corridors**
* **Demographic Pattern**

  Age 19–45 dominates rush hour traffic

---

## Strategic Recommendations

1. **Adjust headway intervals** during rush hours on crowded routes
2. **Trial express (skip-stop) service** on long-duration routes
3. **Reduce frequency** on underutilized long routes, reallocate to fast high-volume ones

---

## Interactive Dashboard

> Built with Tableau
>
> Includes KPIs, critical route map, travel time trends, and age segmentation
>
> [Transjakarta Dashboard](https://public.tableau.com/app/profile/bonifasius.sinurat/viz/capstone_m2_dashboard/Dashboard1)

---


## Tech Stack

* Python 3.13
* Jupyter / VS Code
* Tableau Public

---

## Author

Built by `@bonifasiusx` – Capstone M2 | Data Science

*For academic and learning purposes only*
