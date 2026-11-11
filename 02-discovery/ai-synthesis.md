# AI Synthesis, Product Health & Insights Summary (Module 2)

## Responses
- **Assumption to validate #1:** A clearer and simpler digital journey will increase consumer adoption and completion.
- **Assumption to validate #2:** More affordable and personalised instalment plans will reduce missed payments and improve long-term recovery
- **Assumption to validate #3:** Better multi-claim support and information will reduce unnecessary agent contact and manual work.
- **Moment of misery / red flag #1 (e.g., “user gave up after 3 tries”):** Hits the affordability question and doesn’t know what it’s asking, or what it will be used for
- **Moment of misery / red flag #2:** Agrees to a plan without understanding the consequences
- **Moment of misery / red flag #3:** Agent picks up the pieces blind
- **Product Health & Insights Summary (Claude's output):** Product Health & Insights Summary

Digital instalment journey, German portal. Based on 12 interview notes and 8 tickets/bugs (fictional sample data, not Riverty facts).

Executive Summary

The journey is functionally live end to end, but its technical defects (a failing mobile document upload, portal amounts that differ from the letter, answers lost on navigation) block or erode confidence at the points where consumers are making financial commitments. The larger weakness is experiential: the portal does not explain why it asks for income, does not handle multiple claims, and gives no way to judge affordability or the consequences of a missed payment. Consumers and agents are compensating through abandonment, guesswork, chat shortcuts and phone calls, which pushes cost and complaint risk onto the business even where the system technically works.

Thematic Synthesis
1. Technical Stability

Defects are few but sit on critical steps. The document upload failure stops journeys outright, and the amount discrepancy undermines the integrity of what the portal presents. Both are measured in the hundreds of journeys per month, so they are systemic, not edge cases.

Income document upload times out on mobile for large photos (T-201): Critical. 853 journeys in the sample month requested a document that never arrived.
Portal amount differs from the letter (T-203): High. 531 journeys affected, 343 of them purchased-portfolio cases. The consumer impact is covered under Trust & Clarity (N-07).
Back button on plan review clears affordability answers (T-204): Medium. Forces re-entry of sensitive data at the decision point.
2. Onboarding / UX

The journey assumes one claim, a steady income and a clear idea of what is affordable. Consumers outside that pattern stall or choose badly. The evidence is qualitative, so the scale of each issue is not established in this data set.

No single plan across multiple claims (T-202): High. Consumers see one claim at a time and cannot tell whether paying one stops letters about the other (N-03). Those with three claims and tight finances report the most anxiety (N-06).
Ambiguous income question for irregular earners (N-01): High. A shift worker could not tell whether “income” meant this month or a normal month, and abandoned the journey.
Plan selection by shortcut (N-02): High. One consumer chose the shortest plan as the “right answer”, found it unaffordable and missed the second payment. This is a single account and needs corroboration.
Preference for human advice on cost (N-04): Low. Some consumers will not self-serve regardless of journey quality.
3. Trust & Clarity

Consumers are asked for sensitive information and for commitment without enough context. They don’t know why income is requested, how long it is kept, whether the figures could be used against them, or what happens if they pay late. This produces hesitation, avoidance and reliance on others for reassurance.

No explanation of why income is asked or how long it is kept (T-206): High. Linked to fear of misstatement and misuse (N-06).
Chat assistant confirms plans without showing missed-payment consequences (T-208): High. The chat is fast but leaves consumers unsure about late payment (N-05).
Amount in portal differs from the letter (N-07): High. A consumer declined to agree to anything until someone explained the gap.
Explainability of plan decisions (N-12): Medium. Compliance expects any recommendation to be explainable to consumer and agent, which the current journey does not support.
4. Support Load & Agent Enablement

Agents are working without visibility into the online journey, so calls start from zero and failed plans cannot be diagnosed. The gap also reaches the client relationship.

Agent screen shows neither consumer entries nor why a plan was offered (T-205): High. Agents re-ask details already typed online (N-08) and see only a number when a plan fails (N-09).
Broken plans surface in client reporting (N-10): Medium. The client weighs complaints alongside recovery, so unsustainable plans carry reputational and contractual exposure.
5. Data Quality & Portfolio Variance

Acquired portfolios carry uneven data, which constrains accuracy and contactability.

Unreliable phone and address history in some acquired portfolios (N-11): Medium. It limits outreach reliability and contributes to the mismatch risk seen in T-203.
Minor Technical Debt

Reminder before first instalment sent after the due date in some cases (T-207), intermittent and unquantified in this data.

Notes on Evidence
This data set contains tickets and interviews only. It has no funnel, conversion, contact-volume or missed-payment metrics, so severity ratings are qualitative judgements from ticket impact and interview content.
Several themes rest on single interviews (e.g. N-02, N-06) and should be treated as signals, not established patterns.
All figures and quotes are fictional sample data and should not be presented as Riverty research.
- **Did the AI catch the specific moment of misery / pain point you found in Step 1?:** Yes
- **Did it smooth over a critical frustration into a generic bullet point?:** No
- **Did the AI try to suggest features or a roadmap despite the constraints?:** No
- **Logic leak / hallucination #1 (e.g., “AI suggested a new search bar feature, roadmap leak”):** _(not filled in)_
- **Logic leak / hallucination #2:** _(not filled in)_
