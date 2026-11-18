# BU Collection: A Fair Way Forward

> Create affordable instalment plans that customers can understand and keep

**Sofie Petersson, Riverty Cohort 2, November 2026** · https://github.com/SofieP18/pm-final-project

Prototype: 04-roadmap/prototype.html

---

## Final Project Deliverables

### Slide 5 · Strategy
- **Problem:** # Problem Hook & Value Proposition, Module 1

- **Scenario:** Riverty BU Collection, A Fair Way Forward

## Strategic crisis
It risks losing competitiveness as other companies offer smoother digital repayment solutions, while operational costs remain high and recovery opportunities are missed

## Moment of misery
Consumers are likely using Google, calculators, spreadsheets and their banking apps to understand their finances and find affordable repayment options, or contacting customer service because Riverty's current journey does not give them enough clarity or confidence to make a decision digitally

## Problem hook
Consumers struggle to find and agree on affordable repayment plans, leading to abandoned journeys, missed recovery opportunities, higher operational costs and unnecessary agent contact

## Value proposition
For a consumer with one or two open claims who works irregular shifts and has no fixed monthly income, we will provide a simple, transparent and personalised digital journey  because we want customers to set up affordable instalment plans, while helping Riverty improve debt recovery, increase self-service and reduce manual work for collection agents.

## Cold-read self-review
The business risk is high enough to justify a new initiative, as poor digital instalment journeys can negatively impact recovery performance, increase operational costs and weaken Riverty's competitive position. This is a systemic problem rather than an edge case, as fragmented processes and unclear digital journeys create recurring challenges for both consumers and collection agents across the instalment process.
- **Value proposition:** Create affordable instalment plans that customers can understand and keep
- **Hypothesis:** # Data-Backed Hypothesis, Module 3

- **Scenario:** Riverty BU Collection, A Fair Way Forward
- **Bet type:** Optimizing the existing

## The hypothesis
She also keeps the first payments, because she knew what she was committing to and she calls an agent only when she wants advice. It maps to Retention when an a agreement is kept, 
Churn by minimizing abandoned journeys and broken plans, and
Revenue when instalments actually is collected., as measured by when the reached income document step gets over 83.7%. We will protect the 60-day missed-payment rate among shift-income agreements (baseline 22.5%, versus 17.4% for fixed salary) and make a go/no-go decision after a 50/50 test on shift-income starters, read once, 10 weeks after enrolment stops (week 36 at the latest). We will ship if reach improves by at least 3 points and the 60-day missed-payment rate stays within the guardrail (upper bound below +2.8 points, with kept agreements per 100 starters no lower than control); otherwise iterate or kill.

## Evidence
- **Qualitative (M2):** agrees to a plan without understanding the consequences
- **Quantitative (M3):** that agreements with missed payment during 60 days is 19%

## Persona & problem
- **Role:** a consumer with one or two open claims who works irregular shifts and has no fixed monthly income
- **Goal:** set up a repayment plan that fits what she can actually pay, without risking a missed payment
- **Friction:** on her break, the portal asks for her income and she cannot tell whether it means this month or a normal month. She closes the journey intending to return. In the version of her story where she does continue, she picks the plan with the fewest months because it looks like the “right answer,” finds the amount too high, and misses the second payment
- **Problem you are solving:** the income and plan commitments questions at the moment of decision

## Outcome & metrics
- **Strategic outcome:** finishing the income step in one sitting, that she chooses a plan by its terms and consequences instead of by screen order or length.
She also keeps the first payments, because she knew what she was committing to and she calls an agent only when she wants advice. It maps to Retention when an a agreement is kept, 
Churn by minimizing abandoned journeys and broken plans, and
Revenue when instalments actually is collected.
- **Primary success metric:** when the reached income document step gets over 83.7%
- **Guardrail metric:** the 60-day missed-payment rate among shift-income agreements (baseline 22.5%, versus 17.4% for fixed salary)
- **Decision window:** run a 50/50 test on shift-income starters, read once, 10 weeks after enrolment stops (week 36 at the latest). Ship if reach improves by at least 3 points and the 60-day missed-payment rate stays within the guardrail (upper bound below +2.8 points, kept agreements per 100 starters no lower than control); otherwise iterate or kill

