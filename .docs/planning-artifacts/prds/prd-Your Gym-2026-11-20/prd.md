---
title: "PRD: RepRoute"
status: final
created: 2026-11-20
updated: 2026-11-21
---

# PRD: RepRoute
*Working title (formerly "Your Gym"). Name availability in the app stores and as a trademark has not been checked.*

## 0. Document Purpose

This PRD defines what RepRoute must do for the IBE160 school prototype, written so the product can be launched later without a rewrite. It builds on the product brief (`.docs/planning-artifacts/briefs/brief-Your Gym-2026-10-18/brief.md`) and the market research in `.docs/planning-artifacts/research/`; it does not repeat their reasoning. Where this PRD differs from the brief, this PRD wins (see Open Questions). Terms in §3 are used exactly throughout. Requirements are grouped by feature with globally numbered FRs. Inferred details carry `[ASSUMPTION]` tags and are indexed in §9.

## 1. Vision

RepRoute turns a gym workout into a short game level. Each workout is a **Gym Map**: the machines laid out in the order of the workout, with a finish line at the end. The user's **Avatar** walks from machine to machine. At each machine the user logs sets in a few taps, then moves on. Crossing the finish line ends the session with an animation, a few questions about how it went, XP and a stronger Avatar.

It is built for beginners and for people who have never used a workout tracker. The user creates an Avatar, sets a goal, and RepRoute offers workout splits that fit that goal and the user's real life. Between workouts the Avatar lives on the **Dashboard**, happy when the user is on track, gently sad after a missed week. The point is a reason to come back that feels good, not like homework.

The game feel is what makes RepRoute different, and it must never get in the way of fast logging.

## 2. Target User

### 2.1 Jobs To Be Done
- When I'm new to the gym and don't know where to start, I want a plan that fits my goal and my life, so I can walk in knowing what to do.
- When I'm at a machine, I want to log my set in seconds, so tracking doesn't interrupt my workout.
- When I've never kept a training log, I want tracking to feel fun, so I actually keep doing it.
- When life gets busy, I want the app to be forgiving and help me restart, so one bad week doesn't end my progress.

### 2.2 Non-Users (v1)
Experienced lifters who are happy with Hevy or Strong. When needs conflict, beginners decide.

### 2.3 Key User Journeys

- **UJ-1. John's first session.**
  - **Persona + context:** John, 18, new to the gym, no tracker experience.
  - **Entry state:** First launch, no account.
  - **Path:** John creates an account → meets his Avatar and chooses gender, body colour, hairstyle and facial features → sets his experience level, Objective, focus body parts and workouts per week, and ticks off the equipment his gym has → the Avatar asks reality-check questions (job, busy weekends, kids, school) → the Avatar "thinks" and presents several Split options → John picks one and can add or remove exercises → he starts a workout and his Avatar stands at the first machine → he logs a set (reps, kg, effort) and the Avatar plays a small animation → he drags the Avatar to the next machine, in any order, skipping where needed.
  - **Climax:** John walks the Avatar across the finish line and the Avatar plays a finish animation.
  - **Resolution:** The Avatar asks a few questions about how the workout felt. John earns XP and returns to the Dashboard.
  - **Edge case:** A machine is taken. John goes to a different machine first, or skips one, and the workout still finishes.

- **UJ-2. John comes back.**
  - **Persona + context:** John, week 2 or 3, has used the app a few times.
  - **Entry state:** Logged in, opens the app.
  - **Path:** John lands on the Dashboard and sees his Avatar with its level and XP bar, his Weekly Goal status and "Start a workout".
  - **Climax:** If he has logged workouts, the Avatar is happy and says something encouraging. If he missed a whole week, the Avatar is a little sad and says something to get him back on track.
  - **Resolution:** John taps "Start a workout" and continues into UJ-1 from the Gym Map.
  - **Edge case:** Life changes (new job, exams). John updates his goals and asks the Avatar for a new plan.

Building a workout by hand (FR-10) and logging without signal in the gym (FR-21) are covered as requirements, not separate journeys.

## 3. Glossary

