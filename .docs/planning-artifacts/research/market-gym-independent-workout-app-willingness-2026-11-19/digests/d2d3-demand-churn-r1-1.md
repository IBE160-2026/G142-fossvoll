# Digest D2/D3: demand and churn (run r1-1)

Hypothesis tested: "People care more about their bodies than ever. Fitness influencers push 'progressive overload' everywhere, so tracking sets and reps matters to people."

Tags: **[FOR]** supports the hypothesis, **[AGAINST]** goes against it, **[NEUTRAL]** is context.

Access constraints this run: Reddit was blocked to the search and fetch tools, so no Reddit threads were mined. The apps.apple.com review pages returned HTTP 429. App Store reviews came from Apple's public RSS review feed instead.

## Findings

### D2: Demand and participation

- **[FOR]** US fitness-facility membership hit a record 81M in 2025, up 5.2% from 2024. Gen Z adults (18–24) had the highest penetration of any age group at 35.5%. | https://www.healthandfitness.org/?p=5212 | Health & Fitness Association (HFA), 2026 U.S. Health & Fitness Consumer Report release | 2026-04 | accessed 2026-11-19 | confidence high (primary industry body, US only) | participation
- **[FOR]** HFA says free-weight use (dumbbells, barbells, kettlebells) has grown faster than any other equipment category since 2021. The release gives no number for it. | https://www.healthandfitness.org/?p=5212 | HFA | 2026-04 | accessed 2026-11-19 | confidence medium (qualitative claim, no figure) | participation
- **[FOR]** Strava Year in Sport 2025: Gen Z is "2x more likely than Gen X to say weight training is their primary sport", with "61% more Gen Z than Gen X saying they lift for aesthetics". Women were "21% more likely than men to record Weight Training". The survey covered more than 30,000 users and non-users. Note that some secondary coverage misreports the aesthetics figure as "61% of Gen Z". | https://press.strava.com/articles/strava-releases-12th-annual-year-in-sport-trend-report-2025 | Strava (press release) | 2025-12 | accessed 2026-11-19 | confidence medium-high (primary, but Strava's own user base and vendor survey; the baseline is undefined) | participation / behavior
- **[FOR]** Strava says strength is "one of the fastest-growing sport types on Strava", with "over 500 million uploads in 2025 alone". It has since added a dedicated strength workout log and muscle maps. A large general fitness platform is investing in set/rep logging. | https://press.strava.com/articles/strava-overhauls-strength-experience-with-expanded-partner-ecosystem-new-workout-log-and-muscle-maps | Strava (press release) | undated (2026 per context; not verified) | accessed 2026-11-19 | confidence medium (seen only as a search snippet; page not fetched) | behavior
- **[FOR]** Garmin reportedly saw strength sessions up 29% in 2025. | https://www.t3.com/active/garmin-strava-end-of-year-report-2025 | T3 (secondary, citing Garmin Connect data) | 2025-12 | accessed 2026-11-19 | confidence low-medium (secondary; Garmin primary not fetched) | behavior
- **[AGAINST]** In a YouGov survey of frequent gym-goers in the US and GB, only 28% tracked fitness or diet through fitness apps. "Don't track at all" was the largest group, at about two in five. This is the most direct evidence that most gym-goers do not log in an app. | https://business.yougov.com/content/43857-us-britain-tools-gym-goers-use-track-fitness | YouGov | 2022 (DATED, more than 2 years old) | accessed 2026-11-19 | confidence medium (reputable pollster but stale; mixes fitness and diet apps; seen via search summary) | behavior
- **[AGAINST / NEUTRAL]** FitTech Global reported that 27% of gym members track their physical activity, most often with a phone app. | https://www.fittechglobal.com/fit-tech-features/Activity-tracking-Tracking-vs-retention/31159 | FitTech Global | undated (likely dated) | accessed 2026-11-19 | confidence low (secondary, date unknown) | behavior
- **[NEUTRAL]** Some App Store reviewers explicitly name progressive overload and replacing the notebook as their reasons for using a tracker. Strong: "it's perfect for tracking progressive overload"; "This app replaces the notebook, and will save time in the gym". Hevy: "Tracking weights can be tedious, but Hevy makes it simple". This shows the motivation exists among people who already log. It says nothing about how common it is in the wider population. | https://itunes.apple.com/us/rss/customerreviews/id=464254577/sortBy=mostRecent/json ; https://itunes.apple.com/us/rss/customerreviews/id=1458862350/sortBy=mostRecent/json | Apple App Store (Strong, Hevy reviews) | 2026-08 to 2026-11 | accessed 2026-11-19 | confidence low for prevalence, medium as motive evidence | sentiment

