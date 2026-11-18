# GTM Launch Plan, Riverty BU Collection, A Fair Way Forward

| Field | Value |
|---|---|
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