- **User** — A person with a RepRoute account.
- **Avatar** — The User's cozy, round character, customised at sign-up. Walks the Gym Map, reacts to logged sets, shows mood on the Dashboard. One per User.
- **Objective** — What the User wants to achieve: stronger, lose weight, or build muscle.
- **Weekly Goal** — The number of workouts per week the User aims for.
- **Reality Check** — The Avatar's questions about the User's real life (job, busy weekends, kids, school) used to judge whether the Weekly Goal is realistic.
- **Split** — A weekly plan of workouts (for example push/pull/legs or full body) built from a fixed template and adapted to Objective, focus body parts, Weekly Goal and equipment.
- **Workout** — A named list of exercises in order, either from a Split or built by the User.
- **Exercise** — One movement in the exercise library. Each Exercise on the Gym Map is represented by a Machine Station.
- **Equipment** — The machines a User's gym has, ticked off by the User. Limits which Exercises are offered.
- **Week** — Monday to Sunday. `[ASSUMPTION]`
- **Gym Map** — The top-down room generated from a Workout, showing Machine Stations in workout order and a finish line.
- **Machine Station** — The placeholder for one Exercise on the Gym Map. Shows the Exercise name.
- **Set** — One logged round of an Exercise: reps, weight in kg and an effort rating.
- **Effort** — How hard a Set felt, rated on a 1–10 scale or as RPE (reps in reserve). The User chooses which.
- **How-To** — A short animation showing correct form for an Exercise, opened from a "?" at the Machine Station. Only some Exercises have one.
- **Session** — One played-through Workout, from start to crossing the finish line.
- **XP / Level** — Points earned by completing Sessions and the Level they add up to. Free.
- **Dashboard** — The home screen: Avatar with Level and XP bar, Weekly Goal status, "Start a workout", progress.
- **Mood** — The Avatar's happy or sad state, driven by whether the User trained during the week.

## 4. Features

### 4.1 Account and Onboarding
**Description:** A new User signs up and is led straight into creating an Avatar and setting goals. Realizes UJ-1.

**Functional Requirements:**

#### FR-1: Create an account
A visitor can create an account and sign in. `[ASSUMPTION: email and password, plus optional Google/Apple sign-in; final method decided in architecture.]`

**Consequences (testable):**
- A User can sign in again on another device and see the same Avatar and history.
- Onboarding resumes where it stopped if the User leaves midway.

#### FR-2: Update goals later
A User can change experience level, Objective, focus body parts, Weekly Goal and equipment at any time, and ask the Avatar for a new plan. Realizes UJ-2.

**Consequences (testable):**
- Changing goals does not delete logged history.
- A new plan is offered as new Split options; the current Split stays until the User picks one.

### 4.2 Avatar
**Description:** The User builds a personal Avatar with a few tweaks. It is the User's companion on the Gym Map and the Dashboard.

#### FR-3: Create and customise the Avatar
A User can choose gender, body colour, hairstyle and facial features for the Avatar.

**Consequences (testable):**
- The chosen look appears identically on the Dashboard and the Gym Map.
- The User can change the look later.

The look must be original, cozy, round and lovable, and not copied from existing characters.

**Out of Scope:** Clothes and other cosmetics (Premium, after launch).

#### FR-4: Avatar reacts to logged Sets
The Avatar plays a short animation each time a Set is logged and a longer one at the finish line.

**Consequences (testable):**
- The animation never delays or blocks the next tap (see NFR-1).
- After a Session the Avatar shows a temporary strength effect on the finish screen. On the Dashboard its base shape is unchanged, and no Mood or Session result ever changes the body shape as punishment.

### 4.3 Goals and Reality Check
**Description:** The User states what they want. The Avatar then checks it against their real life, so the plan is something they can keep. Realizes UJ-1.

#### FR-5: Set goals
A User can set experience level, Objective, focus body parts and Weekly Goal.

**Consequences (testable):**
- All four inputs are required before Split options are shown.

#### FR-6: Reality Check
The Avatar asks the User about job, busy weekends, kids and school, and uses the answers to confirm or adjust the Weekly Goal.

**Consequences (testable):**
- If the answers conflict with the Weekly Goal, the Avatar suggests a lower number and the User can accept or keep their own.
- Avatar messages come from a reviewed set of supportive texts, and none blames the User.

### 4.4 Equipment
#### FR-7: Tick off available equipment
A User can optionally tick off the machines their gym has.

**Consequences (testable):**
- If the User ticks equipment, Split options only use Exercises that can be done with it.
- If skipped, Split options use the full Exercise library.

### 4.5 Workout Builder and Split Options
**Description:** The User gets several Split options built from fixed templates and adapted to their goals, or builds a Workout from scratch. Realizes UJ-1, UJ-2.

#### FR-8: Offer several Split options
After onboarding, the Avatar presents several Split options for the User to choose between. `[ASSUMPTION: 2–3 options.]`

**Consequences (testable):**
- Every option is built from a fixed template and respects Objective, focus body parts, Weekly Goal and equipment.
- The Avatar shows a short "thinking" state before the options appear.
- Split options are always produced, with or without a connection: templates are chosen by rules `[ASSUMPTION]`, and AI is an optional layer for the Reality Check and personalised wording that needs a connection. The exact AI role is decided in architecture.