### D3: Churn and why people stay

- **[NEUTRAL, churn drivers]** Strong, 50 most recent US App Store reviews (2026-08-20 to 2026-11-17): 14 rated 1–3 stars. The recurring themes among those 14 were:
  - Exercise library and customization limits: 5 ("Can't put your own machines in detail"; "Wish the app had a way to build rep ranges into templates").
  - Apple Watch sync and lost data: 3 ("my workout history has disappeared"; "Sets disappear from history").
  - Paywall or price: 2 ("Can't do anything unless u pay"; "pro pricing just doesn't make sense").
  - Device support (iPad, foldable): 2.
  - Stagnation: 1 ("This app hasn't really changed in 5+ years").

  | https://itunes.apple.com/us/rss/customerreviews/id=464254577/sortBy=mostRecent/json | Apple App Store | 2026-08 to 2026-11 | accessed 2026-11-19 | confidence medium (one app, one store, small sample; distinct reviewers) | sentiment
- **[NEUTRAL, stay drivers]** Strong 5-star reviews (25 of 50) cluster on four themes:
  - Simplicity and few taps: about 8 ("does exactly what I need it to with as few presses as possible").
  - Reliability and no money grab: about 6 ("most free apps gradually get worse and more aggressively demand cash over time").
  - Seeing progress: about 4.
  - Customization: about 4.

  **[AGAINST a game layer]** One 5-star reviewer praised "no stupid AI or leaderboards being crammed down your throat". | same source | Apple App Store | 2026-08 to 2026-11 | accessed 2026-11-19 | confidence medium | sentiment
- **[FOR a game or social layer]** Hevy, 50 most recent reviews: 41 are 5-star. Praise themes:
  - Ease of use: about 12.
  - Progress data and graphs: about 12.
  - Motivation: about 7 ("Makes working out like a video game"; "it gives positive feedback on accomplishments"; "the calendar that shows everyday that you've worked out with blue squares").
  - Light social features: about 5 ("I love the light social feature and the process graphs!").

  The 4 complaints were foldable iPhone support (2), a paywall after 7 custom exercises (1) and gaps in the exercise library (1). **Caveat:** all 50 reviews fall within about 2 days, which suggests in-app review prompts after a positive moment. They are a skewed sample and say little about churners. | https://itunes.apple.com/us/rss/customerreviews/id=1458862350/sortBy=mostRecent/json | Apple App Store | 2026-11 | accessed 2026-11-19 | confidence low-medium (selection bias) | sentiment
- **[NEUTRAL, churn driver: paywalls and billing]** Unstar profiled 1–3 star reviews (US, iOS and Android, Aug–Sep 2026) for 20 adjacent health and fitness apps: step counters, calorie trackers, running and period apps. None are strength trackers. Share of apps where each theme ranked as a top complaint:
  - Billing and refunds: 45%.
  - Paywall and pricing: 40%.
  - Ads: 30%.
  - Bugs: 25%.
  - Data accuracy: 20%.
  - Sync and data loss: 10%.

  | https://unstar.app/de/research | Unstar.app (review-mining tool) | 2026-09 | accessed 2026-11-19 | confidence medium-low (rule-based classifier; adjacent category; the unit is apps, not reviewers) | sentiment
- **[NEUTRAL]** Hevy review aggregators (Marlvel, Justuseapp) name Pro subscription gating as the top complaint and the logging interface as the top praise. Hevy's listed prices are $2.99 a month, $23.99 a year and $74.99 lifetime. | https://adapty.io/paywall-library/hevy/ ; https://marlvel.ai/api/llm/apps/health-fitness/com-hevyapp-hevy | Adapty; Marlvel (AI aggregator) | undated | accessed 2026-11-19 | confidence low (aggregators, seen via search summary only) | sentiment
- **[NEUTRAL]** Third-party blogs that summarise Reddit say people abandon a tracker when logging a set takes "more than a few seconds". They also cite fear of acquisition or repricing, dislike of streak and achievement notification spam, and a wish for data export. These blogs come from a competitor (Setgraph) with a commercial interest, and the claims could not be checked against Reddit this run. | https://setgraph.app/ai-blog/best-workout-tracker-app-reddit | Setgraph (competitor blog) | 2025 | accessed 2026-11-19 | confidence low | sentiment

