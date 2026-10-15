# The Signals · FinWise

> Module 4 · Data & Analytics. The data pattern you found and the indicators you'll steer by.

## The data pattern

_What the funnel data revealed, the real problem behind the headline metric._

The headline metric is **trial-to-paid conversion at ~2%**, but the real pattern behind it is a **ceiling**: conversion stays at exactly 2% of trials no matter what happens during the trial. Over 13 months (Oct 2023 – Oct 2024), paid conversions equal trials × 2% (rounded) in every single month. The monthly rate moves by about ±0.06 percentage points, where random variation alone would move it by about ±0.63, and in 20,000 simulations of a random 2% rate none stayed this flat. Meanwhile, data import rose 19%, financial-modeling adoption nearly doubled and visits per user went up, and none of it moved conversion. **The product delivers the same outcome whatever trial users do, so more set-up or more feature usage won't break the ceiling.** It needs a new value moment before the paywall, and that has to be proven with **user-level** data (trial users who import and return vs those who don't), because monthly totals can't show what drives a rate that never moves.

_Metric patterns: Conversion, **Ceiling** (1.87–2.08% in all 13 months, no trend: r = 0.22, p = 0.48). Modeling usage, **doesn't fit cleanly**: strong growth with volatility (24.9% → 46.9% between the first and second half, p = 0.002), plus a −38% drop in Oct 2024 (58.1% → 36.0%) that could be the start of a cliff and needs watching. Import usage, **Ceiling**: after a Jan–Mar 2024 dip (~31%), it plateaued at 41–45% from Jul to Oct 2024, so more than half of users never import. Session duration, **Cliff (Jul 2024)**: steady at 11–14 min from Dec 2023 to Jun 2024, then a sharp drop to 7.0 min in Jul 2024 (−42%) that held (Jul–Oct average 7.3 vs 12.8 before). Sessions/user, **Ceiling (tentative)**: down to 3 in Jan 2024, back up to its earlier high of 8–9 from Jul to Oct 2024._

_Correlation test: **Leading 1 (data import, measured as Import Data %) vs trial-to-paid: no correlation**, r = −0.05 (p = 0.87), and r = −0.20 (p = 0.54) when import leads by one month. Leading 2's proxy (sessions per user) was also checked: r = 0.41 (p = 0.16), not significant. **Hypothesis revised:** the problem stays at the Revenue stage, but shifts from "trial users don't reach value" to "conversion has hit a ceiling that trial engagement hasn't moved". The leading indicators below are still the right ones to steer by, but they must be tested on user-level cohorts, not monthly totals._
_____

## Leading indicators

_What predicts the outcome, early and movable._

North Star (Aim): the number of trial users who import financial data and reach their first modeling output. Both leading indicators draw a line back to it through the set-up and the habit that come before the decision to pay.

- **Day-0 data-connection rate (share of new trial users who import or connect their business financial data in their first session):** It's the set-up step every North Star user must pass first, and the only behavior in FinWise's data that moves with repeat usage (sessions per user, r = 0.67). Lifting it should feed both the North Star and the trial-to-paid decision. It has hit a ceiling at 41–45%, so the experiment should be a new way in (e.g. one-click bank connection with a sample-data fallback), not a tweak.
- **Week-1 return rate (share of trial users who come back to check their cash forecast 3+ times in their first week):** A user who forms the weekly check-in habit during the premium period has something to lose at the downgrade, which is exactly what the reverse trial needs before the Revenue decision. It's the metric a weekly "cash clear" mechanic is designed to move. Visit frequency alone isn't enough (it rose while session length hit a cliff), so it should be measured as completed weekly checks, not raw sessions.



_____

## Lagging indicators

_The outcome metrics themselves._

- **Trial-to-paid conversion rate (baseline ≈ 2%: 128 of 6,424 trials over 13 months):** It's the Revenue-stage outcome where FinWise loses 98% of trials, and the ceiling to break. It can't be moved directly: it should rise only if more trial users connect their data, reach their own cash picture and return before the trial ends. That makes it the proof that the leading indicators were the right ones.
_____