### Slide 6 · Research
- **Competitive analysis:** # Persona & Future-State Journey, Module 2

- **Scenario:** Riverty BU Collection, A Fair Way Forward

## Persona
- **Role:** A consumer with one or two open claims who works irregular shifts and has no fixed monthly income
- **Goal:** Set up a repayment plan that fits what she can actually pay, without risking a missed payment
- **Friction:** On her break, the portal asks for her income and she cannot tell whether it means this month or a normal month. She closes the journey intending to return. In the version of her story where she does continue, she picks the plan with the fewest months because it looks like the “right answer,” finds the amount too high, and misses the second payment

## Current workaround (the status quo to beat)
- **External tools:** Use the "plan order" as a decision rule
- **The process:** Gets past the affordability step despite the ambiguity.
Lacks a way to test what she can safely afford, so she substitutes a shortcut: the fewest-months option looks like the “right answer.”
Commits to that plan.
Finds the amount too high and misses the second payment
- **Core frustration:** First in the affordability step where she cannot tell whether she should provide this month or a normal month and then in the plan review step.
- **The evidence:** “I picked the plan with the lowest number of months because it looked like the right answer. The amount was too high and I missed the second payment”

## Future-state journey map
1. See my case

User action
Opens reminder link, sees both claims together → knows total owed instantly.

Internal state
Case data verified and freshness-checked → context captured from first click.

Pain point addressed
Unclear scope and confusion → customer stays instead of closing
2. Share income simply

User action
Picks "typical month" or "this month" range → answers without guessing.

Internal state
Uncertain inputs flagged low-confidence → routed to a human, never auto-declined.

Pain point addressed
Ambiguous income question → stated purpose reduces abandonment.
3. Choose a plan that fits

User action
Compares plans with a safe-amount default → picks sustainable, not shortest.

Internal state
Options bounded by affordability, not highest payment → fairer, lower default risk.

Pain point addressed
Fewest months looks "right" → prevents missed second payment.
4. Confirm and stay on track

User action
Confirms plan, sees missed-payment rules → trusts the commitment.

Internal state
Plan, reasoning and override trail logged → agents skip repeat checks.

Pain point addressed
Fear of consequences and missed payments → early help path.

## Competitive advantages
Fewer drop-offs: Plain-language income prompts and a “safe amount” default replace call-back guesswork, so the customer finishes the journey the first time.
No repeated checks for agents: Entered data, confidence flags and reasons arrive with the case, so agents correct exceptions instead of re-asking everything.
Plans built to be kept: Affordability-bounded options reduce missed payments, so a rising SSR reflects better outcomes rather than plans that collapse.
- **Journey map:** She opens the link, scans to the income question, hesitates because she cannot tell which income to enter, and bounces. The explainer steps in at that exact moment, so she answers with confidence and keeps going.

### Slide 7 · Blueprint
- **Roadmap:** # Feature Roadmap, Module 4 · BU Collection

**Scenario:** Riverty BU Collection, A Fair Way Forward

**Team:** [your assumed team size]

