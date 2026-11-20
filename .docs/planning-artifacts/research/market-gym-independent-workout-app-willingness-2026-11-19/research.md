---
title: 'market research: gym-independent workout app willingness to pay'
type: 'market'
topic: 'Will gym members pay for a gym-independent, gamified workout-path tracking app?'
decision: 'Go ahead with Your Gym as a gym-independent B2C app with the workout-path map; set personas, pricing and differentiation in the PRD'
source: 'native run (web search), 2 rounds'
status: complete
preset: 'standard'
validation: 'normal'
claims_verified: 5
claims_unverified: 7
claims_disputed: 1
created: '2026-11-19'
updated: '2026-11-19'
---

# Market research: gym-independent workout app willingness to pay

**Decision this research serves:** whether to build Your Gym as a gym-independent B2C app with the new "workout path" map, and whether members, especially beginners, will pay for it. The answer feeds the PRD's personas, pricing and differentiation.

**Concept tested:** the map is no longer the real gym's floor plan. It is a generic rectangular room with the machines laid out in workout order and a finish line at the end. The user's avatar walks from machine to machine in a bird's-eye game view, and the app works in any gym.

## Executive summary

**Answer: go ahead, but treat the game map as the hook, not the reason people pay.** Demand for strength training is real and growing. Willingness to pay for a tracking app is low and concentrated in a few winners. Your clearest advantage is that nobody has found a way to show one workout as a room you walk through. For a school project the product makes sense, but the business case is weak unless it converts better than typical fitness apps.

What drives this answer:

1. **Strength training is booming, especially among young people. Logging is a minority habit.**
   - US gym membership hit a record 81M in 2025, and Gen Z has the highest membership rate [9].
   - Gen Z is twice as likely as Gen X to call weight training their main sport [10].
   - In the Nordics, 59% of gym-goers prioritize strength training [12].
   - But in the only broad survey found, just 28% of frequent gym-goers tracked their training in an app, and about 40% tracked nothing [11]. That survey is from 2022.
   - Your hypothesis is half right. People care about their bodies, but no evidence was found that "progressive overload" content makes people log.
2. **Few people pay, and those who do pay little.**
   - Only about 3–4% of people who download a fitness app end up paying [5][6].
   - Loggers cost 235–325 kr a year in Norway (Hevy, Strong) [1][2]. AI-planned apps cost 879–1,190 kr a year (Fitbod) [3].
   - Human remote coaching costs about $1,800–2,400 a year [4].
   - A "digital PT" positioned above the logger tier has to show AI-plan value to justify Fitbod-level pricing.
3. **The workout-path map is new, but game features fade.**
   - Many apps put RPG skins, XP or ranks on gym logging: HeroFit, GymLevels, Quest2Fitness, and Liftoff with its free ranks and leaderboards [19][21].
   - None lays out one session as a path with an avatar walking between machines [19].
   - Studies show game features increase activity by a small-to-medium amount, but the effect largely disappears after the game ends [17][18].
   - People stay with trackers for speed, simplicity and visible progress [13]. The map must never slow down logging.

**Biggest caveat:** none of the gamification research covers strength training. Reddit was out of reach, and there is no Norway-specific evidence on willingness to pay. Treat the beginner-pays hypothesis as unproven until tested with real users.

## D1: Willingness to pay

**Prices (Norwegian App Store, live listings):**

| App | Model | Monthly | Yearly | Lifetime |
|---|---|---|---|---|
| Hevy Pro [1] | Logger, social | 35–49 kr | 275 kr | 899 kr |
| Strong PRO [2] | Logger | 49–55 kr | 235–325 kr | 999–1,290 kr |
| Fitbod Elite [3] | AI-planned workouts | 139–199 kr | 879–1,190 kr | none |
| Future [4] | Human remote coach | about $149–199 | — | — |

Several price variants per tier suggest the vendors are actively testing prices. Future's prices come from third-party reviews (one is a competitor's), so confidence is medium [4].

