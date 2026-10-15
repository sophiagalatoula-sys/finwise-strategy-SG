# The Mechanic · FinWise

> Module 3 · Retention & Engagement. The engagement mechanic that builds the habit loop, with rationale and a wireframe.

## The mechanic

_The habit loop: trigger → action → reward → investment._

**Mechanic:** Progress Bar: **"Week in the Clear"**. Each week has one clear finish line, *this week's cash picture is fully up to date*, reached in four quick checks. Completing it rewards the user with a concrete result about their own money, not points or badges.

- **Trigger:** A natural moment, the start of the working week, when owners plan which bills to pay and which invoices to chase. FinWise marks it with one Monday prompt ("Your week in the clear: 0 of 4. Two bills are due this week.") and timely bill alerts, nothing more. Over time the internal trigger takes over: *"Am I covered this week?"*
- **Action:** Checking their own cash-flow forecast by completing the week's four steps: review new transactions (already categorised; confirm or fix), check bills due in the next 7 days, check who still owes them (remind overdue clients, schedule reminders for upcoming ones), and check their cash runway.
- **Reward:** The progress ring fills step by step (goal-gradient effect), with copy that grows honestly ("Good start" → "Halfway there" → "Nearly there"). At 4/4: *"This week is clear ✓"*, a summary of the user's own numbers (money in, bills due and covered, money still owed, runway) plus a **"Since last time"** line that changes every week (e.g. "€2,750 more in than last week", "runway up 3 days"). That makes it a variable reward, grounded in real value.
- **Investment:** Every confirmed or corrected transaction, planned bill, chased invoice and alert makes next week's forecast more accurate *for this user*. Each cleared week is added to a visible history of "Clear" / "Partly clear" weeks. Optional extras deepen it further: a "what-if" scenario on next month (e.g. a client paying 30 days late) and sharing the week's clear picture with their accountant.


_____

## Rationale

_Why this drives retention before the paywall._

**Diagnosis first.** FinWise loses 60% of paying customers within a year of converting. Comparing the first six months of FinWise's 13-month funnel data (Oct 2023 – Mar 2024) with the last seven (Apr – Oct 2024) points to **value churn, not price churn**:
- Financial-modeling adoption nearly doubled, from 24.9% to 46.9% of users (+89%, p = 0.002), yet modeling adoption has never moved trial-to-paid conversion (r = 0.25, not significant).
- Average session length fell from 11.5 to 9.3 minutes (−19%; a trend, not statistically significant).
- The monthly churned count rose from 19.2 to 28.9 (+51%, p = 0.04).
- Sessions per user went up while sessions got shorter. Users touch more of the product and return more often, but each visit isn't solving a real problem.

Revenue per paying customer is constant across all 13 months and there's no billing-cycle data, so price churn can't be confirmed or ruled out. Exit surveys and churn timing against the billing cycle would settle it.

**This addresses value churn because** it turns each visit into one concrete answer: *exactly where my cash stands this week*. Breadth without depth is replaced by a weekly job that is finished, visibly, on the user's own numbers. Short visits are fine here (a fast, complete check is good design), as long as each one ends with a result. **A user about to churn would stay because** the value has become visible and cumulative: their forecast is accurate *because* of the weeks they've cleared, and leaving means giving up a picture they've built. The weekly cadence also means a trial user completes several cycles **before the paywall**, so the reverse trial's downgrade is felt as a real loss.

**Why this mechanic fits:**
- **Tied to a meaningful behavior:** the repeatable form of FinWise's Aha moment (seeing one's own cash-flow picture).
- **Matched to the natural cadence:** weekly, like small-business bills and invoices; daily would be nagging, and monthly gives too few repeats inside a trial.
- **Taps a real motivation:** progress toward a clear, finished week, which mirrors what missing a week actually feels like: losing sight of your cash.
- **Earns the return:** the reward is information the owner needs, with no guilt or urgency copy.
- **Connected to core value:** the mechanic *is* the core value, cash clarity, rather than points bolted onto a hollow loop.

**Decided against: a streak counter.** Missing a week feels like losing sight of your cash, not like breaking a streak, so a streak's loss aversion would fall flat. And visit frequency already rose while churn rose, so a streak would push a metric that isn't the problem. A social benchmark ("businesses like yours") was also ruled out: it adds context, not value, and could discourage the struggling businesses most likely to churn.

**How we'd know it works:** run it against a holdout group of new trial users. Measure week-4 return rate and churn per new paying customer, not just visits. Treat "Partly clear" weeks as the drop-off backlog.

_____

## Wireframe

_A link or image of the mechanic in context._

**Interactive mock-up:** https://mockup-gamification-finwise.lovable.app

Click-through states (demo switcher at the top; sample business "Northstar Creative", all data simulated):
1. **Monday trigger:** "Your week in the clear: 0 of 4" notification.
2. **Dashboard widget at 0 of 4:** progress ring + four steps, each opening a panel with one action (confirm or fix categories · mark bills as planned · send or schedule invoice reminders · check runway).
3. **Mid-week (2 of 4):** "Halfway there: 2 checks to go."
4. **Completed (4 of 4):** the "This week is clear ✓" result card with "Since last time", plus the optional what-if and accountant-share extras.
5. **History:** the last six weeks as "Clear" / "Partly clear" tiles with one-line results, including the week just cleared. No streak counter.


_____
