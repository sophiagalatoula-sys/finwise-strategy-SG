# The Validation · FinWise

> Module 5 · Experimentation Methods. The experiment brief that tests the bet.

## Method

_Test design (A/B, holdout, switchback, …) and why it fits._

**Method:** A/B Test (user-level randomization, 50/50, new trial users), with the **leading indicator** as the primary metric.

**Why:** A standard A/B test is enough for this hypothesis, so it doesn't need anything more complex. The change (a new onboarding flow) can be randomized per user, there are only two variants, and we need a clean causal read, not real-time optimization, so a multi-armed bandit adds nothing. There's no shared environment or market-level effect, so geo or switchback testing would only cost precision. What rules out the obvious design is **time**. Testing the lagging result directly (trial-to-paid, 2% → 3%) would need 3,826 trials per arm, about **14 months** at FinWise's current ~535 trials a month, and a long-term holdout would take about 40 months. Trial-to-paid has also been fixed at 2% in every one of the last 13 months, so it can't be the metric that responds first. The experiment therefore targets the leading indicator the strategy depends on, **day-0 data connection**, which needs about 612 users per arm (**~10 weeks**). Trial-to-paid is kept as a guardrail and a longer-range secondary read.


_____

## Hypothesis + primary metric

_If we [change], then [primary metric] moves by [target]._

If we replace the current onboarding with a guided four-screen flow (a one-question focus quiz → a one-click, read-only bank connection with a "try with sample data" fallback → the user's own cash-flow snapshot, led by the focus they chose → an optional accountant invite) for **new FinWise trial users**, we expect **more of them to connect their real business data in their first session**, as measured by the **day-0 data-connection rate**.

**Primary metric:** Day-0 data-connection rate: share of new trial users who connect or import their **real** business financial data in their first session (sample-data exploration doesn't count), target: **+8 percentage points, from ~44% to ≥ 52%**, statistically significant at p < 0.05 (MDE = 8 pts; ~612 users per arm at 80% power). Baseline proxy: Get Started import usage averaged 44.0% from Jul to Oct 2024.

_Experiment: **Day-0 Connect & Clarity Onboarding Test**, objective: raise the share of trial users who connect their data and see their own cash picture on day one. That's the set-up step behind FinWise's North Star (trial users who import financial data and reach their first output) and the precondition for breaking the 2% trial-to-paid ceiling: a reverse trial only converts users who have felt value they don't want to lose._

_Testing **the guided four-screen onboarding flow, shipped as one package behind a feature flag** (prototype: https://onboard-my-cash.lovable.app) on **all new FinWise trial users who sign up during the enrollment window, randomized 50/50 at user level** (existing customers and invited accountants excluded). Current experience: **FinWise's existing onboarding, in which importing data is a separate "Get Started" step that about 44% of users complete (Jul–Oct 2024 average); the rest never set up their data.**_

_Predicted outcome: **day-0 data connection rises from ~44% to at least 52%**, more trial users reach their own cash-flow snapshot (the Aha) in their first session, and week-1 return visits (the secondary leading indicator: 3+ forecast checks in week one) rise with it. If successful: **roll the flow out to all new trial users via the feature flag; then test its components one at a time (quiz vs one-click connect vs sample-data fallback) to learn which drove the lift, and run the "Week in the Clear" weekly mechanic as the next experiment on week-1 return. Keep reading trial-to-paid for the enrolled cohorts to see whether the leading indicator carries through to conversion.** If unsuccessful: **read drop-off by screen to find where users stall (most likely the bank-connection screen), check how many chose the sample-data path instead, and test an alternative set-up route (e.g. accounting-software or CSV import) before questioning the Aha moment itself.**_

_____

## Guardrail + read date

- **Guardrail:** _the metric that must not degrade (and by how much)._
  
  (1) Day-1 drop-off (trial users who never return after their first session) must not rise by more than 2 percentage points versus control: a flow that forces a bank connection must not scare users away.

  (2) Trial-to-paid conversion in the treatment arm must not fall below the 2% baseline.

  (3) No increase in onboarding-related support tickets about data access or security. If any guardrail breaks, the result is read as a Mixed Signal and investigated before shipping, even if the primary metric wins.
  
- **Read date:** _when you call it, no peeking._
  Fixed before launch: **when both arms reach 612 new trial users, about 10 weeks after launch at ~535 trials a month, and no earlier.** The secondary trial-to-paid read happens once the last enrolled cohort's reverse trial has ended. No peeking: interim dashboards are for guardrail monitoring only. Avoid launching just before the December–January dip seen in last year's data (import fell to 30.5–32.2% in Jan–Mar 2024, and sessions per user hit their low of 3 in Jan 2024), and don't run any other experiment on the same onboarding surface at the same time.
