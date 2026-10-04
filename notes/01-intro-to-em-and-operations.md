# Lecture 1 — Introduction to Engineering Management & Operations

Slides: [`slides/01 Intro to EM+Ops.pdf`](../slides/01%20Intro%20to%20EM+Ops.pdf)

## Course info

- **Faculty:** Arif Khan — arif.khan@aiub.edu
- **Consultation:** 13:00–14:30, Mon/Wed
- **Textbook:** William J. Stevenson, *Operations Management*, 12th ed.

### Marks breakdown

| Component | Marks |
|---|---|
| Class attendance | 13 |
| Class engagement | 2 |
| 2× in-class worksheets | 5 |
| 2× quizzes (best one counts) | 10 |
| In-class case study | 10 |
| Group project | 10 |
| Midterm / final exam | 50 |
| **Total (per term)** | **100** |

Bonus points come from Kahoot. Midterm term = 40% and final term = 60% of the overall grade.

## What the course covers

Three areas:
1. **Fundamental knowledge:** technical expertise + business principles + decision-making. EMs bridge engineering and management, so projects meet both the technical spec and the organisation's goals.
2. **Psychomotor skills:** applying that knowledge with tools: Gantt charts, operations trade-offs (inventory, queues, line speed), budget and cost modelling, technical presentations.
3. **Affective skills:** empathy, accountability and integrity, inclusivity, resilience, continuous improvement.

## Business vs engineering management

- **Engineering management** applies engineering principles to business practice: technical projects, product development, process optimisation. It is the *value creator*.
- **Business management** coordinates production, finance, marketing and HR toward organisational goals. It is the *value pricer*.
- Both co-lead product development, cost optimisation and digital transformation. Together they are the *value sustainer*.

| Aspect | Business mgmt | Engineering mgmt |
|---|---|---|
| Strategy | Market/profit-driven | Technology/feasibility-driven |
| Focus | Value proposition, brand, ROI | Functionality, safety, technical excellence |
| Tools | Balanced Scorecard, SWOT, 5 Forces | FMEA, root cause analysis, Six Sigma, CAD |
| Metrics | Market share, ROI, customer satisfaction | Cost/time/scope control, delivery KPIs, reliability |
| Typical role | Strategy / marketing manager | Operations / technology manager |

**Example: Tesla Gigafactory.** Business managers handled strategy, Panasonic supply contracts, investment and demand forecasts, and reported to the CEO. Engineering managers built and commissioned the production lines, used Six Sigma and lean, and cut battery cost per kWh by about 30%. They reported to the CTO.

Video from class: <https://youtu.be/TayGW3nRxUk>

## Competitiveness

> How effectively an organisation meets customer wants and needs **relative to others** offering similar goods or services.

Companies compete through strategy, product/service, marketing, **operations**, distribution and R&D.

The slide's competitive factors and examples: **innovation** (Apple), **dependability** (Walton), **cost** (H&M), **quality** (Intel) and **delivery speed** (Dell).

### Ten ways businesses compete using operations
1. **Product & service design:** innovation and time-to-market.
2. **Cost:** productivity drives cost advantage; outsourcing is one lever.
3. **Location:** near inputs means cheaper inputs; near markets means cheaper, faster delivery.
4. **Quality:** materials, workmanship, design and service. Customers pay more for perceived quality.
5. **Quick response:** fast launches, fast delivery, fast complaint handling.
6. **Flexibility:** adapting to changes in design, volume or mix.
7. **Inventory management:** matching supply to demand.
8. **Supply chain management:** coordinating buyers and suppliers for timely, cost-effective delivery.
9. **Service:** after-sale value. Service quality is a sustainable differentiator.
10. **Managers & workers:** competent, motivated people are an edge in themselves.

## Types of operations

- **Project-based:** unique, time-bound outputs (construction).
- **Manufacturing:** tangible goods (textiles, cars).
- **Service:** intangible value (consulting, education, software support). Its challenges:
  - *Intangibility:* quality is hard to measure.
  - *Variability:* customer experiences are inconsistent.
  - *Perishability:* idle capacity is lost revenue.
- **Hybrid:** goods plus services (restaurants, healthcare).

