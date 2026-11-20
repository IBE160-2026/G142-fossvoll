---
title: "Addendum: RepRoute product brief (formerly Your Gym)"
created: 2026-10-18
updated: 2026-11-20
---

# Addendum: Your Gym

Detail that supports the brief but belongs in downstream documents (PRD, architecture, go-to-market).

## Pivot to RepRoute (2026-11-20)

- **Market research behind the pivot:** `.docs/planning-artifacts/research/market-gym-independent-workout-app-willingness-2026-11-19/research.md`. It covers prices, conversion benchmarks, competitors and the evidence on gamification.
- **Name ideas considered:** RepRoute (chosen as the working name), Liftpath, SetQuest, Finish Set, Gym Run and Repway.
- **Avatar style (for UX):** cozy, round and lovable. The feeling is inspired by Wii Miis and Club Penguin, but the design must be original.
- **Avatar mood rule (for the PRD):** the avatar's mood is evaluated per week against the user's own goal. It never changes body shape as a penalty. After a workout it shows extra strength temporarily, then returns to its base shape.
- **Goal setting (for the PRD):** the AI asks about the user's gym experience, suggests a sustainable weekly goal, and raises it after the user succeeds.
- **Machines (for the PRD):** there is a standard machine library, and the user picks a machine per exercise. The optional equipment checklist limits what the AI suggests to the machines the user has.
- **Premium:** one package containing AI-built workouts and cosmetics (avatar clothes, room designs). It is a mock-up in the school prototype.
- **Gamified competitors to know (from the research):** HeroFit (its avatar shrinks when goals are missed), Avatone, GymLevels, Quest2Fitness, Liftoff (free ranks and leaderboards), Fitness RPG (step-based map) and Ring Fit Adventure (console, about 10M sold).

The sections below come from the original white-label concept (2026-10-18). They are kept as background: the B2B parts no longer apply to version 1.

## Competitive landscape (desk research, 2026-10-18)

Most figures are vendor marketing or third-party estimates, so treat them as directional only.

### White-label member apps
- **PushPress:** branded app add-on at $81–97/mo. The gym also pays $99/yr for its own Apple developer account. Multi-location discounts are 20–50%. https://help.pushpress.com/en/articles/4339170-core-branded-app-pricing
- **Trainerize:** Studio Plus is about $248/mo per location, branded app included. https://costbench.com/software/gym-management/trainerize/
- **Virtuagym and Glofox:** pricing is behind a demo. Estimates run around $120–150/mo per location. https://coachway.io/articles/virtuagym-pricing/
- **EGYM (strongest threat):** a branded member app plus "Genius", which builds AI workouts from the gym's full equipment inventory. **EVO Fitness (Norway) runs its member app on EGYM.** https://egym.com/us/blog/egym-genius-operators , https://apps.apple.com/app/id6444803807
- **Technogym Mywellness:** a cloud platform and app linked to Technogym equipment.
- **Nordic players:**
  - The SATS app does booking, PT, stats, challenges and social features. SATS Group includes Fresh Fitness, with about 250 centres and 700k members (undated figure).
  - The 3T app is booking only.
  - BRP Systems (Sweden) is the Nordic gym software leader, with clients such as Nordic Wellness and Fitness24Seven. It was acquired by Nordic Capital in 2024.
  - Exerp (Denmark) also serves this market.

### Workout trackers members already use
- **Hevy:** claims 9–15M+ users and positions itself as social.
- **Fitbod:** about 15M downloads and around 300k paid subscribers (unverified). It generates AI workout plans.
- **Strong:** much smaller.
- None of them knows which gym the member is in.

### Gamification and per-machine tagging
- **Myzone:** gamifies heart-rate effort, with a vendor claim that members stay 24% longer.
- **QR codes on machines:** linking to demo videos is common and dates back to Gymcodes in 2012.
- **Gym-floor maps:** the only member-facing one found is BETA's map for climbing gyms. Mappedin offers generic indoor mapping.
- **No product found that combines a game-like gym map, per-machine exercises and logging.**

### Machine-usage analytics
- **Connected equipment:** Life Fitness Facility Connect, Matrix Facility 360 / Ecofit, EGYM and Technogym already report per-machine usage.
- **Sensors:** OnSight (radar, heat maps) and GYMetrix.
- **Gap:** free weights and older non-connected strength machines are mostly tracked by manual counts.

### AI form guidance
- **Camera form checkers:** Form Fix and FormLens use pose estimation. Peloton Guide's form feedback stayed in beta, and Tempo uses a 3D depth sensor.
- **Regulation:** consumer fitness AI is likely not high-risk under the EU AI Act unless it gives medical advice. The new EU Product Liability Directive makes it easier for injured users to claim against software. The gym's brand on bad advice adds risk for the gym.

### Retention
- **Benchmark:** the HFA 2025 benchmark puts average annual retention at 66.4%. https://uptivo.fit/blog/gym-member-retention-statistics
- **App claims:** retention claims for member apps are mostly untraceable vendor claims.
- **Drop-off:** most fitness-app users stop within weeks.

### Apparently open space
- A game-style map of the member's own gym as the main way to navigate.
- Logging that starts from a specific machine.
- Usage data for non-connected equipment, as a by-product of members logging.
- Data on how a session felt.
- An affordable option for independent and mid-size Nordic gyms that are not on EGYM or Technogym.
