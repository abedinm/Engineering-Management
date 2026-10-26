# Part 2: Forecast series 2 (Policy target), 2027–2030

Series 2 asks how much capacity Solaric would need by 2030 if Bangladesh meets its **2025 policy target of 20% of national power demand from green sources by 2030**, and Solaric keeps its current share of the solar market.

## Assumptions

The case study doesn't give national figures, so these come from published sources:

| # | Assumption | Value | Source / reasoning |
|---|---|---|---|
| A1 | Bangladesh peak power demand in 2030 | **29,000 MW** | Integrated Energy and Power Master Plan (IEPMP 2023), as cited by ADB (~29,000 MW by 2030). The IEPMP range is 27,138–29,156 MW |
| A2 | Green share of demand by 2030 (policy target) | **20%** | Given in the case (2025 update) |
| A3 | Solar's share of green capacity | **80%** | Solar is about 80% of Bangladesh's renewable capacity today. The rest is mainly Kaptai hydro and small wind. Assume this mix holds to 2030 |
| A4 | National installed solar capacity in 2025 | **1,397 MW** | SREDA: 1,019 MW on-grid + 377 MW off-grid |
| A5 | Solaric's installed capacity in 2025 | **30 MWp** | Given in the case |
| A6 | Solaric keeps a constant market share to 2030 | – | Simplest neutral assumption: Solaric grows at the same pace as the national solar market |

## Step 1: Solaric's market share (2025)

Market share = Solaric capacity ÷ national solar capacity
= 30 ÷ 1,397
= **2.147%**

## Step 2: National solar requirement in 2030

- Green capacity needed = 29,000 MW × 20% = **5,800 MW**
- Solar portion = 5,800 MW × 80% = **4,640 MW**

## Step 3: Solaric's 2030 forecast, F_30 series 2

F_30 series 2 = 4,640 MW × 2.147% = **99.64 MWp**

## Step 4: Percentage difference against series 1

F_30 series 1 = 42.57 MWp (from Part 1)

% difference = (F_30 series 2 − F_30 series 1) ÷ F_30 series 1 × 100
= (99.64 − 42.57) ÷ 42.57 × 100
= **134.06%**

To meet the policy target, Solaric's 2030 capacity must be about **2.34 times** its trend forecast.

## Step 5: Apply the % difference to 2027–2029

F_t series 2 = F_t series 1 × (1 + 1.3406)

| Year | F series 1 (MWp) | Working | **F series 2 (MWp)** |
|---|---|---|---|
| 2027 | 35.54 | 35.54 × 2.3406 | **83.19** |
| 2028 | 37.89 | 37.89 × 2.3406 | **88.67** |
| 2029 | 40.23 | 40.23 × 2.3406 | **94.16** |
| 2030 | 42.57 | from Step 3 | **99.64** |

## Sensitivity: what if demand is different?

The 2030 demand figure (A1) has the biggest effect on the result, and published forecasts disagree. Keeping A2–A6 the same:

| 2030 demand scenario | National solar 2030 | F_30 series 2 | % diff vs series 1 | F_27 series 2 |
|---|---|---|---|---|
| IEEFA (lower, efficiency gains): 25,834 MW | 4,133 MW | 88.76 MWp | 108.51% | 74.11 MWp |
| **IEPMP 2023 (base case): 29,000 MW** | **4,640 MW** | **99.64 MWp** | **134.06%** | **83.19 MWp** |
| PSMP 2016 (higher): 33,000 MW | 5,280 MW | 113.39 MWp | 166.34% | 94.67 MWp |

Even the lowest scenario needs Solaric to roughly **double** its trend capacity by 2030. The conclusion that business-as-usual growth is far short of what the policy requires holds whichever figure you use.

## Sources

- ADB, linked document for project 57232-001 (IEPMP demand forecast): https://www.adb.org/sites/default/files/linked-documents/57232-001-ssa.pdf
- The Financial Express, "Pledges for increased use of renewable energy and Bangladesh reality" (SREDA solar capacity): https://thefinancialexpress.com.bd/views/pledges-for-increased-use-of-renewable-energy-and-bangladesh-reality
- LightCastle Partners, "Solar energy in Bangladesh: promise vs practicality" (solar ≈ 80% of renewables): https://lightcastlepartners.com/insights/2025/09/solar-energy-in-bangladesh-promise-vs-practicality/
- The Daily Star / IEEFA (lower 2030 demand estimate): https://www.thedailystar.net/business/news/power-development-board-can-save-12-billion-year-fixing-core-problems-ieefa-3767911
- Wikipedia, Electricity sector in Bangladesh (PSMP 2016 figure): https://en.wikipedia.org/wiki/Electricity_sector_in_Bangladesh