#### FR-9: Edit a Split
A User can add, remove and reorder Exercises in any Workout of a chosen Split.

#### FR-10: Build a Workout by hand
A User can build their own Workout from the Exercise library, without AI help.

**Consequences (testable):**
- The library is searchable and filterable by body part.
- For an Exercise the User can choose which machine or variation to use. `[ASSUMPTION: from a standard machine library, as in the brief.]`
- A saved Workout can be started from the Dashboard.

#### FR-11: Exercise library
The app includes an Exercise library larger than the animated set. `[ASSUMPTION: about 30–40 Exercises for the prototype.]`

**Notes:** `[NOTE FOR PM]` Library size and exercise sources are open (see §8).

### 4.6 Gym Map
**Description:** A started Workout becomes a top-down room. The Avatar walks it, machine by machine. Realizes UJ-1.

#### FR-12: Generate the Gym Map
Starting a Workout generates a Gym Map with one Machine Station per Exercise in Workout order and a finish line at the end.

**Consequences (testable):**
- Each Machine Station shows the Exercise name.
- The Avatar starts at the first Machine Station.

#### FR-13: Move the Avatar
A User can drag the Avatar to any Machine Station, in any order, and can skip one.

**Consequences (testable):**
- Skipped Exercises are recorded as skipped, not as failures.
- Works with touch on mobile and tablet and with the mouse on desktop.

#### FR-14: Finish a Session
The User can walk the Avatar across the finish line after all Exercises are done, or earlier when they choose to stop.

**Consequences (testable):**
- A partly finished Session is saved and counts toward the Weekly Goal. `[ASSUMPTION]`
- The Avatar plays a finish animation and asks a few questions about how the Workout was. `[ASSUMPTION: 2–3 short questions, e.g. overall feel and energy, all skippable.]`
- XP is awarded for each finished Session, and the Avatar shows if a new Level is reached. XP amounts and Level thresholds are open (§8).
- The Avatar gives a short piece of kind feedback on the Session, based on the answers.

### 4.7 Set Logging
**Description:** The core loop. It must be quicker than the spreadsheet-style trackers it competes with. Realizes UJ-1.

#### FR-15: Log a Set
A User can log a Set with reps, weight in kg and Effort in a few taps.

**Consequences (testable):**
- Weight and reps are prefilled from the last Set or the last Session of that Exercise, and easy to raise or lower.
- Logging a Set takes no more than a few taps `[ASSUMPTION: target of 3 taps or fewer when accepting prefilled values]`.
- The User can edit or delete a logged Set.

#### FR-16: Choose the Effort scale
A User can choose between a 1–10 scale and RPE for logging Effort, and switch later.

**Notes:** The list view (a plain, non-game way to log) is not in the prototype, but the design must not exclude adding it.

### 4.8 How-To
#### FR-17: Open a How-To
A User can tap a small "?" next to an Exercise to see its How-To animation at the Machine Station.

**Consequences (testable):**
- The "?" is subtle and the How-To is never shown automatically.
- Opening it never blocks logging.
- Exercises without a How-To show no broken or empty animation `[ASSUMPTION: "?" hidden or shows "coming soon"]`.
- How-To content shows a short form-safety disclaimer.

**Notes:** Only some Exercises (about 5–10) have a How-To in the prototype, to show the feature.

### 4.9 Dashboard, Mood and Progress
**Description:** The home screen. Realizes UJ-2.

#### FR-18: Dashboard
A User sees their Avatar with Level and XP bar above it, Weekly Goal status, "Start a workout" and a link to Progress.

#### FR-19: Avatar Mood
The Avatar is happy and encouraging when the User has trained, and a little sad with a supportive message only after a whole Week without a logged Session.

**Consequences (testable):**
- Missing one or two planned workouts does not make the Avatar sad.
- The Avatar returns to happy as soon as the User logs a Session again.
- Messages never shame. They encourage.

#### FR-20: Progress view
A User can see their history, weights lifted over time and Level.

### 4.10 Offline
#### FR-21: Log without a connection
A User can start a Workout, log Sets and finish a Session offline, and the data syncs when the connection returns.

**Consequences (testable):**
- No logged Set is lost when the connection drops or the app is closed.
- AI features show a clear "needs connection" state instead of failing silently.

### 4.11 Premium (mock-up only)
#### FR-22: Show Premium as a mock-up
The app shows Premium (AI-built workouts, avatar clothes, room designs) as a non-functional mock-up. No payment.

**Notes:** After launch, AI-built workouts become Premium. Cosmetics are Premium. Logging, Gym Map, Avatar, XP and Progress stay free.