## Strategic anchors
- **Persona:** A consumer with one or two open claims who works irregular shifts and has no fixed monthly income
- **Primary metric:** When the reached income document step gets 3 points above 80.7% (83.7% or more)
- **Moment of misery:** On her break, the portal asks for her income and she cannot tell whether it means this month or a normal month. She closes the journey intending to return. In the version of her story where she does continue, she picks the plan with the fewest months because it looks like the “right answer,” finds the amount too high, and misses the second payment
- **Guardrail:** The 60-day missed-payment rate among shift-income agreements stays protected (baseline 22.5%, versus 17.4% for fixed salary).

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
| B1 One plan for several claims | 2 | 5 | Time Sinker | Next | Strong for multi-claim consumers, but she has one or two claims and it would consume most of the quarter. |
| B2 Income explainer | 4 | 1 | Quick Win | Now | Fixes her first Moment of Misery cheaply if it says which income to enter, but it only indirectly moves the missed-payment gap. |
| B3 Affordability check before plan options | 5 | 3 | Major Project | Next | Replaces her shortcut plan choice with a basis for choosing, the main lever on the 5.1-point shift-income missed-payment gap. |
| B4 Agent handoff summary | 2 | 2 | Fill-In | Later | Cuts agent re-asking (N-08), but it doesn’t change what she sees or whether her plan holds |
| B5 Mobile upload fix or skip document | 4 | 2 | Quick Win | Now | Removes a real failure (T-201), but it is a conversion fix, not her plan-choice problem, and skipping the document could weaken affordability data. |
| B6 Pay-day date | 3 | 3 | Time Sinker | Later | Plausible for missed payments, but unsupported by the research, and irregular shifts may not give her a fixed pay day |
| B7 Shortest plan first | 1 | 1 | Fill-In | Cut | Reject: it repeats the Month 4 change, when missed payments rose from 15.6% to 18.4%, and works against the guardrail. |
| B8 Chat assistant on every page | 1 | 4 | Time Sinker | Cut | The chat confirms plans without showing consequences (T-208), and chat users miss more (21.6% vs 18.3%), so it spreads her shortcut problem. |

### NOW, this sprint
- **B2 Income explainer**, Fixes her first Moment of Misery cheaply if it says which income to enter, but it only indirectly moves the missed-payment gap.
- **B5 Mobile upload fix or skip document**, Removes a real failure (T-201), but it is a conversion fix, not her plan-choice problem, and skipping the document could weaken affordability data.

### NEXT, the following sprints
- **B1 One plan for several claims**, Strong for multi-claim consumers, but she has one or two claims and it would consume most of the quarter.
- **B3 Affordability check before plan options**, Replaces her shortcut plan choice with a basis for choosing, the main lever on the 5.1-point shift-income missed-payment gap.

### LATER, backlog
- **B4 Agent handoff summary**, Cuts agent re-asking (N-08), but it doesn’t change what she sees or whether her plan holds
- **B6 Pay-day date**, Plausible for missed payments, but unsupported by the research, and irregular shifts may not give her a fixed pay day

### ✂ Cut List
- **B7 Shortest plan first**, Reject: it repeats the Month 4 change, when missed payments rose from 15.6% to 18.4%, and works against the guardrail.
- **B8 Chat assistant on every page**, The chat confirms plans without showing consequences (T-208), and chat users miss more (21.6% vs 18.3%), so it spreads her shortcut problem.
- **PRD highlights:** # Income explainer, Simplified PRD (Riverty BU Collection, A Fair Way Forward)

**Scenario:** Riverty BU Collection, A Fair Way Forward

**Author:** Me · **Status:** Draft · **Target:** High-Fidelity Prototype · **Persona:** Shift workers with one or two open claims and irregular income

## 1. The Big Picture
- **Vision:** To eliminate the guesswork that makes shift workers abandon or regret their repayment plan, by explaining what the income question means and what each plan commits them to.
- **Press release:** Riverty makes the income question answerable in one sitting

Today, Riverty launched a plain-language income explainer in its German instalment portal. At the income field, consumers with irregular pay now see which income to enter and what to do when pay varies, in a few lines readable on a phone during a break. They can answer in one sitting, with confidence, instead of closing the page meaning to come back.

It is the first step of “A Fair Way Forward”, Riverty’s effort to help consumers agree to repayment plans they understand and can keep.
- **Success metric:** When the reached income document step gets 3 points above 80.7% (83.7% or more)
- **Guardrail:** The 60-day missed-payment rate among shift-income agreements stays protected (baseline 22.5%, versus 17.4% for fixed salary).

