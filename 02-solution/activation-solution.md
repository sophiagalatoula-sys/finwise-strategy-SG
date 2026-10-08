# The Solution · FinWise

> Module 2 · Acquisition & Activation. The onboarding solution and the Aha moment that makes value land.

## Aha moment

_The exact moment FinWise becomes "my money, finally clear."_

**A trial user connects their real business finances and sees their own cash-flow picture (current balance, what's coming in and going out, and cash runway in days) in their first session.** This is the moment FinWise stops being software they are evaluating and becomes "my money, finally clear".

- **The action:** connect business data *and* view their own cash-flow snapshot.
- **The timeframe:** within the first session (day 0) of the reverse trial.
- **The habit that should follow:** returning to check the cash forecast at least 3 times in week 1.

**What led me here.** Across 13 months of FinWise funnel data (Oct 2023 – Oct 2024), trial-to-paid conversion held at ~2% regardless of feature adoption. Modeling adoption rose from 10.78% to 58% with no change in conversion (r = 0.25, not significant), so "use more features" is not the lever. The one behavioral signal that moves with how often people come back is data import: in months when more trial users imported their data, sessions per user were higher (r = 0.67, p = 0.013). Import is the set-up step, and the Aha is the first payoff on the other side of it. It also fits the reverse trial: users can only feel the loss of premium value they have seen on *their own* numbers.

**Stated assumption.** The dataset is monthly aggregates with no user-level retention, so this is the best-supported hypothesis, not a proven predictor. Validating it means comparing 90-day retention of trial users who reach their cash snapshot on day 0 against those who don't.


_____

## Onboarding prototype

_Screenshots or a shareable link to the flow that gets users to the Aha faster._

**Link:** https://onboard-my-cash.lovable.app

Four screens, one job and one action each, from sign-up to the Aha moment (a reverse-trial badge, "Premium trial · 14 days left", and a step indicator run throughout):

| # | Screen | Job | One action |
|---|---|---|---|
| 1 | **What do you want to get clear on first?** | Personalize early with a single question: Cash flow / Unpaid invoices / Upcoming bills | Pick one |
| 2 | **Connect your money** | Set-up: get real data in, with read-only, bank-level security reassurance | One-click "Connect your bank" (fallback: "Try with sample data") |
| 3 | **Your money, finally clear** ← **Aha** | The user's own snapshot: balance, incoming vs outgoing, runway in days, recent activity, plus a highlighted card matching their screen-1 choice (e.g. "Your next 30 days look positive" or "€2,400 is due in 6 days") | "Set a cash alert" |
| 4 | **Bring in your accountant** | Start the collaboration loop *after* value has landed | Send invitation, or "Skip for now" |

The flow lands on the FinWise dashboard ("You're all set"). Bank connection and data are simulated with a realistic sample small business.

_____

## Why this activates

_The activation logic: what changes, and why it converts trial users._

**This works because** every screen moves the user toward one moment, seeing their own money clearly, and nothing else is asked of them first. **The friction I removed was manual data import:** it is replaced by a one-click bank connection with a sample-data fallback, so no trial user stalls at set-up before seeing value. **That matters because** set-up is the step that co-moves with repeat usage in FinWise's data, and repeat usage is the habit that leads to retention. Getting more users through set-up on day 0 means more users reach the value the reverse trial is betting they won't want to lose.

How the flow meets the benchmark for a strong Aha-moment flow:
- **One job per screen:** four screens, each with a single action.
- **Value before asks:** the accountant invite comes only after the user has seen their snapshot, and it is skippable.
- **Minimum viable set-up:** the only required step is connecting data, and even that has a sample-data escape hatch.
- **Personalize early:** one question on screen 1 decides which insight the Aha screen leads with.
- **Aha is unmistakable:** screen 3 is named for the moment ("Your money, finally clear") and shows the user's own numbers, not a product tour.

**How I'd measure it** (as an A/B test against the current onboarding):
- **Activation rate:** share of new trial users who reach screen 3 with their own data on day 0.
- **Time to Aha:** minutes from sign-up to first cash snapshot.
- **Drop-off rate by screen:** especially screen 2, the set-up step.
- **Post-onboarding retention:** week-1 return visits (the habit) and, ultimately, trial-to-paid conversion against the ~2% baseline.

_____
