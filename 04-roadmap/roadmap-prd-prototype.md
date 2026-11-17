# Feature Roadmap, Module 4 · BU Collection

**Scenario:** Riverty BU Collection, A Fair Way Forward

**Team:** [your assumed team size]

## Strategic anchors
- **Persona:** A consumer with one or two open claims who works irregular shifts and has no fixed monthly income
- **Primary metric:** When the reached income document step gets over 80.7%
- **Moment of misery:** On her break, the portal asks for her income and she cannot tell whether it means this month or a normal month. She closes the journey intending to return. In the version of her story where she does continue, she picks the plan with the fewest months because it looks like the “right answer,” finds the amount too high, and misses the second payment
- **Guardrail:** When the shift-income rate falls toward the fixed-salary rate (22.5% vs 17.4% for fixed salary), a 5.1-point fall ideally with the 60-day rate following later as confirmation.

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
|---|---|---|---|---|---|
| B1 One plan for several claims | 2 | 5 | Time Sinker | Next | Strong for multi-claim consumers, but she has one or two claims and it would consume most of the quarter. |
| B2 Income explainer | 4 | 1 | Quick Win | Now | Fixes her first Moment of Misery cheaply if it says which income to enter, but it only indirectly moves the missed-payment gap. |
| B3 Affordability check before plan options | 5 | 3 | Major Project | Next | Replaces her shortcut plan choice with a basis for choosing, the main lever on the 5.1-point shift-income missed-payment gap. |
| B4 Agent handoff summary | 2 | 2 | Fill-In | Later | Cuts agent re-asking (N-08), but it doesn’t change what she sees or whether her plan holds |
| B5 Mobile upload fix or skip document | 4 | 2 | Quick Win | Now | Removes a real failure (T-201), but it is a conversion fix, not her plan-choice problem, and skipping the document could weaken affordability data. |
| B6 Pay-day date | 3 | 3 | Time Sinker | Later | Plausible for missed payments, but unsupported by the research, and irregular shifts may not give her a fixed pay day |
| B7 Shortest plan first | 1 | 1 | Fill-In | Cut | Reject: it repeats the Month 4 change, when missed payments rose from 15.6% to 18.4%, and works against the guardrail. |
| B8 Chat assistant on every page | 1 | 4 | Time Sinker | Cut | The chat confirms plans without showing consequences (T-208), and chat users miss more (21.6% vs 18.3%), so it spreads her shortcut problem. |

## Roadmap
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
