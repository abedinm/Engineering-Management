# Worksheet 2: Forecasting

Faculty's solved worksheet: [`EM WS2 Forecasting (solved).pdf`](EM%20WS2%20Forecasting%20(solved).pdf)

I re-checked every answer with a script. All of them are correct apart from small rounding differences, noted below.

## How the faculty does it (use the same method in exams)

| Topic | Faculty's method |
|---|---|
| **Weighted MA, weights not ordered** | Sort the weights in **descending** order and give the biggest to the **most recent** period |
| **Starting exponential smoothing** | When no forecast is given, the period-2 forecast = period-1 actual (**naive**) |
| **MAD for smoothing** | Average only over periods that have a forecast. Here that's periods 2–6, so **÷ 5** |
| **Trend regression** | Convert years to t = 1, 2, 3, …, then use b = (nΣty − ΣtΣy) ÷ (nΣt² − (Σt)²) and a = (Σy − bΣt) ÷ n |
| **Accuracy of a trend line** | Plug t = 1…n back into the equation to get "forecasts" for the past years, then compute the errors |
| **MAD** | Σ\|e\| ÷ **n** |
| **MSE** | Σe² ÷ **(n − 1)** (confirmed: 36,761.91 ÷ 5 with n = 6) |
| **MAPE** | Σ(\|e\| ÷ A × 100) ÷ **n** |

## Q1: Ice-cream demand, periods 1–6 = 2000, 2200, 1800, 2100, 2300, 2200

**(a) 3-period MA for period 7:** (2100 + 2300 + 2200) ÷ 3 = **2200**

**(b) Weighted MA with weights 0.3, 0.5, 0.1, 0.1:** reorder them to 0.5, 0.3, 0.1, 0.1, starting from the most recent period.
0.5(2200) + 0.3(2300) + 0.1(2100) + 0.1(1800) = **2180**

**(c) Exponential smoothing, with F₂ = 2000 (naive):**

| Period | A | F (α = 0.3) | \|e\| | F (α = 0.6) | \|e\| |
|---|---|---|---|---|---|
| 2 | 2200 | 2000 | 200 | 2000 | 200 |
| 3 | 1800 | 2060 | 260 | 2120 | 320 |
| 4 | 2100 | 1982 | 118 | 1928 | 172 |
| 5 | 2300 | 2017.4 | 282.6 | 2031.2 | 268.8 |
| 6 | 2200 | 2102.18 | 97.82 | 2192.48 | 7.52 |
| 7 | — | **2131.53** | | **2196.99** | |
| **MAD** | | | **191.68** | | **193.66** |

The MAD is lower with **α = 0.3**, so it's the more accurate choice.

> **One caution:** the worksheet says a lower MAD means MSE and MAPE "will also be lower". That **happens** to be true here: MAPE is 9.18% vs 9.42%, and MSE is also lower for α = 0.3. It is **not true in general**. MSE punishes big errors, so a method can have a lower MAD and a higher MSE. Set 1, Q16 of the quiz MCQs shows two methods with the same MAD but very different MSEs. If an exam asks you to compare methods on MSE, calculate it rather than assuming.

## Q2: Trend regression, 2018–2023 demand = 1000, 1100, 1300, 1700, 2000, 2300

- With t = 1…6: Σt = 21, Σy = 9,400, Σt² = 91, Σty = 37,700
- b = (6 × 37,700 − 21 × 9,400) ÷ (6 × 91 − 21²) = 28,800 ÷ 105 = **274.29**
- a = (9,400 − 274.29 × 21) ÷ 6 = **606.67** (the worksheet's 606.65 comes from rounding b first)
- **F(t) = 606.67 + 274.29t**
  - 2024 (t = 7): **2,526.7**
  - 2025 (t = 8): **2,801.0** (the worksheet's 2,800.97 is rounding)

**Accuracy (periods 1–6):** MAD = 377.13 ÷ 6 = **62.86**. MSE = 36,761.91 ÷ 5 = **7,352.38**. MAPE = 30.28 ÷ 6 = **5.05%** (the worksheet shows 5.04%, which is rounding).

## Q3: Cell-phone sales, weeks 1–10 = 700, 724, 720, 728, 740, 742, 758, 750, 770, 775

- Σt = 55, Σt² = 385, Σy = 7,407, Σty = 41,358
- b = (10 × 41,358 − 55 × 7,407) ÷ (10 × 385 − 55²) = 6,195 ÷ 825 = **7.51**
- a = (7,407 − 7.51 × 55) ÷ 10 = **699.40**
- **F(t) = 699.40 + 7.51t**
  - Week 11: **782**
  - Week 12: **790** (789.5 rounded)

> The worksheet writes b as `10(41358) − 55(7407) / 10(385) − (55)²` without brackets. In an exam, put brackets around the top and the bottom so the marker sees the correct order of operations.
