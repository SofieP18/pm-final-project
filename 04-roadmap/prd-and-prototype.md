# Income explainer, Simplified PRD (Riverty BU Collection, A Fair Way Forward)

**Scenario:** Riverty BU Collection, A Fair Way Forward

**Author:** Me · **Status:** Draft · **Target:** High-Fidelity Prototype · **Persona:** Shift workers with one or two open claims and irregular income

## 1. The Big Picture
- **Vision:** To eliminate the guesswork that makes shift workers abandon or regret their repayment plan, by explaining what the income question means and what each plan commits them to.
- **Press release:** Riverty makes the income question answerable in one sitting

Today, Riverty launched a plain-language income explainer in its German instalment portal. At the income field, consumers with irregular pay now see which income to enter and what to do when pay varies, in a few lines readable on a phone during a break. They can answer in one sitting, with confidence, instead of closing the page meaning to come back.

It is the first step of “A Fair Way Forward”, Riverty’s effort to help consumers agree to repayment plans they understand and can keep.
- **Success metric:** When the reached income document step gets 3 points above 80.7% (83.7% or more)
- **Guardrail:** The 60-day missed-payment rate among shift-income agreements stays protected (baseline 22.5%, versus 17.4% for fixed salary).

## 2. The Details
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

## 3. The Logistics
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
### Evals
- Accuracy: does she enter the right income? ≥ 90% of test participants enter the income asked for
- Time-on-task: can she finish on her break? ≥ a median of 60 seconds or less from income step viewed to income confirmed on mobile, with the slowest 10% under 120 seconds
- Safety: does it avoid every “never”? ≥ 100% pass, with 0 violations

## MoSCoW scope
- **Must:** Inline explainer at the income field. It sits on the same screen, with no link out, and works on mobile. If it sends her away from the step, it can only hurt the reach rate.; One plain rule for which income to enter, including irregular shifts. It states the basis (net or gross), the period, and how to arrive at a typical month when pay varies. This is the Moment of Misery, so a feature without it does nothing. Risk or Credit Policy must supply the definition.; Approved copy. Compliance or Risk signs off, because the wording defines the data behind the affordability check.; No change to the income field’s data or validation. The schema, required status and rules stay as they are. This protects the affordability data and avoids a dev dependency inside one sprint.; Instrumentation for the metric. Log the step-reach rate with a pinned denominator, explainer viewed, and drop-off at the income field. Without this you can’t tell whether the 83.7% target was hit.
- **Should:** Log income edited after the explainer is viewed. This is a leading signal that the explainer changed behaviour.; One worked example for a shift worker. It uses clearly illustrative numbers.; “What counts / what doesn’t” list. It covers overtime, shift premiums, benefits and second jobs, collapsed by default so the step stays short.; Accessibility and translation of the copy. If company standards require these, they move to Must.; Guardrail monitoring. Watch the missed-payment rate and affordability data quality alongside the primary metric. A step-reach metric can be hit by pushing people through with a wrong number.
- **Could:** Employment-type variants of the copy.; Averaging helper that calculates a typical month from recent pay periods.; Sanity nudge for entries that look like the wrong basis.; Copy A/B tests.; Pre-fill from earlier entries.
- **Won't (now):** Mobile upload fix or skipping the document (B5). This acts after the step is reached, so it doesn’t move this metric. It also risks weakening affordability data.; Affordability check or plan recommendations (B3).; Chat assistant (B8), agent handoff summary (B4), pay-day date (B6) and multi-claim plans (B1).; Income verification or a bank-data pull.; Redesign of the income step or changes to which fields are required.; Any extra step or screen before the document step. It would work against the metric.

