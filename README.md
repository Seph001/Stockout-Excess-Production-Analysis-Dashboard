# Stockout & Excess Production Analysis

A Power BI dashboard that shows where a company is **running short on products** and where it is **producing too much**.

**Period covered:** May 21, 2020 – Dec 31, 2022

---

## What This Project Does

It brings production, demand, inventory and supplier data into one dashboard so a manager can quickly see:

- Which products customers want but the company cannot supply
- Which products the factories are making far more of than needed
- How suppliers and plants are performing

## Dashboard Pages

| Page | What It Shows |
|---|---|
| Inventory Intelligence | Main KPIs, unmet demand and overproduction by product |
| Availability Monitor | Product table with stock levels, reorder levels and alerts |
| Factory Consumption | Demand vs production by month, and output by plant |
| Supply Chain Monitor | Supplier volumes, supply cost and supply gap |

## Key Numbers

| Metric | Value |
|---|---|
| Total Demand | 265,322 units |
| Total Production | 7,991,803 units |
| Total Supply | 228,488 units |
| Supply Gap | 98,503 units |
| Total Supply Cost | 3,435,082 |
| Overproduced Products | 5 |
| Suppliers | 10 |
| Stock Cover | 252 days |

## What I Found

**1. The company is producing far more than it sells.**
Production is about 30 times demand. Five products are the main cause:

| Product | Extra Units Produced |
|---|---|
| Energy Drink 50cl | 1.73M |
| Maize Flour 5kg | 1.68M |
| Yoghurt 500ml | 1.58M |
| Maize Flour 1kg | 1.52M |
| Bottled Water 50cl | 1.36M |

**2. Some products have demand but no supply.**
Six products have customer demand with nothing produced or supplied to cover it, totalling 98,503 units:

| Product | Unmet Demand |
|---|---|
| Bottled Water 75cl | 32,893 |
| Orange Juice 1L | 31,022 |
| Vegetable Oil 5L | 25,676 |
| Vegetable Oil 1L | 6,554 |
| Rice 5kg | 1,720 |
| Tomato Paste 70g | 638 |

**3. Production does not follow demand.**
Production peaks in July and April, but demand peaks in January and September.

**4. The problem is company-wide.**
All 10 plants produce a similar amount (about 674K to 913K units each), so no single plant is the cause.

## Recommendations

1. Cut production of the five overproduced products to match demand.
2. Fix the supply gap first for Bottled Water 75cl, Orange Juice 1L and Vegetable Oil 5L.
3. Plan production around the months when demand is highest.
4. Update the stockout alert so it also flags negative available stock.

## Data Model

Five source tables: **Demand**, **Inventory**, **Product Master**, **Production** and **Supply Chain**, plus calendar tables and a measure table for DAX.

## Tools Used

Power BI Desktop, DAX, Power Query

## Author

**Daniel Joseph Unwujoh**
Data Analyst & Business Intelligence Consultant