### User stories
- As a shift worker entering my income, I want a plain statement of which figure to enter, so that I can fill in the field with confidence and move on to the document step.
- As a shift worker whose pay changes from month to month, I want a clear rule for what to enter when my income is irregular, so that I’m not guessing and don’t give a figure that misrepresents what I can afford.
- As a shift worker on the income screen, I want the explanation on the same screen as the field, so that I don’t have to leave the step to find out what to enter and don’t drop off before the document step.
### Screens to build
- Entry point: income step with explainer trigger
- Feature core: explainer open)
- Success / confirmation: income entered, ready to continue
### Functional requirements
- FR-1: The explainer opens in place on the income screen, with no navigation away.	Zero page or route changes on open. The explainer is visible within 1 second of the tap, tested on the smallest supported mobile viewport [360 px]
- FR-2: Opening and closing the explainer never alters what the user has typed.The income field value is identical before open and after close in 100% of test cases, including on mobile.
- FR-3: The trigger is visible on the income screen without scrolling, and the Continue button works whether or not the explainer was opened.	The trigger is in view at the minimum viewport 360 px and has a tap target of at least 44×44 px. A user can proceed with zero explainer interactions.
- FR-4: The explainer states which income to enter (net or gross) and for which period, in no more than two sentences. The text is a verbatim match to the Risk-approved definition, with a sentence count of 2 or fewer.
- FR-5: The explainer gives one rule for working out a typical month when pay is irregular. The approved rule from Risk appears in 100% of explainer displays. Exactly one rule is shown, with no alternatives.
- FR-6: The income field’s schema, validation and required status are unchanged, and no screen or step is added before the document step.	Zero differences in field rules in regression tests against the current release. The step count before the document step is the same as the baseline.
- FR-7: No explainer copy goes live without recorded Compliance or Risk approval.	100% of live copy versions carry an approval reference [ID, approver, date]. Release is blocked if one is missing.
- FR-8: The funnel events needed for the primary metric are logged. Five events are captured: income step reached, explainer opened, income edited after explainer viewed, document step reached, and drop-off at the income field. Event capture is at least 95% against a manual QA check, identical in both arms. The denominator and window are written into the PRD.
### Smart behaviors (Situation → Outcome)
- If she lands on the income step, then show the one-line helper and the “Which income do I enter?” trigger without scrolling.
- If she taps the trigger, then open the explainer in place and keep anything she has already typed.
- If she closes the explainer (“Got it”), then return her to the income field with her entry intact and the cursor in the field.
- If she never opens the explainer, then let her continue as normal, with no forced read and no extra step.
- If she opens the explainer, then show the approved definition first (which income, which period) and the irregular-shift rule second.
- If she edits the income field after viewing the explainer, then log “income edited after explainer viewed” and apply the existing validation unchanged.
- If her entry fails the existing validation, then show the standard error and keep the trigger visible.
- If she completes the income step, then show the basis of what she entered (for example “Monthly net income: [value]”) and enable Continue to the document step.
- If she reaches the document step, then log it against the primary metric (target 83.7% or more, 3 points above the 80.7% baseline).
- If she leaves the income step without completing it, then log the drop-off at the income field, with or without an explainer view.
- If the explainer fails to load, then keep the helper line and the income field working so she can still proceed, and log the failure. The feature must never block the step.
- If copy has no recorded Compliance or Risk approval, then block the release (FR-7).
- Should have: if she expands the worked example or the “what counts” list, then keep it collapsed by default and log the expansion.
- Should have: if the missed-payment rate or affordability data quality moves outside the agreed guardrail at the review point [date], then flag it for review before the explainer is extended.
### Technical constraints
- No backend, DB or API change

