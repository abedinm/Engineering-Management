# Forecasting & Accuracy

Notes from Dr. Khan's lecture deck: [`05 Forecasting & Accuracy.pdf`](../slides/05%20Forecasting%20&%20Accuracy.pdf) (49 slides). Every worked answer below was recomputed. Three small slips on the slides are flagged with ⚠.

## Why forecast

- The primary goal of OM is to **match supply to demand**. A demand forecast tells you how much capacity or supply you'll need.
- Anticipated demand comes from **customer orders** and/or **forecasts**.
- Forecasts are a basic input for budgeting, capacity, sales, production and inventory, personnel and purchasing.
- Forecasting is part of **yield management** (the % of capacity used): good forecasts help managers decide when to offer discounts.

**Who uses forecasts:** accounting (cost estimates, profit projections, cash), finance (equipment replacement, funding), HR (hiring, training, layoffs), marketing (pricing, promotion), MIS (information systems), operations (schedules, capacity, inventory, make-or-buy, outsourcing), product/service design.

## 7 elements of a good forecast

1. **Timely:** the horizon covers the time needed to make changes
2. **Accurate**, with the degree of accuracy stated
3. **Reliable:** works consistently
4. **Meaningful units:** $ for finance, units for production, machines and skills for schedulers
5. **In writing**
6. **Simple to understand and use**
7. **Cost-effective:** benefits outweigh costs

## Time horizon

- **Short-term** → ongoing operations. **Long-term** → strategic planning (new products, equipment, facilities).
- **Planning the system** = long-range (products, facilities, equipment, location).
- **Planning the use of the system** = short and intermediate range (inventory, workforce, purchasing, production, budgeting, scheduling).

## Buyer beware

1. Forecasts are not perfect, so allow for errors.
2. Forecasts for **groups** of items are more accurate, because errors cancel out.
3. Techniques assume the same causal system continues.
4. **Accuracy decreases as the time horizon increases.**

## Approaches

- **Qualitative** (subjective, soft information) vs **quantitative** (hard data).
- **Judgmental:** consumer surveys, sales staff, managers and executives, expert panels.
- **Time-series:** project past experience into the future.
- **Associative:** explanatory variables (paint demand ← price, advertising, drying time).

## Time-series patterns

| Pattern | Meaning |
|---|---|
| Trend | long-term upward or downward movement |
| Seasonality | short-term, regular variation (calendar, time of day) |
| Cycles | wavelike variations lasting **more than one year** |
| Irregular | unusual one-offs (weather, strikes) → identify and remove |
| Random | what's left after all the others |

## Methods

| Method | Formula | Key point |
|---|---|---|
| Naive | F<sub>t+1</sub> = A<sub>t</sub> | stable → last value; trend → last value + last change. Doesn't smooth |
| Moving average | F<sub>t</sub> = MA<sub>n</sub> = ΣA<sub>t−i</sub> ÷ n | more periods = smoother but more lag |
| Weighted MA | Σ(weight × actual) | weights sum to 1; heaviest on the most recent |
| Exponential smoothing | F<sub>t</sub> = F<sub>t−1</sub> + α(A<sub>t−1</sub> − F<sub>t−1</sub>) | α usually < 50%; α closer to 0 = more smoothing |
| Least squares | F<sub>t</sub> = a + bt | b = [nΣty − ΣtΣy] ÷ [nΣt² − (Σt)²], a = [Σy − bΣt] ÷ n |

The MA slide also says "more recent values are given more weight". That's the weighted MA; a simple MA weights every value equally.

## Accuracy

- MAD = Σ|A − F| ÷ n · MSE = Σ(A − F)² ÷ (n − 1) · MAPE = Σ(|A − F| ÷ A × 100) ÷ n
- Lower = more accurate. n = the periods that have both an actual and a forecast.

## Forecasting steps

Purpose → time horizon → obtain, clean and analyse data → select a method → make the forecast → monitor the errors.

## Worked examples (all checked)

| Example | Answer |
|---|---|
| Naive: 50, 53 | F₃ = 56 |
| Naive: 50, 53, 55, 58 (changes not consistent) | F₅ = 58 |
| MA₃ carts: 42, 40, 43, 40, 41 | F₆ = 41.33; with A₆ = 38, F₇ = 39.67 |
| WMA .4/.3/.2/.1, same data | F₆ = 41.0; with A₆ = 39, F₇ = 40.2 |
| ES: F = 42, A = 40, α = .1 | 41.8, then 41.92 after A = 43 |
| ES α = .15: 10, 14, 12, 19, 8 | F₃ 10.60, F₄ 10.81, F₅ 12.04 (slide: 12.03), F₆ 11.43 |
| ES table α = .1 vs .4, periods 1–11 | F₁₂ = 41.73 and 40.92 (⚠ slide shows 42.35 at t = 10; exact 42.36) |
| Complaints 60, 65, 55, 58, 64 | naive 64 · MA₃ 59 · WMA .5/.3/.2 60.4 · ES α = .4 → 60.83 |
| Practice #3 (e), n = 4 | MAD 4.62 · MSE 34.44 · **MAPE 7.68%** (⚠ slide divides e² by A and gets 43.48%) |
| Least squares, 9 periods | F<sub>t</sub> = 45.47 + 1.75t → F₁₀ 62.97, F₁₁ 64.72 |
| Practice #1 passengers | F<sub>t</sub> = 933.33 + 171.43t → F₇ 2,133.34, F₈ 2,304.77 |
| Practice #2 cell phones (= Worksheet 2 Q3) | F<sub>t</sub> = 699.40 + 7.51t → F₁₁ 782, F₁₂ 790 |
| Accounts serviced, 8 periods | MAD 2.75 · MSE 10.86 · MAPE 1.28% (answer was hidden under a grey box) |
| Technique 1 vs 2 | T1: 4.67 / 49.6 / 0.97% · T2: **5.67** / 52.8 / 1.17% → T1 better (⚠ slide writes T2 MAD 6.67) |
