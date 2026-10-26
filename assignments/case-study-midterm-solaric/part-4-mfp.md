# Part 4: MFP, planned vs revised requirements, 2027–2030

**Multifactor productivity (MFP) = Output ÷ (sum of all inputs)**

All inputs must be in the **same unit** before they can be added (lecture 2), so each input for the 100 MW plant is first converted to US dollars.

- **Planned requirement** = forecast series 1 (least-squares trend)
- **Revised requirement** = forecast series 2 (policy target)

## Step 1: Convert the inputs to dollars

The total input is the cost of **building the plant and running it for its first year** (capital cost + one year of operating cost).

| Input (100 MW plant) | Quantity | Unit cost assumption | Cost (US$) | Share |
|---|---|---|---|---|
| Machinery & equipment | $96,000,000 | **+15% VAT** (2024 policy update) | 110,400,000 | 90.53% |
| Land | 400 acres | Tk 30 lakh per acre | 9,775,967 | 8.02% |
| Manpower | 600 persons | Tk 30,000 per person per month, 12 months | 1,759,674 | 1.44% |
| Water | 80 m³/day | Tk 46.2 per m³ (WASA commercial rate), 365 days | 10,990 | 0.01% |
| **Total input** | | | **121,946,632** | 100% |

**Assumptions** (the case study doesn't give these):

| Assumption | Value | Source / reasoning |
|---|---|---|
| Exchange rate | Tk 122.75 per US$ | Bangladesh Bank interbank rate, April 2026 |
| VAT | 15% on machinery | Case study, 2024 policy update. Assumes the $96M quote excludes VAT |
| Land price | Tk 30 lakh per acre (≈ $24,440) | Assumed price for non-agricultural or char land suitable for solar. National land policy bars converting fertile farmland. No official published rate was found |
| Average wage | Tk 30,000 per month | Assumed blended average for engineers, technicians, O&M staff and security |
| Water tariff | Tk 46.2 per 1,000 L | Dhaka WASA commercial rate after its 10% July increase |

Machinery is over 90% of the total input, so the result is not very sensitive to the land, wage or water assumptions.

**100 MW plant MFP** = 100 MW ÷ $121.95M = **0.820 MW per $ million**

## Step 2: MFP for planned and revised requirements

Total input is held at the 100 MW plant level ($121.95M), and output is each year's required capacity:

MFP = Required capacity (MW) ÷ Total input ($ million)

| Year | Planned capacity, S1 (MW) | Revised capacity, S2 (MW) | **MFP planned** (MW/$M) | **MFP revised** (MW/$M) | **Difference** (MW/$M) | % difference |
|---|---|---|---|---|---|---|
| 2027 | 35.54 | 83.19 | 0.2915 | 0.6822 | **0.3907** | 134.06% |
| 2028 | 37.89 | 88.67 | 0.3107 | 0.7272 | **0.4165** | 134.06% |
| 2029 | 40.23 | 94.16 | 0.3299 | 0.7721 | **0.4422** | 134.06% |
| 2030 | 42.57 | 99.64 | 0.3491 | 0.8171 | **0.4680** | 134.06% |

Example for 2027:
- MFP planned = 35.54 ÷ 121.95 = 0.2915
- MFP revised = 83.19 ÷ 121.95 = 0.6822
- Difference = 0.6822 − 0.2915 = 0.3907 MW per $M

## What the results mean

1. **To meet the policy target with the same resources, MFP must rise by 134%.** The revised requirement needs 2.34 times more output from the same inputs every year.
2. **That rise is not realistic through productivity alone.** By 2030 the revised MFP (0.817) is almost equal to the full productivity of a complete 100 MW plant (0.820). Solaric would need to get nearly 100 MW of output from one plant's worth of inputs, at full design capacity, with no losses. From lecture 4, actual output is always below design capacity, because utilisation is below 100%.
3. **So the gap has to be closed mainly by adding resources, not by working the existing ones harder.** Productivity gains can help at the margin, for example by cutting losses and raising efficiency. But most of the roughly 57 MW gap needs new machinery, land and staff. Part 5 calculates these.
4. **The 15% VAT lowers MFP.** Without VAT, the total input would be $107.55M and plant MFP would be 0.930 MW/$M. The VAT makes each MW about **13% more expensive** to build, which raises the investment needed to close the gap.

> **Note on method:** if inputs are assumed to grow in proportion to capacity (each MW always uses 1% of the 100 MW plant's inputs), MFP is the same for both requirements (0.820 MW/$M), and the difference shows up only in total inputs. The method above holds inputs fixed and shows how much more productive Solaric would have to be to hit the target without new resources. Part 5 then works out the extra resources.

## Sources

- UNB, "Interbank dollar rate remains stable at Tk 122.75": https://unb.com.bd/category/Business/interbank-dollar-rate-remains-stable-at-tk-12275/184736
- The Daily Star, "Dhaka Wasa hikes water prices by 10pc from July": https://tds-images.thedailystar.net/news/bangladesh/news/dhaka-wasa-hikes-water-prices-10pc-july-3621781
- Eco-Business, "In Bangladesh, solar power brings work, but land shortage slows growth" (land-use restrictions): https://www.eco-business.com/news/in-bangladesh-solar-power-brings-work-but-land-shortage-slows-growth/