### Features out
- Affordability check before plan options
- Mobile upload fix or skipping the document
- One plan for several claims
- Agent handoff summary
- Pay-day date
- Chat assistant on every page
- Shortest plan first
- Income verification or bank-data pull
- Changes to the income field (schema, validation, required status)
- Redesign of the income step	The explainer is a layer on the existing step, not a new flow.
- Any new screen or step before the document
- Income calculator or averaging helper
- Sanity nudge for wrong-basis entries
- Employment-type copy variants
- Pre-fill from earlier entries
### Edge cases & safety guard
- Empty income field → safety: never invent a figure. No pre-fill, no suggested amount, and no placeholder that looks like a real value.
- Approved definition missing → safety: never invent wording. Hide the explainer, keep the income field working, and block the release (FR-7).
- Irregular-pay rule missing or unapproved → safety: never invent a rule. Show only the approved basis line, with no improvised averaging advice.
- No pay periods or a zero-income month → safety: never invent a typical month. The explainer states the rule and does not calculate for her.
- Overtime, shift premiums, benefits or a second job not covered by the approved copy → safety: never invent whether it counts. Don’t say it counts or that it doesn’t.
- Explainer fails to load → safety: never invent fallback text. Show the approved helper line only, keep Continue working, and log the failure.
- Translation missing or unapproved for a language → safety: never invent a machine translation. Don’t release that language until it is approved [confirm fallback with Compliance].
- Entry fails existing validation → safety: never invent a corrected value. Show the standard error and don’t auto-correct her entry.
- Entry looks like the wrong basis (for example gross, not net) → safety: never invent a correction. Accept it as the system does today. A nudge is V2.
- Effect of her entry on approval or plan unknown → safety: never invent consequences. The copy makes no claims about outcomes, and Risk must confirm any such statement.
- Worked example data absent → safety: never invent real-user numbers. Use clearly labelled illustrative figures only (Should-Have).
- Approval reference missing for a copy version → safety: never invent an approval. The release pipeline blocks the version.
- Funnel baseline, denominator or window missing → safety: never invent a metric result. Report “not measurable”, not an estimated reach rate against 80.7%.
- Event not logged or capture incomplete → safety: never invent funnel numbers. No interpolation, and gaps are shown as gaps.
- Guardrail data (missed-payment rate, affordability data quality) missing at the review date → safety: never invent a pass. Report it as unknown and flag it for review.
### Decision log
- Explains the income question and does not act on the answer
- Front-end and copy only: no API, DB or logic change
- The journey map has four stages. This release covers stage 2 only, as an explainer layer. Stages 1, 3 and 4 follow with B1 and B3.
### Evals
- Accuracy: does she enter the right income? ≥ 90% of test participants enter the income asked for
- Time-on-task: can she finish on her break? ≥ a median of 60 seconds or less from income step viewed to income confirmed on mobile, with the slowest 10% under 120 seconds
- Safety: does it avoid every “never”? ≥ 100% pass, with 0 violations

## MoSCoW scope
- **Must:** Inline explainer at the income field. It sits on the same screen, with no link out, and works on mobile. If it sends her away from the step, it can only hurt the reach rate.; One plain rule for which income to enter, including irregular shifts. It states the basis (net or gross), the period, and how to arrive at a typical month when pay varies. This is the Moment of Misery, so a feature without it does nothing. Risk or Credit Policy must supply the definition.; Approved copy. Compliance or Risk signs off, because the wording defines the data behind the affordability check.; No change to the income field’s data or validation. The schema, required status and rules stay as they are. This protects the affordability data and avoids a dev dependency inside one sprint.; Instrumentation for the metric. Log the step-reach rate with a pinned denominator, explainer viewed, and drop-off at the income field. Without this you can’t tell whether the 83.7% target was hit.
- **Should:** Log income edited after the explainer is viewed. This is a leading signal that the explainer changed behaviour.; One worked example for a shift worker. It uses clearly illustrative numbers.; “What counts / what doesn’t” list. It covers overtime, shift premiums, benefits and second jobs, collapsed by default so the step stays short.; Accessibility and translation of the copy. If company standards require these, they move to Must.; Guardrail monitoring. Watch the missed-payment rate and affordability data quality alongside the primary metric. A step-reach metric can be hit by pushing people through with a wrong number.
- **Could:** Employment-type variants of the copy.; Averaging helper that calculates a typical month from recent pay periods.; Sanity nudge for entries that look like the wrong basis.; Copy A/B tests.; Pre-fill from earlier entries.
- **Won't (now):** Mobile upload fix or skipping the document (B5). This acts after the step is reached, so it doesn’t move this metric. It also risks weakening affordability data.; Affordability check or plan recommendations (B3).; Chat assistant (B8), agent handoff summary (B4), pay-day date (B6) and multi-claim plans (B1).; Income verification or a bank-data pull.; Redesign of the income step or changes to which fields are required.; Any extra step or screen before the document step. It would work against the metric.
- **Prototype:** 04-roadmap/prototype.html

