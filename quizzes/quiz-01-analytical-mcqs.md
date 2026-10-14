# Quiz 1: Analytical MCQs (Productivity & Forecasting)

20 calculation and reasoning questions. Every wrong option is a **common mistake**, so if you pick one, the solutions tell you which trap you fell into.
Aim for about **1.5 minutes per question**. Solutions start on the next page.

## Part A: Productivity

**1.** A bakery runs one shift: 6 workers × 7.5 hours produce 1,080 loaves. Quality control rejects 5%. What is the labour productivity?
(a) 24.0 loaves/LH  (b) 22.8 loaves/LH  (c) 171 loaves/worker  (d) 21.6 loaves/LH

**2.** A plant makes 2,400 units a day, sold at $5 each. Each day it uses 3 workers × 8 h at $15/h, $640 of materials, and overhead equal to 50% of labour cost. What is the multifactor productivity in **units per dollar**?
(a) 2.40  (b) 6.67  (c) 2.03  (d) 10.17

**3.** A workshop produces **500 units per day** and runs 5 days a week. Its **weekly** costs are labour $2,000, materials $1,500 and overhead $500. What is the MFP?
(a) 0.125 units/$  (b) 0.625 units/$  (c) 1.25 units/$  (d) 0.25 units/$

**4.** Before automation, a line produced 400 units in 80 labour-hours. After automation it produces 440 units in 72 labour-hours. By how much did labour productivity change?
(a) +10.0%  (b) +11.1%  (c) +22.2%  (d) +1.1 units/LH, which is +10%

**5.** A firm produces 1,000 units with $2,000 of inputs per period. Spending an extra $300 per period would raise output by 10%. What happens to MFP?
(a) It rises 10%  (b) It rises about 4.3%  (c) It falls about 4.3%  (d) It stays the same

**6.** A team of 4 workers on an 8-hour shift currently produces 720 units. Management wants **25 units per labour-hour**. How many **more** units per shift are needed?
(a) 25  (b) 80  (c) 100  (d) 180

**7.** A process turns 2,000 kg of raw material into 1,640 kg of good product. If yield improves to 90% on the same input, by how much does good output increase?
(a) 8.0%  (b) 9.8%  (c) 10.0%  (d) 18.0%

**8.** A company lays off 20% of its workforce, and total output falls by 10%. Hours per worker are unchanged. What happens to labour productivity in the short term?
(a) It falls 10%  (b) It rises 10%  (c) It rises 12.5%  (d) It rises 2.5%

## Part B: Forecasting

**9.** Demand for months 1–4 was 120, 132, 126 and 138. What is the 3-month moving-average forecast for month 5?
(a) 129  (b) 132  (c) 138  (d) 130

**10.** Using the same data, find the month-5 forecast with weights **0.5, 0.3, 0.2**, where 0.5 goes to the most recent month.
(a) 131.4  (b) 132.0  (c) 133.2  (d) 138.0

**11.** The month-1 forecast was 100. Actual demand was 110 in month 1 and 106 in month 2. With α = 0.3, what is the forecast for **month 3**?
(a) 103.0  (b) 103.9  (c) 104.8  (d) 106.0

**12.** Demand has **permanently** jumped from about 200 to about 240. The last forecast was 200 and the last actual was 240. Which α gives the better next forecast, and what is that forecast?
(a) α = 0.2 → 208  (b) α = 0.8 → 232  (c) α = 0.2 → 232  (d) Either. α doesn't matter after a permanent shift

**13.** Sales for periods 1–4 were 20, 24, 27 and 33. Fit a linear trend F(t) = a + bt and forecast **period 5**.
(a) 36.5  (b) 37.2  (c) 33.0  (d) 39.0

**14.** A forecaster predicted 52 in each of four periods. Actual demand was 50, 56, 48 and 60. What is the MAD?
(a) 1.5  (b) 4.5  (c) 6.0  (d) 18.0

**15.** Forecast errors (A − F) over five periods were +8, +6, +10, +4 and +7. Which statement is correct?
(a) TS = 1.0, so there is no bias
(b) TS = 5.0, so the forecast is consistently **too high**
(c) TS = 5.0, so the forecast is consistently **too low**, and the model should be reviewed
(d) MAD = 35, so accuracy is poor

**16.** Two methods were tested over five periods:
- Method A errors: +2, −2, +2, −2, +12
- Method B errors: +4, −4, +4, −4, +4

If one large miss is very costly, such as a stock-out, which method should you choose?
(a) A, because it has a lower MAD
(b) B. Both have the same MAD (4), but B has a much lower MSE
(c) A, because its errors are mostly smaller
(d) Either, because they have the same MAD

**17.** Actual demand was 200 and 250. The forecasts were 180 and 260. What is the MAPE?
(a) 7.0%  (b) 7.5%  (c) 14.0%  (d) 15.0%

**18.** Q3 has a seasonal relative of 0.9. Actual Q3 sales were 450 units. What are the **deseasonalised** sales?
(a) 405  (b) 450  (c) 500  (d) 540

