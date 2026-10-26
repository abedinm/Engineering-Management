# Lecture 4: Strategic Capacity Planning

Slides: [`slides/04 Strategic Capacity Planning.pdf`](../slides/04%20Strategic%20Capacity%20Planning.pdf)

## What capacity is

- **Capacity** is the **upper limit or ceiling** on the load an operating unit (a plant, department, machine or employee) can handle.
  - The load can be **physical units** (bicycles assembled per hour) or **services** (computers upgraded per hour).
- Capacity is a major factor in a project's **initial cost**, because it limits the possible output rate.
- **Bigger capacity means higher capital cost but lower operating cost.** That's why projects often start with a small pilot or market-test unit even though its operating costs are higher.
- **Three key questions:** *What kind* of capacity? *How much*, to match demand? *When* is it needed?

## Why capacity decisions are strategic

They affect:
1. **Operating costs.** Matching capacity to demand keeps them down.
2. **Long-term commitment of resources.** Hard or expensive to change once built.
3. **Competitiveness.** Excess capacity, or the ability to add it quickly, is a **barrier to entry** for other firms and supports delivery speed.
4. **Ease of management.** Matched capacity is easier to manage than a mismatch.

**Globalisation** makes this harder: distant supply chains and markets add uncertainty, and long project lifecycles need **scenario planning**. A power plant, for example, can take years to build, by which time demand may have changed.

## Measuring capacity

| Measure | Meaning |
|---|---|
| **Design capacity** | The maximum output rate under **ideal** conditions |
| **Effective capacity** | Design capacity **minus** planned allowances: breaks, personal time, product-mix changes, maintenance, scheduling and balancing problems, scrap |
| **Actual output** | Effective capacity **minus** unplanned losses: breakdowns, absenteeism, material shortages, quality problems and other factors outside the manager's control |

Design ≥ Effective ≥ Actual.

$$\textbf{Efficiency} = \frac{\text{Actual output}}{\text{Effective capacity}} \times 100\% \qquad \textbf{Utilisation} = \frac{\text{Actual output}}{\text{Design capacity}} \times 100\%$$

> Don't confuse this with lecture 2. "Efficiency" here is a **capacity ratio** (actual ÷ effective). In lectures 2 and 3, *efficient* meant "doing things right with minimum waste".

**Example: truck repair.** Design = 50/day, effective = 40/day, actual = 36/day.
- Efficiency = 36 ÷ 40 = **90%**
- Utilisation = 36 ÷ 50 = **72%**
- 90% looks good, but 72% against the design capacity is the more meaningful number.
- Effective capacity acts as a lid on output. To raise utilisation, raise **effective capacity**: fix quality problems, maintain equipment, train staff, improve bottlenecks and eliminate waste (lean).

## Eight determinants of effective capacity

| Factor | Key idea | Slide example |
|---|---|---|
| **Facilities** | Size, room to expand, location, layout, heating, lighting, ventilation | **Boeing 737 MAX (2020):** the Renton line was idled because there was no storage space for undelivered jets |
| **Product/service** | Uniform output means more standardisation and more capacity. A limited menu is faster than a big one | **Tesla Model 3 (2018):** complex wiring and battery designs slowed assembly and added rework |
| **Process** | Quality problems cause inspection and rework. Batch changeover time also counts | **Toyota Aichi (2016):** retooling for hybrid engines cut capacity for a while |
| **Human** | Job design, training, skill, experience, motivation, absenteeism, turnover | **Foxconn (2020, COVID):** labour shortages and absenteeism |
| **Policy** | Whether management allows overtime or 2nd and 3rd shifts | **India textile quotas (2006):** export quotas left mills under-used |
| **Operational** | Scheduling, inventory, late deliveries, purchasing, inspection. One missing component halts assembly | **Ford JIT (2011):** a software error caused line stoppages |
| **Supply chain** | Can suppliers, warehousing, transport and distributors handle the change? | **Toyota microchip shortage (2021):** single-source dependency |
| **External** | Product standards, pollution rules, regulatory paperwork, disasters | **Bangladesh garment floods (2017):** Gazipur and Savar factories lost weeks of output |

**Memory aid:** **F**acilities, **P**roduct, **P**rocess, **H**uman, **P**olicy, **O**perational, **S**upply chain, **E**xternal.

## Determining needed capacity

You need: demand forecasts per product, standard processing time per unit, work days per year, and number of shifts.

$$\text{Units of capacity needed} = \frac{\text{Processing time needed}}{\text{Processing time capacity per unit}}$$

**Example:** one 8-hour shift, 250 days a year, so each machine gives 8 × 250 = **2,000 h/year**.

| Product | Annual demand | Hours per unit | Hours needed |
|---|---|---|---|
| 1 | 400 | 5.0 | 2,000 |
| 2 | 300 | 8.0 | 2,400 |
| 3 | 700 | 2.0 | 1,400 |
| **Total** | | | **5,800** |

5,800 ÷ 2,000 = 2.90, so you need **3 machines**. Always **round up**, because you can't buy 0.9 of a machine.