### Slide 8 · Validation
## Parameters
| Parameter | Decision |
| Feature under test | an Income explainer |
| Persona | a consumer with one or two open claims who works irregular shifts and has no fixed monthly income |
| Expected outcome | her reaching the income document step in the same session in which she reaches the income question, because she knows which income to enter and for which period |
| Primary success metric | the share of users who reach the affordability questions and then reach the income document step in the same session |
| Baseline rate | 80.7% (re-measure on the exact same-session definition before launch) |
| Guardrail metric | the 60-day missed-payment rate among shift-income agreements (baseline 22.5%) |
| Guardrail boundary | +2.8 points (one-sided 95% upper bound for B minus A; Risk review at a point estimate above +1.0 point) |
| Second guardrail | Documents needing review (baseline 28.0%) no more than +2.0 points above A. Companion: kept agreements per 100 randomised shift-income users no lower than A, and the shift-income agreement rate no more than 3.0 points below A. A guardrail failure overrides a primary win: do not ship |
| Minimum Detectable Effect | 3pt |
| Sample size per arm | 2,551 minimum for the primary. Enrol until 5,500 pooled shift-income agreements are reached, with a cap of 26 weeks (the stop rule is written before launch and uses the agreement count only, never outcome data). Then wait 10 weeks (60-day window, agreement-creation lag and data lag) and read once. The read is expected at about week 30 if the real rate is about 275 agreements a week, and at week 36 at the latest. The guardrail needs about 5,500 pooled shift-income agreements, and 7,150 are expected over 26 weeks. Between 4,500 and 5,500 the guardrail still applies, with about 73 to 80% power. If fewer than 4,500 exist at the 26-week cap, the guardrail is monitoring only and a ship needs written Risk sign-off in place of the guardrail condition. Change freeze on the income step and plan screen for the whole window. |
| Traffic split | 50/50 |
| Test duration | About 30 weeks expected, 36 weeks at most |
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

### Slide 9 · Launch
- **GTM:** # GTM Launch Plan, Riverty BU Collection, A Fair Way Forward

| Field | Value |
| Feature | Income explainer |
| Goal | Conversion |
| Launch tier | M, Targeted |

## Goal & Audience
- **Goal:** Conversion, convert more shift workers who reach the income question into users who complete the income step and reach the income document step in the same session, with the 60-day missed-payment rate protected.
- **Target audience:** consumers in the instalment portal who reach the income question. Persona within them: shift-income consumers with one or two open claims. Targeted by place (the income step) and by message, not by user. Internal enablement audience: collection agents, Risk, Compliance and client account managers.

## Launch Tier
- **M, Targeted**, About 3,700 users a month are exposed during enrolment (up to 26 weeks), and about 7,364 a month after a ship. During the 10-week wait after enrolment stops: arms stay as assigned, nobody new is counted, nothing changes until the read. Upper-bound impact at a 3-point lift: about 140 extra agreements and €9,000 a month committed (about €7,300 intact at 60 days), assuming marginal users convert like average. Nothing is realised until a ship decision at the read (about week 30, week 36 at the latest). M reflects the internal briefing for agents, Risk and client managers, not a consumer campaign.

## Channels
1. **Owned: active from launch: the income step in the instalment portal. It is the only channel that carries the message during the test.**
2. **Owned: held: SMS and email reminders, unchanged until a ship decision. After a ship, add a “have your net monthly pay ready” line.**
3. **Owned: enablement only: the agent phone line, same scripts and no new wording. After a ship, an updated script and training.**

## Enablement & Assets
One-page launch brief, Agent quick-reference card, Client talking points, Approval pack, Escalation and kill-switch runbook, Contact-reason code “income question”