**19.** Exponential smoothing with **α = 1** gives the same result as:
(a) a 3-period moving average  (b) the naive forecast  (c) a linear trend  (d) a forecast that never changes

**20.** Demand rises steadily every period, and a 4-period moving average is used. What will you see?
(a) The forecast leads demand, errors are negative and TS is negative
(b) The forecast lags demand, errors are positive and TS is positive
(c) The errors are random and TS is near 0
(d) The forecast matches demand exactly

<div style="page-break-before: always"></div>

## Solutions

| Q | Ans | Working | Trap options |
|---|---|---|---|
| 1 | **b** | Good loaves = 1,080 × 0.95 = 1,026. Labour-hours = 6 × 7.5 = 45. 1,026 ÷ 45 = **22.8** | (a) counted the rejects. (c) per worker, not per labour-hour |
| 2 | **c** | Labour = 3 × 8 × 15 = $360. Overhead = 0.5 × 360 = $180. Inputs = 360 + 640 + 180 = $1,180. 2,400 ÷ 1,180 = **2.03** | (a) left out overhead. (b) labour only. (d) revenue per $, not units |
| 3 | **b** | Weekly output = 500 × 5 = 2,500. 2,500 ÷ 4,000 = **0.625** | (a) mixed daily output with weekly costs |
| 4 | **c** | 400 ÷ 80 = 5.00, 440 ÷ 72 = 6.11. (6.11 − 5) ÷ 5 = **+22.2%** | (a) output change only. (b) hours change only |
| 5 | **c** | Before: 1,000 ÷ 2,000 = 0.500. After: 1,100 ÷ 2,300 = 0.478. Change **−4.3%** | Output goes up but inputs go up more (+15%), so MFP falls |
| 6 | **b** | Target = 25 × (4 × 8) = 800. 800 − 720 = **80** | (a) confused the target rate with the number of units |
| 7 | **b** | New good output = 2,000 × 0.90 = 1,800. 1,800 ÷ 1,640 − 1 = **+9.8%** | (a) 90% − 82% is percentage points, not a % increase |
| 8 | **c** | Productivity ratio = 0.90 ÷ 0.80 = 1.125, so **+12.5%** | The short-term rise after a layoff (burnout risk comes later) |
| 9 | **b** | (132 + 126 + 138) ÷ 3 = **132** | (a) averaged all four months |
| 10 | **c** | 0.5(138) + 0.3(126) + 0.2(132) = 69 + 37.8 + 26.4 = **133.2** | (a) weights reversed: 0.5 put on the oldest month |
| 11 | **b** | F₂ = 100 + 0.3(110 − 100) = 103. F₃ = 103 + 0.3(106 − 103) = **103.9** | (a) stopped after one step |
| 12 | **b** | 200 + 0.8(40) = **232**. A high α reacts quickly to a real shift | (a) a low α keeps forecasting near the old level for many periods |
| 13 | **a** | Σt = 10, Σy = 104, Σty = 281, Σt² = 30. b = (4·281 − 10·104) ÷ (4·30 − 100) = 84 ÷ 20 = 4.2. a = (104 − 42) ÷ 4 = 15.5. F₅ = 15.5 + 4.2·5 = **36.5** | (c) naive forecast. (d) extended the last jump (+6) |
| 14 | **b** | Errors: −2, +4, −4, +8. Σ\|e\| = 18, divided by 4 = **4.5** | (a) used signed errors: 6 ÷ 4. (d) forgot to divide by n |
| 15 | **c** | Σe = 35, MAD = 35 ÷ 5 = 7, TS = 35 ÷ 7 = **5**, which is outside ±4. Every error is positive, so the forecast is always below actual | (b) got the sign backwards. Error = A − F, so positive means the forecast was too low |
| 16 | **b** | Both MADs = 20 ÷ 5 = 4. MSE: A = 160 ÷ 4 = 40, B = 80 ÷ 4 = 20. B halves the MSE whether you divide by n or n − 1 | MSE squares errors, so it punishes the one big miss of 12 |
| 17 | **a** | 20 ÷ 200 = 10% and 10 ÷ 250 = 4%. (10 + 4) ÷ 2 = **7%** | (b) divided by the forecast instead of the actual. (c) added the % errors without averaging. (d) raw error total 30 ÷ 2 |
| 18 | **c** | Deseasonalised = actual ÷ relative = 450 ÷ 0.9 = **500** | (a) multiplied instead of dividing |
| 19 | **b** | F = F + 1·(A − F) = A, which is last period's actual | (d) is what α = 0 gives |
| 20 | **b** | An MA averages older, lower values, so it trails a rising trend. A > F gives positive errors and a positive TS | A reason to use a trend model or a higher α |

**Score guide:** 17–20 means you're ready. 13–16 means re-check the trap column for the ones you missed. Below 13, go back over the formulas in the full prep sheet.

**Common traps to remember**
- Leaving rejects in the output.
- Mixing daily and weekly figures.
- Leaving overhead out of MFP.
- Error = **A − F**, so a positive error means the forecast was too low.
- Percentage points are not a percentage change.
- Weights go on the **most recent** period.
- Deseasonalise by **dividing** by the seasonal relative.
