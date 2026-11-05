# Class Notes: Midterm Revision (4 Nov 2026)

Made from the recording of the online class (Microsoft Teams, Dr. Arif Mostafa Khan). He went through his **"EM Mid Notes 2627: Engineering Management Midterm Revision Notes, Fall 26/27"** PDF and answered questions about the exam. He said the notes are on the **Portal**.

> **What the recording missed (now filled in from the full PDF).** The recording started at 15:02, after the class had begun, so it missed the start of the notes. The full revision notes are now filed at [`EM Mid Notes 2627.pdf`](EM%20Mid%20Notes%202627.pdf). The parts the recording missed:
>
> - **Competitiveness:** the ability to win and retain customers relative to alternatives. Operations contribute through cost, quality, delivery speed, delivery reliability and flexibility. The priorities depend on what the customer values.
> - **Management skills:** *technical* (a frontline supervisor diagnoses calibration drift and explains the corrective procedure), *human* (coaching staff, resolving conflict across functions), *conceptual* (a middle manager coordinating purchasing, production and quality; senior management deciding whether to fund a spare-parts network). All levels use all three skills; the emphasis shifts.
> - The multifactor and total rows of the productivity table (filled in below).

## A. What he said about the midterm

- **Marks split (his rough estimate):** about **80% problem solving**, about **20% modified true/false and short answers**.
- **Topics:** productivity, forecasting and capacity planning. He said the midterm syllabus is short and "fairly simple".
- **Break-even:** there is **one** formula, but he can ask you to find **any** part of it:
  - profit;
  - quantity;
  - price;
  - even the **variable cost per unit (v)**.
  - In his words: "You must be able to manipulate the equation in order to find your answer."
- **Make or buy:**
  - Find the **indifference point Q₀**. You can set **total costs equal** (fixed + variable) or **profits equal**.
  - If the required volume is below Q₀, one option is better (cheaper or more profitable). Above Q₀, the other one is.
  - Sketch the graph if it helps.
- **Machines needed:** **always round up**. His example: 5.2 machines means **6** in your answer.
- **Utilisation vs efficiency:**
  - **Efficiency** reflects **management's competence**.
  - **Utilisation** also reflects the **wider environment**. His example: during political unrest, output can drop even if management does well.
- **Practice:** he told the class to **work through the worksheets** for more realistic problems. The revision notes are there to clarify the concepts.
- **Group project presentations:** to be delivered on the **first day back** after the break. He's expecting good presentations because the class has had a lot of time. Email or message him if you want feedback.

## B. Productivity

- **Production** is the quantity produced in a period. **Productivity** is output ÷ input over the same period.
- **More output doesn't always mean better productivity.** If good output goes from 800 to 920 units (+15%) but labour goes from 100 to 125 hours, labour productivity **falls** from 8.00 to 7.36 units per hour. Higher output can come from using more resources rather than from a better process.

| Measure | What goes in the denominator | Example unit |
|---|---|---|
| **Partial** | One input (labour or energy) | Units per labour-hour; $ output per $ of energy |
| **Multifactor** | A selected combination of inputs | Dollars of output per dollar of labour and materials |
| **Total** | All inputs within the stated measurement scope | Dollars of output per dollar of total input cost |

- **Use a common value basis (e.g. $) to combine inputs.** Adding labour hours to kilograms means nothing.
- **A company-wide labour measure is still partial**, because only labour is in the denominator.

### Effectiveness vs efficiency
- **Effectiveness:** did the operation **achieve its goal**?
- **Efficiency:** how well did it **use its resources**?
- Example: a repair team restores service by noon (effective) but uses more technician hours than planned (less efficient).
- **Services:** define good output carefully. A help desk can close more tickets per hour by rushing complex cases, so track **successfully resolved** tickets alongside repeat incidents. In a factory, count only **conforming** units so scrap doesn't inflate output.

### His worked example: shop with two products
500 controllers at $48 and 800 mounts at $20 in a month. Six employees work 20 days at $90 per person-day. Uses 700 kg of material at $6/kg and 2,400 kWh at $0.25/kWh.

- Output value = 500 × 48 + 800 × 20 = **$40,000**
- Inputs:
  - Labour = 6 × 20 × 90 = $10,800
  - Material = 700 × 6 = $4,200
  - Energy = 2,400 × 0.25 = $600
  - **Total = $15,600**
- Labour productivity = 40,000 ÷ 10,800 = **3.70**
- Energy productivity = 40,000 ÷ 600 = **66.67**
- Total productivity = 40,000 ÷ 15,600 = **2.56**
- Each result is dollars of output per dollar of that input.
- **If mount output rises 20%,** with prices and inputs unchanged:
  - Revenue rises by 160 × $20 = $3,200.
  - Total productivity = 43,200 ÷ 15,600 = **2.77**, only about **+8%**, not +20%, because mounts are only part of the output mix.
- To compare periods when prices change, use **constant prices** so you see the change in physical performance.

## C. Forecasting

**Demand patterns:**
- **Level:** fluctuates around a roughly stable average.
- **Trend:** a persistent rise or fall.
- **Seasonality:** repeats at a known interval, e.g. a demand surge each semester.
- **Isolated surge:** a one-off special event.

Watch out:
- A method built for a stable level will **lag a trend**.
- A trend line can **mistake a temporary surge for real growth**.

**A useful forecast is** timely enough to act on, reasonably accurate, reliable under similar conditions, in meaningful units, and easy to update. **Start by identifying the decision and the time horizon.** Tomorrow's staffing and next year's machine purchases may need different methods.

