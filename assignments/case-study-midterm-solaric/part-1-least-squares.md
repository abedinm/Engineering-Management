# Part 1: Forecast series 1 (Least Squares), 2020–2030

**Data:** Solaric's installed capacity (MWp), 2020–2025.

Years are converted to t = 1, 2, …, 6 (2020 = 1) to keep the calculation simple, the same way as in Worksheet 2.

| Year | t | Capacity, y (MWp) | t² | ty |
|---|---|---|---|---|
| 2020 | 1 | 18 | 1 | 18 |
| 2021 | 2 | 22 | 4 | 44 |
| 2022 | 3 | 25 | 9 | 75 |
| 2023 | 4 | 26 | 16 | 104 |
| 2024 | 5 | 29 | 25 | 145 |
| 2025 | 6 | 30 | 36 | 180 |
| **Sum** | **21** | **150** | **91** | **566** |

n = 6

**Slope**

b = [nΣty − (Σt)(Σy)] ÷ [nΣt² − (Σt)²]
  = [6(566) − (21)(150)] ÷ [6(91) − (21)²]
  = (3,396 − 3,150) ÷ (546 − 441)
  = 246 ÷ 105
  = **2.343**

**Intercept**

a = [Σy − b(Σt)] ÷ n
  = [150 − 2.343(21)] ÷ 6
  = (150 − 49.2) ÷ 6
  = **16.80**

**Trend equation**

**F(t) = 16.80 + 2.343t**

Installed capacity grows by about **2.34 MWp per year**.

## Forecast series 1

| Year | t | Actual (MWp) | Forecast series 1, F(t) (MWp) |
|---|---|---|---|
| 2020 | 1 | 18 | 19.14 |
| 2021 | 2 | 22 | 21.49 |
| 2022 | 3 | 25 | 23.83 |
| 2023 | 4 | 26 | 26.17 |
| 2024 | 5 | 29 | 28.51 |
| 2025 | 6 | 30 | 30.86 |
| 2026 | 7 | – | 33.20 |
| 2027 | 8 | – | **35.54** |
| 2028 | 9 | – | **37.89** |
| 2029 | 10 | – | **40.23** |
| 2030 | 11 | – | **42.57** |

The 2027–2030 values (F_27 to F_30 series 1) feed into Parts 2 and 3.

## Accuracy check (2020–2025)

| Year | A | F | \|e\| | e² | \|e\|/A × 100 |
|---|---|---|---|---|---|
| 2020 | 18 | 19.14 | 1.14 | 1.30 | 6.35 |
| 2021 | 22 | 21.49 | 0.51 | 0.26 | 2.34 |
| 2022 | 25 | 23.83 | 1.17 | 1.37 | 4.69 |
| 2023 | 26 | 26.17 | 0.17 | 0.03 | 0.66 |
| 2024 | 29 | 28.51 | 0.49 | 0.24 | 1.67 |
| 2025 | 30 | 30.86 | 0.86 | 0.73 | 2.86 |
| **Sum** | | | **4.34** | **3.94** | **18.56** |

- MAD = 4.34 ÷ 6 = **0.72 MWp**
- MSE = 3.94 ÷ (6 − 1) = **0.79**
- MAPE = 18.56 ÷ 6 = **3.09%**

A MAPE of about 3% means the straight-line trend fits Solaric's past growth closely, so series 1 is a reasonable "business as usual" forecast.

> Note: actual growth slowed after 2022 (+1, +3, +1 MWp a year). A linear trend smooths this out, so series 1 may slightly **overstate** the future if that slowdown continues.
