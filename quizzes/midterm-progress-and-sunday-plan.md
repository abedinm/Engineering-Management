# Midterm progress log and Sunday plan

Midterm: Sun 8 Nov, 15:00-17:00. About 80% problem solving, 20% modified true/false and short answer.

Video used: Coder Bhai, [Engineering Management MID Term (AIUB)](https://www.youtube.com/watch?v=_QZq7eA3yFQ)

| Part | Video time |
|---|---|
| Productivity | 1:00-23:00 |
| Naive, moving average, weighted MA, exponential smoothing | 23:00-35:10 |
| Least squares trend | 35:10-48:00 |
| MAD, MSE, MAPE | 48:00-1:01:30 |
| Capacity: efficiency, utilisation, machines | 1:01:30-1:18:20 |
| Cost-volume, break-even, make or buy | 1:18:20-1:34:48 |

## Studied (Sat 7 Nov, 16:01-21:10)

| Topic | Done | Full working |
|---|---|---|
| Productivity | Video 1:00-23:00, solved along with it | [notes/02](../notes/02-productivity-and-competitiveness.md) |
| | Smart-watch MFP (slide 18), worked example | [notes/02, Practice 1](../notes/02-productivity-and-competitiveness.md) |
| | WS1 Q1 (a)-(c), worked example | [WS1 README](../assignments/worksheet-01-productivity/README.md) |
| | WS1 Q2, worked answer: $57 per labour-hour | [WS1 README](../assignments/worksheet-01-productivity/README.md) |
| Forecasting | Video 23:00-35:10 (naive, MA, WMA, exponential smoothing), solved along | [notes/06](../notes/06-forecasting-and-accuracy.md) |
| | Ice-cream exponential smoothing table, alpha 0.3 (WS2 Q1 c) | [WS2 README](../assignments/worksheet-02-forecasting/README.md) |
| Least squares trend | Video 35:10-48:00 watched | [notes/06](../notes/06-forecasting-and-accuracy.md) |

Nothing solved alone yet.

## Left

| Topic | Practice | Answer |
|---|---|---|
| Productivity, solo | WS1 Q4 (a)-(d) | [WS1 README](../assignments/worksheet-01-productivity/README.md) |
| Forecasting, solo | Practice #3 (a)-(d), slides 46-49 | [notes/06](../notes/06-forecasting-and-accuracy.md) |
| Least squares, solo | Practice #1 (passengers) | [notes/06](../notes/06-forecasting-and-accuracy.md) |
| MAD, MSE, MAPE | Practice #3 (e) | [notes/06](../notes/06-forecasting-and-accuracy.md) |
| Capacity: efficiency, utilisation | Slide 5 | [notes/04](../notes/04-strategic-capacity-planning.md) |
| Capacity: machines needed | WS3 Q1 | [WS3 README](../assignments/worksheet-03-capacity-planning/README.md) |
| Break-even, profit, target price | Pies (slide 17), chargers (slide 19), WS3 Q2-Q4 | [notes/04](../notes/04-strategic-capacity-planning.md), [WS3 README](../assignments/worksheet-03-capacity-planning/README.md) |
| Make or buy | Slide 25 | [notes/04](../notes/04-strategic-capacity-planning.md) |
| Formula sheet | Write it from memory | Checklist below |

## Sunday plan (between the AI exam and the EM exam)

| Time | Block |
|---|---|
| 11:15-11:40 | WS1 Q4 (a)-(c) alone |
| 11:45-12:10 | Capacity slide 5 and pies slide 17 as worked steps, then redo pies with the answer covered |
| 12:15-12:40 | Practice #3 (a)-(d) alone |
| 12:40-13:05 | Lunch |
| 13:05-13:20 | Rest, eyes closed, alarm set |
| 13:20-13:45 | Practice #1 alone, then MAD/MSE/MAPE worked on Practice #3 data |
| 13:50-14:10 | WS3 Q1 machines, make or buy, chargers: shortest steps |
| 14:10-14:30 | Formula sheet from memory |
| 14:30 | Walk to the exam room |

## Answers to check against

**WS1 Q4** (AC units; 9 h/day, 5 days)
- a) A 300 / 450 = 0.67 pcs/LH; B 200 / 675 = 0.30
- b) A 15,000,000 / 63,000 = 238.10; B 14,000,000 / 99,000 = 141.41
- c) 29,000,000 / 162,000 = 179.01 (not the average of A and B)
- d) A 2 pcs/kWh > B 1, so A