| Method | How to use it | What to watch |
|---|---|---|
| **Naive** | F(t+1) = A(t) | Uses only the latest actual; useful as a benchmark |
| **Simple moving average** | Average the most recent n actuals | Smooths random ups and downs but lags a sustained trend |
| **Weighted moving average** | Multiply recent actuals by their weights and add | Weights must add up to 1; match each weight to the right period |
| **Exponential smoothing** | F(t+1) = F(t) + α(A(t) − F(t)) | The bracket is the signed error; α is how much of it you correct. Older data still counts through F(t), less and less over time (0 < α < 1). **Smaller α = slower to adjust** |
| **Linear trend regression** | Fit y = a + bt to demand vs time | Projects a trend; assumes the pattern continues |

**Forecast accuracy:**
- **MAD (mean absolute deviation):** the typical size of the error, in the original units.
- **MSE (mean squared error):** squares the errors, so **large misses count more**.
- **MAPE (mean absolute percentage error):** error relative to actual demand.
  - Errors in **low-demand periods weigh more**.
  - An actual of **zero** makes that period's percentage error **undefined**.
- **Mean signed error:** measures **bias**. In his example all the errors were positive, meaning every forecast was **below** the actual. (Error = actual − forecast.)

## D. Capacity planning

**Capacity and performance:**
- **Design capacity:** the maximum rate under ideal conditions.
- **Effective capacity:** design capacity after normal constraints like planned maintenance, setups and product mix.
- **Actual output:** what the operation actually delivers.
- **Bottleneck (new, not in the lecture slides):** the resource whose capacity limits the whole system's output. Improving a *different* resource only creates idle time or inventory, because the bottleneck still decides throughput.

**The two ratios:**
- **Utilisation = actual ÷ design. Efficiency = actual ÷ effective.**
- Design − effective = **planning allowances**.
- Effective − actual = **performance against the achievable plan**.

**His example:** a line designed for 800 units per shift, planned for 640, delivers 576.
- **Utilisation = 576 ÷ 800 = 72%**
- **Efficiency = 576 ÷ 640 = 90%**

### Break-even and target profit
- **Profit = (P − v)Q − F**
  - P = price, v = variable cost per unit, Q = volume, F = fixed cost.
  - Each unit contributes **P − v** toward fixed cost, then profit. P − v must be positive.
  - The model assumes price and variable cost per unit stay constant within the relevant range.
- **Rearrange it for whatever he asks** (from Part A):

| Find | Formula |
|---|---|
| Break-even Q | F ÷ (P − v) |
| Q for target profit | (Profit + F) ÷ (P − v) |
| Price for target profit | v + (Profit + F) ÷ Q |
| Variable cost per unit | P − (Profit + F) ÷ Q |
| Profit at volume Q | (P − v)Q − F |

**His example: pump shop.** Annual lease Tk 480,000, monthly fixed staffing Tk 25,000. Price Tk 950, unit cost Tk 520.
- Monthly fixed cost = 480,000 ÷ 12 + 25,000 = **Tk 65,000**.
- Contribution per pump = 950 − 520 = **Tk 430**.
- Monthly break-even = 65,000 ÷ 430 = 151.16 → **sell at least 152** (round **up** to avoid a loss).
- Check: 151 pumps give Tk 64,930 of contribution, short of the fixed cost. 152 give Tk 65,360.
- **Target profit Tk 220,000 a year at 2,000 pumps:**
  - Annual fixed cost = 65,000 × 12 = Tk 780,000.
  - Required price = 520 + (780,000 + 220,000) ÷ 2,000 = **Tk 1,020 per pump**.
  - Check by solving for v instead: 1,020 − 1,000,000 ÷ 2,000 = 520 ✓
- **Break-even vs crossover:** break-even compares revenue with total cost. A crossover compares the costs of **two ways to supply the same quantity**.

### Make or buy
- Compare the **relevant** total cost of each option for the same parts and volume. Include the fixed costs that **change with the decision** and the variable cost of the volume needed.
- **A sunk cost (already spent) is irrelevant.**

**His example: connector.** Make for Tk 18 per unit plus Tk 156,000 of avoidable fixed cost a year, or buy for Tk 31 per unit.
- **Crossover:** 156,000 + 18Q = 31Q → **Q₀ = 12,000 connectors a year**.
- **Demand:** 1,150 a month = **13,800 a year**, which is above Q₀.
  - **Make** = 156,000 + 18 × 13,800 = **Tk 404,400**
  - **Buy** = 31 × 13,800 = **Tk 427,800**
  - Making saves **Tk 23,400 a year**.
- Below the crossover, buying is cheaper.
- **Also consider:** supplier quality, lead time, and whether your own machines are free.

### Machines needed for a product mix
If machines are interchangeable, convert each product's demand into **standard processing time** and add them up. Products that need **different dedicated machines** get a separate workload per machine group.

**His example:** 12,000 parts at 6 min, 6,000 at 14 min, 2,000 at 24 min. Two machines, 8 h a day, 230 workdays, 5 days of planned maintenance. Each available machine-hour delivers 0.75 standard hours.
- Workload = 12,000 × 6 + 6,000 × 14 + 2,000 × 24 = 204,000 min = **3,400 h**
- Clock time per machine = (230 − 5) × 8 = **1,800 h**
- Work capacity per machine = 1,800 × 0.75 = **1,350 standard hours**
- Machines needed = 3,400 ÷ 1,350 = 2.52 → **round up to 3**, so **add 1 machine**
- Check: two machines give 2,700 h, a shortfall of 700 h. The third adds 1,350 h and covers it.

**New detail to remember:** take out the **maintenance days first**, then apply the **efficiency factor** (0.75). Both reduce capacity.

---
*All 39 numbers in his examples were recomputed and are correct.*