**Case: Starbucks mobile ordering.** Peak-hour bottlenecks caused 20% of orders to be delayed. The causes were variability (unpredictable arrivals) and perishability (drinks remade if not collected). Predictive staffing plus dedicated pickup stations made service 30% faster.

## Why organisations fail

1. Neglecting **operations strategy**.
2. Missing strengths and opportunities, or ignoring competitive threats.
3. Favouring short-term financials over R&D.
4. Over-focusing on product design, under-focusing on process design.
5. Under-investing in technical resources.
6. Poor internal communication across functions.
7. Ignoring customer wants and needs.

## Root cause analysis: fishbone (Ishikawa) diagrams

The **problem or effect** goes at the fish's head. **Cause categories** are the main bones, and sub-causes branch off them.

**Steps:**
1. Agree on a clear, specific problem statement.
2. Agree on the cause categories (8P or 6M/7M).
3. Brainstorm causes by asking *"Why does this happen?"* and place each one on a bone. A cause can sit in several categories.
4. Keep asking *"Why?"* to get sub-causes, which leads to root causes.
5. Look for connections between causes across branches.

| 8P (business / service) | 6M / 7M (manufacturing / project) |
|---|---|
| Procedures | Materials |
| Policies | Machinery |
| Place | Methods |
| Product | Measurement |
| People | Manpower |
| Processes | Mother Nature (environment) |
| Price | Money *(the 7th M)* |
| Promotion | |

- The **8P** diagram breaks down the interdependencies of a business: activities, products and processes.
- The **6M** diagram organises information about a project, often one still in planning.
- In 6M diagrams, causes are often tagged **C** (controllable) or **N** (non-controllable).
- ASQ example: "iron in product", traced through measurement (lab error), materials (supplier), methods (sampling), environment (rusty pipes), manpower (inexperienced analyst) and machines (heat-exchanger leaks).

> Note: the 8P diagram on the slide labels two bones "Physical Evidence" in place of Policies/Price/Procedures. That comes from the services marketing mix. Use the 8P list above for exams unless told otherwise.

## PDCA cycle (Plan, Do, Check, Act)

| Step | What happens |
|---|---|
| **Plan** | Define the problem, gather data, form a hypothesis, set the goal and metrics |
| **Do** | Try the fix **small**, as a controlled experiment rather than full deployment |
| **Check** | Compare results with predictions. Did it work? Why or why not? |
| **Act** | If it worked, standardise and roll out. If not, adjust and go back to Plan |

**Example: meetings overrunning.** Plan: introduce a strict agenda and a timekeeper. Do: try it in one weekly meeting. Check: survey the team and look at productivity after a month. Act: roll it out to all meetings, or try a different approach.

**Class exercise: software team missing sprint deadlines.**
- **Plan:** three months of sprint data show only 60% of work completed on time. Goal: 85% within two months. Metrics: story-point completion, mid-sprint scope changes, capacity utilisation.
- **Do:** pilot on one squad with better estimation, daily scope-change tracking and capacity planning. Document everything.
- **Check:** completion rose to 75%, short of the goal. Unplanned interruptions were eating into capacity.
- **Act:** standardise the estimation process, add a buffer for unplanned work, roll out to other squads, and start a new cycle focused on interruptions.

## Business problem solving: putting it together

- **RCA:** use a fishbone to trace the problem (e.g. machine → method → manpower).
- **PDCA:** Plan (identify) → Do (test the fix) → Check (measure) → Act (implement).

**Case: Boeing 737 MAX.** Two crashes were caused by faulty MCAS software. RCA found *Manpower* problems (inadequate pilot training) and *Methods* problems (gaps in software safety validation). The PDCA action was a redesigned MCAS, mandatory simulator training and recertification.

## Likely exam points

- Define competitiveness, then list the 10 ways operations help firms compete.
- Compare business and engineering management (table, plus the Tesla example).
- Name the four types of operations and the three service challenges.
- List the 8Ps and 6Ms, the fishbone steps, and draw a fishbone for a given problem.
- Apply PDCA to a scenario (sprint deadlines, meetings).
- Explain the Starbucks and Boeing cases.