**Conversion benchmarks (Health & Fitness category):**
- **RevenueCat (2025 data):** median download-to-paid within 35 days is 2.9%, and the top quartile is above 6.2%. Trial-to-paid is 37.7%. The category has the highest early revenue per install of any category, $0.66 by day 60. A paying user is worth $35.64 after one year [5].
- **Adapty (2026):** install-to-trial 9.5%, trial-to-paid 42.2%, which gives about 4% install-to-paid. First renewal is 67.7%. Health & Fitness leads all categories in one-year lifetime value per install, at $1.21 [6]. Two independent publishers agree on the order of magnitude, so this is **verified**.
- **Median prices:** $9.99 a month and $39.94 a year [5].

**Traction:**
- Hevy claims "10M+ users" (the metric isn't defined) [1]. In 2023 it reported 1.5M users and about $2M expected annual revenue, bootstrapped [7]. This is dated.
- Strong claims 1.2M downloads [2].
- None of the apps discloses paid subscriber counts.
- Revenue is winner-take-most. About 5% of Health & Fitness apps reach $10k in total revenue within two years [8], and apps launched before 2020 hold 69% of revenue [8]. Confidence is medium, because this comes from secondary coverage of RevenueCat.

**Beginners specifically:** no study of what gym beginners would pay was found. This is an open question.

## D2: Does "progressive overload" drive tracking?

**For your hypothesis (people care more about their bodies):**
- **US gyms:** a record 81M members in 2025 (+5.2%), and Gen Z adults have the highest membership rate at 35.5%. Free weights have been the fastest-growing equipment category since 2021 [9].
- **Strava Year in Sport 2025:** Gen Z is twice as likely as Gen X to call weight training their main sport, and 61% more Gen Z than Gen X lift for looks [10]. Some coverage misreports this as "61% of Gen Z".
- **Strava has invested in strength:** over 500M strength uploads in 2025 and a new set/rep workout log [26]. Medium confidence: seen only as a snippet.
- **Nordics:** 59% of gym-goers prioritize strength training. 29% (Norway) name lack of motivation as a barrier, and in Denmark 17% "don't know where to start" [12]. That is exactly the beginner gap Your Gym targets.

**Against the second half (it makes people log sets and reps):**
- Only 28% of frequent gym-goers in the US and UK tracked fitness or diet in an app, and about 40% tracked nothing [11]. This is from 2022, older than the freshness bar, so confidence is medium.
- App reviewers do name progressive overload as a reason to log ("it's perfect for tracking progressive overload") [13]. This shows the motive among people who already log, not how common it is.
- No evidence was found that influencer content changes logging behavior. Absence of evidence is reported as a finding.

## D3: Why people quit tracking apps

- **Retention is structurally poor.** Health & Fitness apps keep about 3–4% of users at day 30 [16]. Low confidence: vendor blogs that may recycle the same base data.
- **Complaints, from Strong's 50 latest App Store reviews, 14 of them rated 1–3 stars [13]:**
  - customization limits (5)
  - lost data or Watch sync (3)
  - paywalls (2)
  - device support (2)
- **Complaints in adjacent fitness apps (not strength trackers):** billing and paywalls lead [15].
- **Why people stay:**
  - **Strong's 5-star reviews** praise "as few presses as possible", reliability, and seeing progress [13].
  - **Hevy's reviews** praise motivation features, such as "makes working out like a video game", a streak calendar, and light social features [14]. Hevy's reviews arrived within about two days, which suggests the app prompts for them, so they skew positive.
- **Split on games:** one Strong reviewer praised "no stupid AI or leaderboards" [13]. There is an audience that likes a light game layer, and a vocal one that rejects pushy mechanics.

## D4: Workout-path competitors and the business model

**Nobody found has the concept (confirmed in two independent search rounds):**
- **Gym loggers with an RPG skin:** HeroFit, GymLevels, Avatone, Quest2Fitness and RPGFitness use XP, avatars or battles, but no spatial layout of the session [19].
- **Ranked tracking:** Liftoff is a large free tracker with strength ranks, streaks and leaderboards, and an optional Pro tier ($9.99–79.99 in-app purchases). Its rating count is disputed: about 63k–103k US ratings [21]. It is the most relevant gamified competitor for young lifters.
- **Map metaphors in other kinds of fitness apps:** Fitness RPG ("Fitland map") is step-based [25]. Ring Fit Adventure is a console game where your exercise moves the avatar through levels, and it has sold about 10M units [20]. That proves "workout as a level" can sell at scale, but at home, not in the gym.

**Does gamification work?**
- A meta-analysis of 16 trials found a small-to-medium effect on physical activity (g = 0.42, about +1,600 steps a day). By follow-up the effect had shrunk to g = 0.15 [17].
- The BE FIT trial saw activity fall after the game ended, but it stayed above the control group [18].
- All of this is about steps, not strength training.

**B2C vs. B2B:**
- **B2C (sell directly to users):**
  - The category has the best lifetime value per install [6], but revenue goes to a few winners [8].
  - Paid installs cost about $11–20 on Facebook [24], against a one-year lifetime value of about $1.2 per install [6]. Paid ads lose money unless conversion is far above the median. Growth would have to come from organic and social sharing.
- **B2B white-label (sell to gyms):**
  - Incumbents charge gyms about $80–250 a month per location: PushPress from $81 [23], Trainerize Studio Plus at $248 [22]. The app is usually bundled with booking and billing.
  - A standalone module would compete for a place in those bundles.
- **What the pivot changes:**
  - It removes per-gym map work and makes B2C possible.
  - It also removes the "your own gym" differentiation from the old brief, so the gym is no longer the natural customer.
  - A hybrid remains open, for example a free B2C app plus gym partnerships. No evidence was gathered on how well hybrids work.

## Cross-dimension insights

- **The demand is beginners, but the payers are lifters who already log.** D2 shows growth and a beginner barrier ("don't know where to start", lack of motivation) [12]. D1 and D3 show that the people who pay value speed and simple progress tracking [13]. Your Gym's map serves beginners. Beginners are the group least proven to pay.
- **The map must also make logging faster.** Your brainstorming idea fits the evidence: if machines are laid out in workout order, "next machine" becomes one tap, which supports what makes users stay [13]. If the map ever adds a step to logging, it hits the main reason people churn.
- **The pivot shifts competition.** Before, Your Gym competed with EGYM and white-label vendors for gym budgets. Now it competes with free trackers like Hevy, Strong and Liftoff for the user's attention, where the price ceiling is about 275 kr a year [1].

## Recommendations

1. **Brief update:** record the pivot (generic room in workout order, gym-independent, B2C first) and drop "the gym licenses it" as the main model. Basis: D4 business-model findings. Medium confidence.
2. **PRD personas:** make the beginner who "doesn't know where to start" the primary persona [12], and the progressive-overload logger secondary. Basis: D2. Medium confidence, partly from an operator survey.
3. **PRD requirement:** logging a set must take a few seconds, the map can never block input, and progress charts are core. Basis: D3 review evidence. Medium confidence: one app sample.
4. **PRD pricing:** freemium. Core logging should be free to compete with Hevy, Strong and Liftoff. Charge for AI-built workouts at a level between Hevy (275 kr/yr) and Fitbod (879 kr/yr). Basis: D1 prices, high confidence. The conversion assumption (about 3–4%) is verified.
5. **Keep the game light:** streaks, progress and the finish-line moment, without forced leaderboards. Basis: D3 split sentiment and D4 effects that fade. Medium to low confidence.
6. **Success metric:** measure retention after day 30 against the benchmark of about 3–4% [16]. Low-confidence benchmark, but an obvious test.

## Open questions

- **Do beginners pay?** No study was found. Answer it by testing a prototype with 5–10 beginner gym-goers and asking about price (Van Westendorp questions).
- **Norwegian data:** the total gym member count and app use in Norway. Virke's full report and SATS's full report are the places to look.
- **Reddit user voice:** blocked for the tools. A manual read of r/fitness and r/beginnerfitness threads on "how do you track" would fill this gap.
- **Does gamification work for strength training specifically?** No randomized trial found.
- **Liftoff's real traction and Pro price:** the sources conflict.
- **Do hybrid models work (B2C app plus gym partnerships)?** Not researched.

## Source appendix

| # | Supports | Publisher | Pub date | Accessed | Confidence |
|---|---|---|---|---|---|
| [1] | Hevy NO prices, 10M+ user claim | [Apple App Store (Hevy)](https://apps.apple.com/no/app/id1458862350) | live listing | 2026-11-19 | high (prices), medium (user claim) |
| [2] | Strong NO prices, 1.2M downloads | [Apple App Store (Strong)](https://apps.apple.com/no/app/id464254577) | live listing | 2026-11-19 | high |
| [3] | Fitbod NO prices | [Apple App Store (Fitbod)](https://apps.apple.com/no/app/id1041517543) | live listing | 2026-11-19 | high |
| [4] | Future coaching price | [SensAI](https://www.sensai.fit/blog/future-app-review-2026), [Garage Gym Reviews](https://www.garagegymreviews.com/future-app-review) | 2026-09 | 2026-11-19 | medium |
| [5] | H&F conversion, prices, revenue per install | [RevenueCat State of Subscription Apps 2026](https://www.revenuecat.com/state-of-subscription-apps-2026/) | 2026-03 | 2026-11-19 | high |
| [6] | H&F funnel, LTV per install | [Adapty](https://adapty.io/blog/health-fitness-app-subscription-benchmarks/) | 2026 | 2026-11-19 | medium-high |
| [7] | Hevy 2023 users and revenue | [Ottawa Business Journal](https://obj.ca/fitness-app-entrepreneur-pumped-by-hevys-progress-to-2m-in-annual-revenue) | 2023-03 | 2026-11-19 | medium (dated) |
| [8] | Winner-take-most revenue | [Athletech News](https://athletechnews.com/fitness-apps-monetizable-winner-take-all-or-most/), [ContentGrip](https://www.contentgrip.com/subscription-app-market-2026-growth/) (both recycle RevenueCat) | 2025/2026 | 2026-11-19 | medium |
| [9] | US gym membership, Gen Z, free weights | [Health & Fitness Association](https://www.healthandfitness.org/?p=5212) | 2026-04 | 2026-11-19 | high |
| [10] | Gen Z weight training | [Strava press](https://press.strava.com/articles/strava-releases-12th-annual-year-in-sport-trend-report-2025) | 2025-12 | 2026-11-19 | medium-high |
| [11] | 28% track in apps, ~40% track nothing | [YouGov](https://business.yougov.com/content/43857-us-britain-tools-gym-goers-use-track-fitness) | 2022 | 2026-11-19 | medium (dated) |
| [12] | Nordic strength priority and barriers | [SATS Healthier & Happier Report 2025](https://sats.no/the-healthier-and-happier-report-2025) | 2025 | 2026-11-19 | medium |
| [13] | Strong review themes | [Apple App Store review feed (Strong)](https://itunes.apple.com/us/rss/customerreviews/id=464254577/sortBy=mostRecent/json) | 2026-08 to 2026-11 | 2026-11-19 | medium |
| [14] | Hevy review themes | [Apple App Store review feed (Hevy)](https://itunes.apple.com/us/rss/customerreviews/id=1458862350/sortBy=mostRecent/json) | 2026-11 | 2026-11-19 | low-medium |
| [15] | Paywall and billing complaints, adjacent apps | [Unstar](https://unstar.app/de/research) | 2026-09 | 2026-11-19 | medium-low |
| [16] | Day-30 retention about 3–4% | [UXCam](https://uxcam.com/blog/mobile-app-retention-benchmarks/), [Business of Apps](https://www.businessofapps.com/?p=98298) | 2023–2026 | 2026-11-19 | low-medium |
| [17] | Gamification meta-analysis | [JMIR, Mazeas et al.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8767479/) | 2022-01 | 2026-11-19 | high |
| [18] | BE FIT trial | [Penn CHIBE](https://chibe.upenn.edu/publications/effect-of-a-game-based-intervention-designed-to-enhance-social-incentives-to-increase-physical-activity-among-families-the-be-fit-randomized-clinical-trial) | 2017-10 | 2026-11-19 | high |
| [19] | Gamified strength apps, none spatial | [HeroFit](https://apps.apple.com/us/app/id6446021260), [Quest2Fitness](https://apps.apple.com/app/id6769663664), [GymLevels](https://screensdesign.com/showcase/gymlevels-ranked-gym-workouts), [Avatone](https://www.producthunt.com/products/avatone) | undated | 2026-11-19 | medium |
| [20] | Ring Fit about 10M units | [Shacknews](https://shacknews.com/article/124238/ring-fit-adventure-has-sold-10-million-copies-since-launch) | 2021 | 2026-11-19 | medium |
| [21] | Liftoff model, prices, ratings | [Apple App Store (Liftoff)](https://apps.apple.com/us/app/-/id6448081563), [AppPricingLab](https://apppricinglab.com/iap/apple/6448081563) | 2026 | 2026-11-19 | medium (disputed ratings) |
| [22] | Trainerize white-label pricing | [Trainerize](https://www.trainerize.com/pricing/) | live page | 2026-11-19 | medium |
| [23] | PushPress member app pricing | [PushPress](https://pushpress.com/feature-list/member-app) | live page | 2026-11-19 | medium |
| [24] | Facebook cost per install, fitness | [Superads](https://www.superads.ai/facebook-ads-costs/cost-per-app-install/fitness-training-centers/united-states) | 2025 | 2026-11-19 | low-medium |
| [25] | Fitness RPG step map | [Apple App Store (Fitness RPG)](https://apps.apple.com/app/id1252580641) | undated | 2026-11-19 | medium |
| [26] | Strava strength uploads and log | [Strava press](https://press.strava.com/articles/strava-overhauls-strength-experience-with-expanded-partner-ecosystem-new-workout-log-and-muscle-maps) | 2026 (unverified) | 2026-11-19 | medium |

## Staleness map

Computed with `recon_kit.py staleness`. Freshness windows: pricing 3 months, GTM 12, size 18, sentiment 18, behavior 24.

| Claim | Class | Published | Re-check by | Status |
|---|---|---|---|---|
| [11] Share of gym-goers tracking in apps | behavior | 2022-01 | 2024-01 | **stale already** |
| [24] Facebook fitness cost per install | gtm | 2025-06 | 2026-06 | **stale already** |
| [12] Nordic strength priority and barriers | behavior | 2025-01 | 2027-01 | fresh |
| [1] Hevy/Strong/Fitbod NO prices | pricing | 2026-11 | 2027-02 | fresh |
| [21] Liftoff pricing and ratings | pricing | 2026-11 | 2027-02 | fresh |
| [22][23] White-label gym app pricing | pricing | 2026-11 | 2027-02 | fresh |
| [19] No spatial-path competitor | competitor | 2026-11 | 2027-02 | fresh |
| [5][6] H&F conversion benchmarks | gtm | 2026-03 | 2027-03 | fresh |
| [9] US gym membership and Gen Z | size | 2026-04 | 2027-10 | fresh |
| [13] Tracker review sentiment | sentiment | 2026-11 | 2028-05 | fresh |

Earliest re-check: two claims are already past their window ([11] and [24]). They are kept because no fresher source was found, and they are marked as dated in the text. The next ones expire on **2027-02-01** (prices and the competitor scan).
