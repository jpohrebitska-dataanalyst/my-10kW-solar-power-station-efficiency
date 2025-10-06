# 🌞 Solar PV Performance Dashboard — Kyiv 10 kW Vertical System  

**Status:** Operational since **March 2025**  
**Location:** Kyiv, Ukraine  
**Type:** Residential / Prosumer PV System  
**Capacity:** 10 kW (vertical panels)  
**Grid:** Connected (bi-directional — sell & buy)  

---

## 🔍 Overview  

This project presents a real-world performance analysis of a **10 kW vertical solar power station** located in **Kyiv, Ukraine**.  
The goal is to evaluate **production efficiency**, **consumption balance**, and **energy exchange with the national grid** based on daily operational data.

The dashboard was built in **Tableau**, with supplementary calculations and visualizations performed in **Python** (PVLib, Pandas, Matplotlib).

---

## 📸 Dashboard Preview  

![SPS Dashboard](results/SPS_Dashboard.png)

> Tableau dashboard illustrating production, consumption, and grid balance metrics for the Kyiv 10 kW vertical solar system.

---

## 🎯 Objectives  

- Assess daily and monthly **generation efficiency** of vertically mounted PV panels.  
- Visualize **energy balance** — self-consumption, grid purchase, and grid export.  
- Track **seasonal variation** in solar production and household consumption.  
- Provide a **data-driven view** of system profitability and sustainability.

---

## 🧠 Tools & Technologies  

| Category | Tools / Libraries |
|-----------|------------------|
| Data Processing | Python, Pandas, PVLib |
| Visualization | Tableau Public |
| Data Sources | Smart Meter exports (Solarman Smart), Excel logs |
| Supporting Tools | Excel, Google Sheets |

---

## 📊 Dashboard Structure  

**1. Production vs Consumption Overview**  
Displays daily solar generation and electricity usage, highlighting **self-consumed** and **exported** energy.  

**2. Grid Interaction (Waterfall / Stacked Bar)**  
Shows the **energy sold to** and **purchased from** the grid over time, providing an instant balance view.  

**3. Monthly Performance Summary**  
Aggregated view of total production, self-consumption ratio, and grid dependence.  

**4. Efficiency Trend (Python → Tableau)**  
A Python-generated efficiency index visualized in Tableau, reflecting actual vs. theoretical output.

---

## 📂 Repository Structure  

```text
data/           → Raw & cleaned Excel datasets (production, consumption)  
tableau/        → Packaged Tableau workbook (.twbx)  
python/         → Scripts for efficiency and PV performance analysis  
results/        → Screenshots and exports of Tableau dashboards  
README.md       → Project overview and insights  

---

## 🔍 Methodology  

1. **Data Collection** — Smart meter & inverter data (daily kWh values).  
2. **Data Cleaning** — Removal of missing/duplicate entries, normalization by date.  
3. **Performance Metrics:**  
   - Production / Consumption ratio = Production / Consumption 
   - Grid Export = Production – Consumption (if positive), monthly  
   - Grid Import = Consumption – Production (if positive), monthly  
   - Efficiency = Actual Production / Expected (PVLib model)  
4. **Visualization** — Tableau dashboards for intuitive exploration.  

---

## 📈 Insights  

- Vertical installation provides **better winter output** and **reduced summer overproduction**, improving overall balance.  
- The system shows **avg 1.6 Production/Consumption ratio** overtime and **limited grid dependency** during spring – autumn periods.  
- Real data aligns closely with PVLib model predictions (± X %), confirming the accuracy of vertical-panel modeling.

---

## 🚀 Next Steps  

- Add **real-time data integration** via Solarman API.  
- Extend the dataset for full-year (2025–2026) comparison.  
- Compare **vertical vs. optimal-tilt panels** efficiency under Kyiv conditions.  
- Automate daily metrics upload and Tableau refresh.

---

## 📎 Credits  

**Author:** Julia Pohrebitska  
**Role:** Data Analyst / PV System Owner / Dashboard Developer  

**Tools:** Tableau · Python · PVLib · Excel  
**Location:** Kyiv Region, Ukraine  

