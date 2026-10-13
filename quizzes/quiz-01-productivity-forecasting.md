# Quiz 1 prep: Productivity & Forecasting

**When:** Wednesday 14 Oct 2026, in class. A one-hour Q&A session comes first, then a **30-minute MCQ quiz**.
**Covers:** Productivity (lecture 2) and Forecasting.
**Counts for:** quizzes are 10 marks, and the better of the two quizzes counts.

> Productivity follows the faculty's slides ([lecture 2 notes](../notes/02-productivity-and-competitiveness.md)).
> **Forecasting slides aren't in the repo yet**, so that section follows Stevenson, *Operations Management* 12e, Ch. 3 (the course textbook). Check it against the class slides when you get them, and bring any slide-specific questions to the Q&A hour.

---

## Part A: Productivity cheat sheet

| Concept | Key fact |
|---|---|
| Productivity | **Output ÷ Input** |
| Productivity growth | (Current − Previous) ÷ Previous × 100% |
| Partial / single-factor | One input: Output ÷ Labour (the most common), Machine, Capital or Energy |
| Multifactor (MFP) | Output ÷ (several inputs). **All inputs in one unit, usually $** |
| Total | Output ÷ all inputs |
| Process yield | Good output ÷ raw material input (or rented ÷ available, and so on) |
| Efficient vs effective | Doing things right (minimum waste) vs doing the right thing (the right strategy) |
| 3 critical factors | **Labour, capital, management** |
| General factors | Methods, capital, quality, technology, management |
| Measurement problems | Quality changes, external factors, lack of precise units |
| Layoffs | Productivity rises **short term**, then falls (burnout, fear, the best people leave) |
| New workers / turnover | Lower productivity at first, so growing firms see a lag |
| Improvement steps | Measure → find the bottleneck → develop methods → set goals → get management support → measure and publicise |
| Cases | Toyota Kaizen: 4.2% growth a year. Samsung (productivity) vs TSMC (innovation): **TSMC won 54% share** |

**Calculation traps:** count **usable** units only, and convert everything to the **same time basis** before dividing.

---

## Part B: Forecasting cheat sheet (Stevenson Ch. 3)

### Basics
- **Forecast:** a statement about the future value of a variable, e.g. demand.
- **Features common to all forecasts:**
  1. They assume the causal system of the past will continue.
  2. They are rarely perfect.
  3. **Forecasts for groups of items are more accurate** than forecasts for individual items.
  4. **Accuracy decreases as the time horizon increases.**
- **A good forecast is** timely, accurate, reliable, in meaningful units, in writing, simple to understand and use, and cost-effective.
- **Steps:**
  1. Decide the purpose.
  2. Set the time horizon.
  3. Get, clean and analyse the data.
  4. Choose the technique.
  5. Make the forecast.
  6. Monitor the errors.

### Approaches
| Qualitative (judgement) | Quantitative |
|---|---|
| Executive opinions | **Time-series:** projects past data forward |
| Sales-force opinions | **Associative:** uses explanatory variables, e.g. regression |
| Consumer surveys | |
| **Delphi method:** anonymous experts, repeated questionnaire rounds until they reach consensus | |

### Time-series components
**Trend** (long-term movement), **seasonality** (regular short-term patterns: day, week, month, quarter), **cycles** (wave-like, longer than a year), **irregular variations** (one-off events such as strikes or storms) and **random variation** (residual noise).

### Techniques and formulas
| Method | Formula | Notes |
|---|---|---|
| **Naive** | F(t) = A(t−1) | Uses last period's actual. Simple, cheap, and a benchmark for other methods |
| **Moving average (MA)** | F(t) = (sum of last n actuals) ÷ n | **More periods = smoother but slower to respond** |
| **Weighted MA** | F(t) = Σ wᵢ·Aᵢ, weights sum to 1 | Usually the most recent period gets the biggest weight |
| **Exponential smoothing** | **F(t) = F(t−1) + α·(A(t−1) − F(t−1))** | α between 0 and 1. **Higher α = more responsive**, lower α = smoother |
| **Linear trend** | F(t) = a + b·t | b = (nΣty − ΣtΣy) ÷ (nΣt² − (Σt)²), a = (Σy − bΣt) ÷ n |
| **Seasonal relative** | Seasonal forecast = trend × seasonal relative | A relative above 1 means a season above average |
| **Associative / regression** | y = a + bx | Correlation r runs from −1 to +1. r² is the share of variation explained |

### Forecast accuracy
- **Error e = Actual − Forecast.** A positive error means the forecast was too low.

| Measure | Formula | Notes |
|---|---|---|
| **MAD** | Σ\|e\| ÷ n | Average absolute error, in the same units as the data |
| **MSE** | Σe² ÷ (n − 1) | Squares errors, so it **penalises large errors** |
| **MAPE** | Σ(\|e\| ÷ A × 100) ÷ n | Percentage, so it can be compared across different scales |
| **Tracking signal** | Σe ÷ MAD | Detects **bias**. It should stay within about ±4 MAD, otherwise review the method |

- **Bias:** errors consistently in one direction. Random errors cancel out.
- **Control chart for errors:** limits at 0 ± z·√MSE. Look for points outside the limits or non-random patterns.

