# Quiz 1 in plain English: Productivity & Forecasting

The two topics in plain language, using a tea stall as the running example.

## Productivity: how much you get out for what you put in

**Productivity = what you made ÷ what it took.**
You sell 120 cups of tea in 4 hours. That's 120 ÷ 4 = **30 cups an hour**.

- **Single-factor** looks at one input, usually people's time: cups per hour of work.
- **Multifactor** looks at everything you spent, in money: tea, milk, gas, wages. $60 spent to make 120 cups = 120 ÷ 60 = **2 cups per dollar**. You can only add the inputs together because they're all in dollars.
- **Growth %** compares new with old: (new − old) ÷ old. Going from 30 to 33 cups an hour is 3 ÷ 30 = **10% better**.

**Three traps:**
1. **Spilled cups don't count.** If 10 of the 120 spilled, you made 110.
2. **Same time period for everything.** Don't divide daily cups by weekly costs.
3. **Add all the costs.** Leaving out overhead makes the answer too big.

## Forecasting: guessing tomorrow's sales from the past

- **Naive:** "Tomorrow = today." You sold 100 today, so you guess 100.
- **Moving average:** the average of the last few days. Sales of 90, 100 and 110 average to **100**. Averaging **more days** gives a calmer guess but reacts **slower** to change.
- **Weighted average:** recent days count more. Yesterday might get 50% of the weight, the day before 30%, and so on.
- **Exponential smoothing:** move your old guess part of the way toward what actually happened.
    - **New guess = old guess + α × (actual − old guess)**
    - You guessed 100 and sold 120, so you were 20 short. With α = 0.5 you move halfway: **110**.
    - **α is how much you trust the latest day.** Big α jumps quickly. Small α stays calm.
- **Trend:** sales keep going up by about the same amount, so draw a straight line and extend it.
- **Seasonality:** you sell more tea every winter. A seasonal relative of 1.2 means winter is 20% above normal, so multiply by 1.2.

## Checking how good your guesses were

**Error = what really happened − what you guessed.** You sold 120 and guessed 100, so the error is **+20**. Positive means you guessed **too low**.

- **MAD:** how far off you are on average, ignoring + and −.
- **MSE:** squares the errors, so one **huge miss** is punished heavily.
- **MAPE:** the error as a **percentage**. Use it to compare a small product with a big one.
- **Tracking signal:** checks whether you're **always wrong in the same direction**. Always guessing too low is called **bias**.

## Remember these five

1. Productivity = out ÷ in, counting **good units only**.
2. **Error = actual − guess.**
3. **Big α** means fast reactions. **More days** in an average means smoother but slower.
4. **MSE** hates big misses, and **MAPE** is a percentage.
5. **Tracking signal** is for **bias**.