## 5. Non-Goals (Explicit)
- Not a tool for experienced lifters who want a spreadsheet-style tracker.
- Not a personal trainer or injury-rehab tool. No medical advice.
- Not a social network in v1.
- Never shames the User, and the Avatar's body never changes as punishment.

## 6. MVP Scope

### 6.1 In Scope
- Account, Avatar creation, goals with Reality Check, equipment tick-off.
- Split options from templates, editing, and building a Workout by hand.
- Exercise library, with How-To animations for a few Exercises.
- Gym Map, Set logging, finish flow, XP and Level.
- Dashboard with Mood, Weekly Goal status and Progress.
- Offline logging with sync.
- Responsive web app, mobile-first, working on tablet and desktop.
- Premium as a mock-up.

### 6.2 Out of Scope for MVP
- Real Premium payments, cosmetics and AI as a paid feature.
- Social features: friends and sharing workouts (the user's main idea for after launch).
- Selling to gyms, camera-based form checking, native app-store apps, sensors.
- A plain list view for logging (kept possible, not built).
- The Avatar raising the Weekly Goal as the User keeps it (from the brief). `[NOTE FOR PM]` Revisit after the prototype.

## 7. Success Metrics

**School prototype (primary)**
- **SM-1:** A first-time tester creates an Avatar with at least four customised features without help. Validates FR-3.
- **SM-2:** A first-time tester ends up with a Workout, either by choosing a Split option or building one by hand, without help. Validates FR-8 to FR-10.
- **SM-3:** A first-time tester walks a Gym Map of at least three Exercises, logs a Set at each, and crosses the finish line, with no data lost. Validates FR-12 to FR-15.
- **SM-4:** In a test with seeded data, the Dashboard shows the correct Mood and Weekly Goal status for a week with Sessions and for a week without. Validates FR-18, FR-19.

**Launch (secondary, `[ASSUMPTION]`: carried from the brief, not yet confirmed by the user)**
- **SM-5:** 30-day retention well above the category's 3–4%.
- **SM-6:** Most Users keep their Weekly Goal in most weeks.
- **SM-7:** Logging a Set takes a few seconds and never waits for the game. Validates FR-15, NFR-1.

**Counter-metrics (do not optimize)**
- **SM-C1:** Returns driven by guilt. Do not push retention with sadness or notification pressure. Counterbalances SM-5.
- **SM-C2:** Session time. Do not make Sessions longer for the game's sake. Counterbalances SM-3.

## Cross-Cutting Requirements

- **NFR-1 Speed:** The game never slows logging. Animations are non-blocking, and a tap during an animation is accepted and acted on within 100 ms. `[ASSUMPTION: 100 ms.]`
- **NFR-2 Platform:** Responsive web app, mobile-first, usable on tablet and desktop. `[ASSUMPTION: installable PWA is a likely route, decided in architecture.]`
- **NFR-3 Offline:** See FR-21.
- **NFR-4 Content safety:** Form guidance is checked against a trusted source once, not generated fresh, and carries a disclaimer.
- **NFR-5 Privacy:** The app holds health-related data (weights, goals, history). The prototype needs only a short privacy note. Before launch, age limits (including under-18 Users) and GDPR need a decision.
- **NFR-6 Tone:** Cozy and encouraging. The Avatar's text never judges.

## 8. Open Questions
1. Exercise library size and source, and which 5–10 Exercises get How-To animations. Form must be checked against a trusted source.
2. Name check: is RepRoute free in the app stores and as a trademark?
3. What is the Dashboard's second option beyond "Start a workout"? (Only Progress is set.)
4. What does AI do, exactly, in the prototype, given Splits come from templates? (Reality Check conversation, choosing and adapting templates.)
5. Under-18 Users and GDPR before launch.
6. Launch metrics and the social system are not defined yet.
7. The brief needs updating: Mood rule (now a whole Week missed), Split options, offline logging, Effort scales.
8. XP amounts per Session and Level thresholds.
9. Launch targets for SM-5 and SM-6 have no numbers yet.

## 9. Assumptions Index
- §4.1 FR-1: account method (email plus optional Google/Apple).
- §4.5 FR-8: 2–3 Split options; rules choose templates, AI optional.
- §4.5 FR-11: about 30–40 Exercises in the library.
- §4.6 FR-14: partial Sessions count toward the Weekly Goal; 2–3 skippable finish questions.
- §4.7 FR-15: 3 taps or fewer with prefilled values.
- §4.8 FR-17: "?" hidden or "coming soon" when no How-To exists.
- §4.5 FR-10: machine or variation chosen from a standard machine library.
- §3 Glossary: Week is Monday to Sunday.
- §7: launch metrics SM-5 to SM-7 carried from the brief.
- NFR-1: 100 ms response to taps during animations.
- NFR-2: PWA route.
