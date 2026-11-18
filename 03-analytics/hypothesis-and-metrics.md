# Data-Backed Hypothesis, Module 3

- **Scenario:** Riverty BU Collection, A Fair Way Forward
- **Bet type:** Optimizing the existing

## The hypothesis
> Based on that agreements with missed payment during 60 days is 19%, we believe that solving the income and plan commitments questions at the moment of decision for a consumer with one or two open claims who works irregular shifts and has no fixed monthly income will result in finishing the income step in one sitting, that she chooses a plan by its terms and consequences instead of by screen order or length.
She also keeps the first payments, because she knew what she was committing to and she calls an agent only when she wants advice. It maps to Retention when an a agreement is kept, 
Churn by minimizing abandoned journeys and broken plans, and
Revenue when instalments actually is collected., as measured by when the reached income document step gets over 83.7%. We will protect the 60-day missed-payment rate among shift-income agreements (baseline 22.5%, versus 17.4% for fixed salary) and make a go/no-go decision after a 50/50 test on shift-income starters, read once at week 36. We will ship if reach improves by at least 3 points and the 60-day missed-payment rate stays within the guardrail (upper bound below +2.8 points, with kept agreements per 100 starters no lower than control); otherwise iterate or kill.

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
- **Decision window:** run a 50/50 test on shift-income starters, read once at week 36. Ship if reach improves by at least 3 points and the 60-day missed-payment rate stays within the guardrail (upper bound below +2.8 points, kept agreements per 100 starters no lower than control); otherwise iterate or kill