## Ownership, Budget & Timeline
- **Ownership & budget:** The Risk / Credit Policy lead owns the approval of the income definition and the irregular-pay rule, due L-5 weeks. No extra cost.
The content or UX writer owns the German copy and translations, due L-4 weeks. Extra cost: translation, if it is not done in-house (amount to be quoted).
The Compliance reviewer owns the approval of the final copy and records the approval reference ID, due L-3 weeks. No extra cost.
The Compliance reviewer owns the approval pack (approved copy, reference ID, version log, and the rule that any wording change goes back through approval), due L-3 weeks. No extra cost.
The engineering lead owns building the explainer (helper line, link and panel), due L-2 weeks. Extra cost: sprint capacity.
The engineer or analytics engineer owns logging the five events identically in both arms, due L-2 weeks. Extra cost: sprint capacity.
The data analyst owns re-measuring the same-session baseline, fixing the shift-income classification, checking the real weekly agreement count and confirming what “documents needing review” includes, due L-3 weeks. Extra cost: analyst time.
The UX researcher owns the safety and usability test (accuracy of at least 90%, time on mobile), run on a prototype with the approved copy, due L-2 weeks. Extra cost: participant recruitment and incentives.
The PM owns the decision on B5, either shipped to both arms or frozen, due L-4 weeks. Extra cost: sprint capacity either way.
The Risk lead owns the written agreement of the 2.8-point margin, the +1.0 review trigger and the +2.0 documents limit, due L-2 weeks. No extra cost.
The engineering lead owns testing the kill switch and writing the runbook, due L-1 week. No extra cost.
The PM owns the launch brief, the agent quick-reference card and the client talking points, due L-1 week. No extra cost.
The agent team lead owns the new contact-reason code “income question”, due L-1 week. No extra cost.
The data analyst owns the launch-week checks of sample ratio and logging, in weeks 1 and 2. Extra cost: analyst time.
The data analyst owns the weekly check of sample ratio, logging and safety incidents, with no outcome peeking, weekly until the read. Extra cost: analyst time.
The PM owns the read and the decision at the read date (about week 30, week 36 at the latest). The Risk lead signs off in writing if the review tier triggers. No extra cost.
The data analyst or BI engineer owns the guardrail reporting (missed-payment rate, kept agreements per 100 randomised users, documents needing review), due L-2 weeks. Extra cost: analyst or engineering time.
The engineering lead owns the change freeze on the income step and plan screen for the whole window.
The Risk lead can pull the kill switch alone. The PM can pull it on a safety incident and tells the Risk lead the same day.
The PM owns getting quotes for translation and participant incentives, due L-5 weeks.
The PM owns the decision communication to agents, Risk, Compliance and client managers, due week 38.
Budget: no media or campaign spend. Amounts for translation, participant incentives, analyst time, sprint capacity and agent briefing time are not yet approved. The PM owns getting the quotes by L-5 weeks, and the head of product approves a total cap before launch.
Asset gaps before launch: the approved wording, the German copy, a production screenshot for the agent card, the guardrail dashboard, and the agent team size.
The agent team lead owns confirming the agent team size and who takes income-related calls, due L-3 weeks.
The PM owns the production screenshot for the agent card, due L-1 week.
The PM owns the rollout brief if the explainer ships, due week 40.
The agent team lead owns the updated agent script and training if the explainer ships, due week 42.
The marketing lead owns the updated “have your net monthly pay ready” line if the explainer ships, due week 42.
The data analyst owns the 60-day missed-payment tracking after a ship, reported monthly to the Risk lead.
The engineering lead executes any kill-switch request, or the shutdown after a killed test, within 1 hour.
- **Timeline:** Phase 1: Beta (L-5 weeks to L)

L-5 to L-3 weeks: the Risk / Credit Policy lead approves the income definition and irregular-pay rule. The writer produces the German copy. The Compliance reviewer approves it and records the reference ID.
L-3 weeks: the data analyst re-measures the same-session baseline, fixes the shift-income classification and checks the real weekly agreement count.
L-2 weeks: the engineering lead builds the explainer and logs the five events identically in both arms. The UX researcher runs the safety and usability test on the prototype. The Risk lead agrees the 2.8-point margin, the +1.0 review trigger and the +2.0 documents limit in writing.
L-1 week: the engineering lead tests the kill switch. The PM issues the launch brief, agent card and client talking points. Any fixes from the usability test are made and re-checked.
L-1 week to L: internal dry run, then a soft ramp to a small share of traffic. The analyst checks the sample ratio and logging on that data.
Go / no-go gate at L: approved copy with a reference ID, baseline re-measured, B5 decided, kill switch tested, accuracy at least 90% with 0 safety violations, sample ratio clean and event capture complete in the ramp, Risk margins agreed. Users in the soft ramp are excluded from the final read. The real weekly pooled shift-income agreement count is at least 173; if it is lower, the PM decides before launch whether to lengthen enrolment or accept a monitoring-only guardrail. The guardrail dashboard is live and the budget cap is approved.

