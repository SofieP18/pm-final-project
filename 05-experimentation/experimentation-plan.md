# A/B Experiment Brief, Riverty BU Collection, A Fair Way Forward

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | an Income explainer |
| Persona | a consumer with one or two open claims who works irregular shifts and has no fixed monthly income |
| Expected outcome | her reaching the income document step in the same session in which she reaches the income question, because she knows which income to enter and for which period |
| Primary success metric | the share of users who reach the affordability questions and then reach the income document step in the same session |
| Baseline rate | 80.7% (re-measure on the exact same-session definition before launch) |
| Guardrail metric | the 60-day missed-payment rate among shift-income agreements (baseline 22.5%) |
| Guardrail boundary | +2.8 points (one-sided 95% upper bound for B minus A; Risk review at a point estimate above +1.0 point) |
| Second guardrail | Documents needing review (baseline 28.0%) no more than +2.0 points above A. Companion: kept agreements per 100 randomised shift-income users no lower than A, and the shift-income agreement rate no more than 3.0 points below A. A guardrail failure overrides a primary win: do not ship |
| Minimum Detectable Effect | 3pt |
| Sample size per arm | 2,551 minimum for the primary. Enrol for 26 weeks, then wait 10 weeks (60-day window, agreement-creation lag and data lag) and read once at week 36. The guardrail needs about 5,500 pooled shift-income agreements, and 7,150 are expected. Between 4,500 and 5,500 the guardrail still applies, with about 73 to 80% power. If fewer than 4,500 exist at week 26, the guardrail is monitoring only and a ship needs written Risk sign-off in place of the guardrail condition. Change freeze on the income step and plan screen for the whole window. |
| Traffic split | 50/50 |
| Test duration | 36 weeks |
| Significance threshold | < 0.05 |

## Control vs. Variant
- **Control (A):** At the income step she sees no definition and no stated period, so she can't tell whether "income" means this month or a normal month. She leaves, or continues and later picks a plan by shortcut.
- **Variant (B):** At the income field, add an inline explainer that states which income to enter, for which period, and what to do when pay varies. The copy covers these three things only. It has no content on why income is asked or how long it is kept.
- **Held constant (isolation check):** Product and release: same build in both arms. The only difference is the explainer layer.
Eligibility and entry: same audience, channels and entry rules.
The journey itself: same screens, same income field rules (schema, validation, required status), same Continue button, same step order.
Support and operations: same agent scripts, staffing and contact routes.
Measurement: same event definitions and logging in both arms.
Held constant: B5 (mobile upload fix) is frozen for the whole window

## Hypothesis
> I believe that an Income explainer for a consumer with one or two open claims who works irregular shifts and has no fixed monthly income will result in her reaching the income document step in the same session in which she reaches the income question, because she knows which income to enter and for which period, as measured by a 3pt change in the share of users who reach the affordability questions and then reach the income document step in the same session within 36 weeks. We will protect the 60-day missed-payment rate among shift-income agreements (baseline 22.5%) throughout the test.

## Shipping criteria
> We will **ship** if the share of users who reach the affordability questions and then reach the income document step in the same session improves by ≥ 3pt at < 0.05 and the 60-day missed-payment rate among shift-income agreements (baseline 22.5%) does not reach +2.8 points (one-sided 95% upper bound for B minus A; Risk review at a point estimate above +1.0 point) after 36 weeks.
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 36 weeks, no results reviewed before this date.