## Capacity strategy

**Strategy rests on assumptions about:**
1. The growth rate and variability of demand.
2. The cost of building and running facilities of different sizes.
3. The rate and direction of technological change.
4. Competitors' likely behaviour.
5. The availability of capital and other inputs.

**The eight steps of capacity planning:**
1. Estimate future requirements.
2. Evaluate existing capacity and find the gaps.
3. Identify alternatives.
4. Do a financial analysis of each.
5. Assess the qualitative issues.
6. Select the best long-term alternative.
7. Implement it.
8. Monitor the results.

**Three strategies:**

| Strategy | When capacity is added | Best for |
|---|---|---|
| **Leading** | **Before** demand rises, in anticipation | Long lead times for adding capacity |
| **Following** | **After** demand exceeds current capacity | Avoiding idle capacity, at the risk of lost sales |
| **Tracking** | Like following, but in **small increments** that keep pace with demand | Close matching |

**Make-or-buy decision matrix** (strategic value vs cost):

| | Low cost | High cost |
|---|---|---|
| **High strategic value** | Weigh cost/benefit | **Make** |
| **Low strategic value** | **Buy** | Defer / judgement call |

## Evaluating alternatives: cost-volume analysis

Techniques include **cost-volume analysis**, financial analysis, decision theory and waiting-line analysis.

- **Fixed costs (FC)** stay the same whatever the volume: rent, property tax, equipment, heating and cooling, some admin.
- **Variable costs** change with volume, mainly materials and labour. Assume the cost per unit **v** stays constant and all output is sold.

| Quantity | Formula |
|---|---|
| Total cost | **TC = FC + v·Q** |
| Total revenue | **TR = R·Q** (R = revenue per unit) |
| Profit | **P = TR − TC = Q(R − v) − FC** |
| Contribution margin | **R − v** |
| Volume needed for a target profit | **Q = (P + FC) ÷ (R − v)** |
| **Break-even point** | **Q_BEP = FC ÷ (R − v)** |

- Below the BEP you make a **loss**. Above it you make a **profit**, and the further from the BEP, the bigger the profit or loss.
- **Indifference point:** the volume where two alternatives give equal profit or cost. Below it one option is better, above it the other.

### Worked example 1: Old-Fashioned Berry Pies
FC = $6,000/month, v = $2, R = $7.

| Part | Working | Answer |
|---|---|---|
| a. Break-even | 6,000 ÷ (7 − 2) | **1,200 pies/month** |
| b. Profit at 1,000 pies | 1,000(5) − 6,000 | **−$1,000 (a loss)** |
| c. Pies for a $4,000 profit | (4,000 + 6,000) ÷ 5 | **2,000 pies** |
| d. Price for a $5,000 profit at 2,000 pies | 5,000 = 2,000(R − 2) − 6,000, so R − 2 = 5.5 | **R = $7.50** |

### Worked example 2: Battery chargers
FC = $42,000/month, v = $3, R = $7, so contribution = $4 per unit and profit = 4Q − 42,000.

| Volume | TR | Total VC | FC | TC | Profit |
|---|---|---|---|---|---|
| 10,000 | 70,000 | 30,000 | 42,000 | 72,000 | **(2,000)** |
| 12,000 | 84,000 | 36,000 | 42,000 | 78,000 | 6,000 |
| 15,000 | 105,000 | 45,000 | 42,000 | 87,000 | 18,000 |

- BEP = 42,000 ÷ 4 = **10,500 units/month**
- At 22,000 units: 4(22,000) − 42,000 = **$46,000**

## Make (in-house) or buy (outsource)?

- **In-house:** TC₁ = FC + v·Q
- **Outsource:** TC₂ = R·Q, where R is the supplier's price per unit and there's no fixed cost.
- **Indifference volume:** Q₀ = FC ÷ (R − v). This is the same shape as the BEP formula.
- **Rule:** Q > Q₀ → **make**. Q < Q₀ → **buy**.
- If the supplier's price is **below** your variable cost, just **buy**. Fixed costs don't even matter then.

### Worked example: vending-machine part
Make: FC = $150,000/year, v = $60. Buy: $80 per unit. Volume = 12,000/year.

- **(a)** Make = 150,000 + 12,000(60) = **$870,000**. Buy = 12,000(80) = **$960,000**. So **make**.
- **(b)** Indifference: 150,000 + 60Q = 80Q, so Q = 150,000 ÷ 20 = **7,500 units/year**. Below that, buy. Above it, make.

## Likely exam points

- **Numericals:**
  - efficiency vs utilisation;
  - number of machines needed (round up);
  - BEP, profit at a given Q, Q for a target profit, price for a target profit;
  - a cost-volume table;
  - make-or-buy cost comparison and indifference volume.
- Design vs effective vs actual output: what gets subtracted at each step.
- The eight determinants of effective capacity, each with its case example.
- Leading vs following vs tracking strategies.
- The make-or-buy matrix quadrants.
- Why capacity decisions are strategic (the four reasons).