### Quick worked examples
- **3-period MA** of 42, 40, 43 → (42 + 40 + 43) ÷ 3 = **41.67**
- **Weighted MA** with weights 0.5, 0.3, 0.2 (most recent first) on 43, 40, 42 → 21.5 + 12 + 8.4 = **41.9**
- **Exponential smoothing:** F = 42, A = 40, α = 0.1 → 42 + 0.1(40 − 42) = **41.8**. With α = 0.4 → **41.2**, which moves closer to the actual.
- **Accuracy:** A = 120, 130, 110 and F = 125, 125, 120 → errors −5, +5, −10
  - MAD = 20 ÷ 3 = **6.67**
  - MSE = 150 ÷ 2 = **75**
  - MAPE ≈ **5.70%**
  - Tracking signal = −10 ÷ 6.67 = **−1.5** (within limits)
- **Linear trend:** y = 10, 12, 15, 17, 21 for t = 1 to 5
  - Σt = 15, Σy = 75, Σty = 252, Σt² = 55
  - b = (5·252 − 15·75) ÷ (5·55 − 225) = 135 ÷ 50 = **2.7**
  - a = (75 − 2.7·15) ÷ 5 = **6.9**
  - F(6) = 6.9 + 2.7·6 = **23.1**

---

## Part C: Practice MCQs

### Productivity
1. Productivity is best defined as:
   (a) total output (b) output ÷ input (c) input ÷ output (d) output − input
2. Four workers each work 10 hours a day for 2 days and produce 800 units. Labour productivity is:
   (a) 20 (b) 40 (c) 10 (d) 100 units per labour-hour
3. Productivity rises from 800 to 820 units with the same hours. Growth is:
   (a) 2.0% (b) 2.5% (c) 20% (d) 0.25%
4. In a multifactor productivity calculation, the inputs must:
   (a) all be labour (b) be in the same unit, e.g. dollars (c) exclude overhead (d) include management time
5. A process takes in 1,250 units of raw material and turns out 1,000 good units. Process yield is:
   (a) 1.25 (b) 0.80 (c) 0.20 (d) 250
6. "Doing the right thing" describes:
   (a) efficiency (b) effectiveness (c) productivity (d) yield
7. Right after a layoff, productivity typically:
   (a) falls at once (b) rises in the short term, then may fall (c) stays the same (d) becomes unmeasurable
8. Which of these is **not** one of the three critical factors for productivity improvement?
   (a) labour (b) capital (c) marketing (d) management
9. Samsung had higher productivity, yet TSMC gained 54% market share. This shows that:
   (a) productivity is irrelevant (b) innovation is another route to competitiveness (c) TSMC had lower costs (d) Samsung had better quality
10. In a labour productivity calculation, 70 pieces were produced and 2 were defective. The output to use is:
    (a) 70 (b) 72 (c) 68 (d) 35

### Forecasting
11. Which statement about forecasts is **true**?
    (a) Accuracy increases with the time horizon (b) Group forecasts are more accurate than individual ones (c) Good forecasts are always perfect (d) Forecasts assume the future differs from the past
12. The Delphi method uses:
    (a) regression on past data (b) anonymous expert questionnaires repeated until consensus (c) customer point-of-sale data (d) the last period's actual
13. A naive forecast for next month uses:
    (a) the average of all past data (b) last month's actual (c) a trend line (d) expert opinion
14. Increasing the number of periods in a moving average makes the forecast:
    (a) more responsive (b) smoother and less responsive (c) more biased upward (d) seasonal
15. In exponential smoothing, a **higher α** makes the forecast:
    (a) smoother (b) more responsive to recent changes (c) ignore recent data (d) equal to the naive forecast at α = 0
16. F(t−1) = 50, A(t−1) = 60, α = 0.2. The next forecast is:
    (a) 52 (b) 58 (c) 60 (d) 50
17. Regular patterns that repeat within a year (by day, week or quarter) are:
    (a) trend (b) cycles (c) seasonality (d) random variation
18. A 3-period moving average of 30, 36 and 39 is:
    (a) 35 (b) 36 (c) 39 (d) 105
19. Which accuracy measure **penalises large errors** most heavily?
    (a) MAD (b) MSE (c) MAPE (d) tracking signal
20. A tracking signal far outside ±4 indicates:
    (a) a perfect forecast (b) bias in the forecast (c) seasonality (d) random variation only
21. Errors are −5, +5 and −10. MAD is:
    (a) −3.33 (b) 6.67 (c) 10 (d) 20
22. A forecast that uses advertising spend to predict sales is:
    (a) time-series (b) associative (c) naive (d) qualitative
23. Forecast error is defined as:
    (a) forecast − actual (b) actual − forecast (c) \|forecast\| (d) actual ÷ forecast
24. To compare accuracy across products with very different sales volumes, use:
    (a) MAD (b) MSE (c) MAPE (d) Σe

---

## Answers

| Q | Ans | Q | Ans | Q | Ans |
|---|---|---|---|---|---|
| 1 | b | 9 | b | 17 | c |
| 2 | c (800 ÷ 80) | 10 | c | 18 | a (105 ÷ 3) |
| 3 | b | 11 | b | 19 | b |
| 4 | b | 12 | b | 20 | b |
| 5 | b (1,000 ÷ 1,250) | 13 | b | 21 | b (20 ÷ 3) |
| 6 | b | 14 | b | 22 | b |
| 7 | b | 15 | b | 23 | b |
| 8 | c | 16 | a (50 + 0.2·10) | 24 | c |

Also go back over the 5 "In Review" MCQs at the end of lecture 2. The answers are b, c, d, c, c.

---

## Questions to ask in the Q&A hour
- Will the quiz include numericals, e.g. MA, exponential smoothing or MFP calculations, or only theory?
- Is MSE divided by n or by n − 1?
- Is a calculator allowed?