Phase 2: Launch moment (week 0 to week 2)

Week 0: switch to the full 50/50 split. The launch brief goes to agents, Risk, Compliance and account managers the same day. Agents get no new script.
Weeks 1 and 2: the data analyst checks the sample ratio, logging completeness and any safety incident. Nobody looks at outcome results.
Gate at the end of week 2: sample ratio passes, event capture is complete, no safety incident. If it fails, pause, fix, and restart the clock.

Phase 3: Post-launch (week 3 to week 38 at the latest)

From week 3 until enrolment stops: the weekly integrity check continues. The only three things reviewed are sample ratio, logging and safety incidents.
Enrolment stop rule: stop enrolment when the pooled shift-income agreement count reaches 5,500, or at week 26, whichever comes first. The rule is written down before launch and uses the agreement count only, never outcome data. At the stop, the data analyst confirms the count against 5,500, with 4,500 as the floor, and writes down the read date before any outcome is looked at.
Wait 10 weeks after enrolment stops for the 60-day window and the data lag. The 50/50 split keeps running so nothing changes for users. New arrivals are not counted in the read. At about 275 agreements a week, enrolment stops around week 20; at 173 a week, at the week 26 cap.
Read: 10 weeks after enrolment stops (about week 30 expected, week 36 at the latest), the PM reads the result once. The Risk lead signs off in writing if the review tier triggers.
Weeks 37 to 38: decide. If it ships, build the rollout brief, an updated agent script with training, and an updated reminder message. If it iterates, plan the next test, with no extension. If it is killed, turn the explainer off.
After a ship, keep tracking the 60-day missed-payment rate as follow-up.

## Success Metrics
- **Metrics:** Primary: the share of users who reach the affordability questions and then reach the income document step in the same session. Baseline 80.7% (re-measure before launch). Success: +3.0 points or more, p < 0.05, read once at the read date. Also report the persona subgroup.
Quality: the share of uploaded income documents needing review. Baseline 28.0%. Success: B no more than 2.0 points above A.
Protection: the 60-day missed-payment rate among shift-income agreements. Baseline 22.5%. Success: one-sided 95% upper bound for B minus A below +2.8 points. Companion: kept agreements per 100 randomised shift-income users no lower than A.
- **Bad signal to watch for:** documents needing review in B is more than 2.0 points above A while reach rises. People were pushed through with a guess, so the lift is not a win, and a guardrail failure overrides it. Read at the read date, not before.
- **Likely post-launch decision:** one pre-registered safety look at week 8 on documents needing review only. If B is more than 4.0 points above A, the PM turns the explainer off and the Risk lead reviews within 5 working days. This catches large harm only; the +2.0 limit is decided at the read.
- **Metrics:** Reach income document step in same session, if less than 83.7% reaches, it is not clear enough
Income documents needing review, documents needing review rise more than 2 points
60-day missed-payment rate (shift workers), customers finish the step but can’t keep the plan

### Slide 10 · Story
- **Friction + aha:** What was hard: Taking in everything AI produced. It generated a lot of information and data very quickly, and with the limited time we had, it was hard to read, check and decide what actually mattered.

What surprised me: AI smoothed over a real frustration, labelling “reminder sent after the due date” as minor technical debt.

The aha moment: When I understood the “what is the exact moment she gives up” and could base the concept about that
- **Takeaways / next:** Biggest learnings:
AI executes, I decide what is worth asking and whether the answer is right.
One sharp moment of misery beats a long feature list.
A metric win only counts if guardrails hold.

Build my AI skills further, so I can prompt better, check outputs faster and get more useful help and understanding from AI in future projects.

---

Submitted to the Product Management Certification learning platform · Product School.