**Capacity slide 5:** efficiency 36 / 40 = 90%; utilisation 36 / 50 = 72%

**Pies, slide 17** (FC 6,000, v 2, R 7)
- a) BEP 6,000 / 5 = 1,200
- b) 1,000 x 5 - 6,000 = -1,000
- c) (4,000 + 6,000) / 5 = 2,000
- d) 5,000 = 2,000(R - 2) - 6,000, so R = 7.50

**Practice #3** (60, 65, 55, 58, 64)
- a) naive 64
- b) 3-period MA (55 + 58 + 64) / 3 = 59
- c) WMA 0.5(64) + 0.3(58) + 0.2(55) = 60.4
- d) ES alpha 0.4, F2 = 60: F3 62, F4 59.2, F5 58.72, F6 60.83
- e) |E| 5, 7, 1.2, 5.28: MAD 18.48 / 4 = 4.62; MSE 103.32 / 3 = 34.44; MAPE 30.74 / 4 = 7.68%. Slide 49 shows 43.48%: wrong, it divided E² by A.

**Practice #1** (1000, 1200, 1500, 2000, 1700, 1800)
- Σt 21, Σy 9,200, Σt² 91, Σty 35,200, n 6
- b = (6 x 35,200 - 21 x 9,200) / (6 x 91 - 21²) = 18,000 / 105 = 171.43
- a = (9,200 - 171.43 x 21) / 6 = 933.33
- F7 = 933.33 + 171.43 x 7 = 2,133.33

**WS3 Q1:** 12,380 h / 3,500 = 3.54, round up to 4 machines

**Make or buy, slide 25:** make 150,000 + 60 x 12,000 = 870,000; buy 80 x 12,000 = 960,000, so make. Indifference 150,000 / (80 - 60) = 7,500 units.

**Chargers, slide 19** (FC 42,000, v 3, R 7): BEP 42,000 / 4 = 10,500; profit at 22,000 = 88,000 - 42,000 = 46,000

| Q | TR | TC | P |
|---|---|---|---|
| 10,000 | 70,000 | 72,000 | -2,000 |
| 12,000 | 84,000 | 78,000 | 6,000 |
| 15,000 | 105,000 | 87,000 | 18,000 |

## Formula sheet checklist

- Productivity = output / input; MFP = output / sum of all inputs in $; growth = (new - old) / old x 100
- Naive F(t) = A(t-1); MA = average of last n; WMA = Σ(weight x A), heaviest weight on the latest period
- ES: F(t) = F(t-1) + alpha(A(t-1) - F(t-1))
- Least squares: b = (nΣty - ΣtΣy) / (nΣt² - (Σt)²); a = (Σy - bΣt) / n; F(t) = a + bt
- MAD = Σ|E| / n; MSE = ΣE² / (n - 1); MAPE = Σ(|E| / A x 100) / n
- Efficiency = actual / effective; utilisation = actual / design
- Machines = Σ(demand x time per unit) / hours per machine, round up
- TC = FC + vQ; TR = RQ; P = Q(R - v) - FC
- BEP = FC / (R - v); Q for a profit = (P + FC) / (R - v); price for a profit R = (P + FC) / Q + v
- Make or buy indifference Q = FC / (v_buy - v_make); two options Q = (FC_A - FC_B) / (v_B - v_A)
