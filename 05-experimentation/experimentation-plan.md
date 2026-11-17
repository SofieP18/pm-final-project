# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Based on that agreements with missed payment during 60 days is 19%, we believe that solving the income and plan commitments questions at the moment of decision for a consumer with one or two open claims who works irregular shifts and has no fixed monthly income will result in finishing the income step in one sitting, that she chooses a plan by its terms and consequences instead of by screen order or length. She also keeps the first payments, because she knew what she was committing to and she calls an agent only when she wants advice. It maps to Retention when an a agreement is kept, Churn by minimizing abandoned journeys and broken plans, and Revenue when instalments actually is collected., as measured by when the reached income document step gets over 83.7%. We will protect when the shift-income rate falls toward the fixed-salary rate (22.5% vs 17.4% for fixed salary), a 5.1-point fall ideally with the 60-day rate following later as confirmation and make a go/no-go decision after run a roughly 3-month 50/50 test on shift-income starters, and scale only if their missed-payment rate falls at least 4 points with durable agreements per 100 starters within 1 point of control; otherwise extend once, pivot, or roll back.
- **From M3, your primary success metric & guardrail metric:** When the reached income document step gets over 80.7% & When the shift-income rate falls toward the fixed-salary rate (22.5% vs 17.4% for fixed salary), a 5.1-point fall ideally with the 60-day rate following later as confirmation.
- **From M4, the feature you scoped in your PRD this is what you're testing:** B2 Income explainer.

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** B2 Income explainer.
- **Persona pull your M2 persona:** A consumer with one or two open claims who works irregular shifts and has no fixed monthly income.
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** her reaching the income document step in the same session in which she reaches the income question, because she knows which income to enter and for which period
- **Primary success metric the one number that defines success, from M3:** the share of users who reach the affordability questions and then reach the income document step in the same session
- **Baseline rate today's rate of your primary metric, from your M3 data:** 80.7
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** the 60-day missed-payment rate among shift-income agreements (baseline 22.5%), it can move +2.8 points (one-sided 95% upper bound for B minus A; Risk review at a point estimate above +1.0 point)
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** 3
- **Sample size per arm use the calculator in the builder, baseline + MDE:** 83.7
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** 36 weeks
- **Significance threshold p < 0.05 is standard, explain any deviation:** < 0.05

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** At the income step she sees no definition and no stated period, so she can't tell whether "income" means this month or a normal month. She leaves, or continues and later picks a plan by shortcut
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** At the income field, add an inline explainer that states which income to enter, for which period, and what to do when pay varies. The copy covers these three things only. It has no content on why income is asked or how long it is kept.
- **Isolation check, what has NOT changed? list everything identical between arms (app version, eligibility rules, notifications, onboarding). If something changed inadvertently, your test is compromised.:** Product and release: same build in both arms. The only difference is the explainer layer.
Eligibility and entry: same audience, channels and entry rules.
The journey itself: same screens, same income field rules (schema, validation, required status), same Continue button, same step order.
Support and operations: same agent scripts, staffing and contact routes.
Measurement: same event definitions and logging in both arms.
Held constant: B5 (mobile upload fix) is frozen for the whole window

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** I believe that an Income explainer for a consumer with one or two open claims who works irregular shifts and has no fixed monthly income will result in her reaching the income document step in the same session in which she reaches the income question, because she knows which income to enter and for which period, as measured by a 3pt change in the share of users who reach the affordability questions and then reach the income document step in the same session within 36 weeks. We will protect the 60-day missed-payment rate among shift-income agreements (baseline 22.5%) throughout the test.
- **Your shipping criteria (filled in):** We will SHIP if the share of users who reach the affordability questions and then reach the income document step in the same session improves by ≥ 3pt at < 0.05 and the 60-day missed-payment rate among shift-income agreements (baseline 22.5%) does not reach +2.8 points (one-sided 95% upper bound for B minus A; Risk review at a point estimate above +1.0 point) after 36 weeks. We will ITERATE if direction is positive but lift is below MDE. We will KILL if the primary metric shows no improvement or moves negatively. The read date is fixed at the end of 36 weeks, no results reviewed before then.
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** _(not filled in)_