### D3: Retention benchmarks

- **[AGAINST easy retention]** Health and fitness apps reportedly had about 3% day-30 retention in 2023. | https://www.businessofapps.com/?p=98298 | Business of Apps (aggregator; underlying source not verified) | 2023 data (behavior, at the edge of 2 years: treat as dated) | accessed 2026-11-19 | confidence low-medium | retention-benchmark
- **[AGAINST easy retention]** UXCam's per-category data gives Health & Fitness 3.7% day-30 retention. Phiture puts the 2025–26 cross-industry averages at about 25–26% on day 1, 11–13% on day 7 and 5–7% on day 30. AppsFlyer data cited by Getstream gives a day-30 average of 3.7% on iOS and 2.1% on Android across all categories (Q3 2024). | https://uxcam.com/blog/mobile-app-retention-benchmarks/ ; https://phiture.com/mobilegrowthstack/managing-retention-rate-benchmarks-and-expectations/ ; https://getstream.io/blog/app-retention-guide | UXCam; Phiture; Getstream (vendor blogs) | 2025–2026 | accessed 2026-11-19 | confidence low-medium (vendor blogs; numbers broadly agree, but they may recycle the same AppsFlyer/Adjust base data; definitions differ) | retention-benchmark
- **[UNVERIFIED]** A frequently repeated claim says "71% of users stop using health apps within 90 days", attributed to a JMIR systematic review. Only a blog citation was found, so this is not evidenced. | https://setgraph.app/ai-blog/best-workout-apps-free-reddit | secondary blog | undated | accessed 2026-11-19 | confidence low | retention-benchmark

## Net reading on the hypothesis

- **Part 1 is supported.** Interest in strength training is growing, especially among Gen Z: HFA records, Strava, Garmin.
- **Part 2 is weakly supported at most.** The claim that influencer "progressive overload" content makes people log sets and reps rests on a handful of individual reviewer statements. Primary survey data (YouGov 2022, dated) shows that a minority of gym-goers use apps and roughly 40% track nothing.
- **Hard evidence linking influencer content to logging behavior was not found.**
- **Retention is structurally poor.** Day 30 is around 3–4% for the category.
- **What drives churn:** stated complaints centre on paywalls and billing, lost data and sync, and limits on customization.
- **What drives retention:** people stay for speed, simplicity, reliability and visible progress.
- **On the game layer:** some users enjoy light gamification and social features ("like a video game", streak calendar). A vocal segment rejects leaderboards and pushy streak mechanics.

## Leads worth chasing

- **HFA full report PDF:** age breakdown of strength or free-weight use; global edition; whether app use among members is measured.
- **Strava Year in Sport 2025 full report:** strength share of uploads by age; date and details of the strength-log launch.
- **Garmin Connect Data Report 2025 (primary):** the 29% strength figure.
- **Norwegian and Nordic data:** Virke Trening / Treningsrapporten, SSB idrett og friluftsliv statistics, Norsk Treningssenterforbund. Not searched this run.
- **Google Trends for "progressive overload" (2019–2026):** pull directly. No credible commentary was found.
- **Reddit:** r/fitness, r/GYM, r/beginnerfitness threads on "how do you track" and why people quit apps. Needs a tool or route that can access Reddit, or a manual pass. r/fitness has historically run Daily Simple Questions threads that discuss app vs. notebook vs. spreadsheet.
- **Fitbod and JEFIT reviews:** RSS feeds (`itunes.apple.com/us/rss/customerreviews/id=1041517543/...` for Fitbod). Not fetched due to budget. Fitbod has a subscription-only model, which likely concentrates paywall complaints.
- **Primary retention reports:** AppsFlyer and Adjust category benchmarks, and the RevenueCat State of Subscription Apps (Health & Fitness trial conversion and annual retention).
- **The JMIR systematic review on health-app abandonment:** locate the actual paper.

## Looked for but not found

- **Reddit user voice:** Reddit was blocked to the search and fetch tools.
- **Evidence linking "progressive overload" search or social interest to set/rep logging:** no Google Trends analysis, no survey.
- **A recent (2024–2026) survey on the share of gym-goers who log workouts and with which method (app, notebook, spreadsheet):** only YouGov 2022.
- **Norwegian or Nordic participation data:** not searched within budget.
- **Primary-source fitness-app day-90 retention:** only vendor-blog day-30 figures found.
- **Fitbod and JEFIT review samples:** App Store pages rate-limited; budget spent.
