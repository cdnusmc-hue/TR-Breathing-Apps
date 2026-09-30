# Kids Breathing Coach
## Foundation and Product Requirements Document

**Document ID:** KBC-SPEC-001  
**Version:** 0.1  
**Status:** Working Draft  
**Product stage:** Pre-build  
**Relationship:** Child-focused companion to Breathing Coach; separate pediatric product boundary

## 1. Product Definition

Kids Breathing Coach is an installable, mobile-first web application for children ages 3–12 and their caregivers. It uses an animated character, short stories, and simple playful visuals to guide brief, comfortable breathing activities intended to help children pause, settle, reset, or prepare for an ordinary moment.

The product begins with a concrete, child-friendly question: **What do you need right now?** A child or caregiver chooses a goal and begins an age-appropriate guided activity within seconds.

### Product promise

Help a child begin a safe, understandable breathing activity in no more than three taps and ten seconds—with no technique knowledge required.

### Core problem

Children often cannot translate broad instructions such as “calm down” or “take a deep breath” into a usable action. Most breathing tools are written for adults, depend on abstract emotional vocabulary, or use timing and breath holds that may be confusing or uncomfortable for young children.

### Product thesis

Breathing guidance for children should feel like playing along with a trusted character, not completing an exercise. The child chooses a recognizable need; the character demonstrates a gentle action inside a very short story.

## 2. Audience and Developmental Tracks

Version 1 serves ages 3–12 through two presentation tracks using the same governed session engine.

### Little Explorers: ages 3–6

- Primarily picture, animation, sound, and caregiver-readable prompts
- Concrete imitation: smell the flower, cool the cocoa, float the feather
- Sessions generally 30–90 seconds
- No required reading, counting, breath holds, or precise performance
- Caregiver co-use encouraged, but not required for ordinary gentle sessions

### Big Explorers: ages 7–12

- Child-readable language with optional voice guidance
- Short missions, stories, and explanations of what to do
- Sessions generally 1–3 minutes
- Optional simple pacing choices within approved bounds
- More independent use, while parent controls remain available

### Shared adult role

A parent or caregiver can start any activity, select the developmental track, preview instructions, change sensory settings, review locally stored activity history, and lock settings that should not be child-editable.

Age changes presentation and defaults; it does not create a claim that all children develop identically. Caregivers can switch tracks at any time.

## 3. Version 1 Contexts

- Settling after frustration or overstimulation
- Pausing before reacting
- Preparing for school, homework, a performance, or a difficult conversation
- Transitioning toward bedtime
- Regaining composure after a minor everyday upset
- Practicing a regulation skill with a parent, caregiver, teacher, or counselor

## 4. Explicit Exclusions

- Diagnosis or treatment of anxiety, panic, ADHD, autism, trauma, insomnia, asthma, or any medical or mental-health condition
- Emergency intervention or crisis support
- Rapid breathing, hyperventilation, hypoxic training, prolonged breathing, or breath-hold challenges
- Competitive breathing, scores based on duration or depth, leaderboards, or “beat your best” mechanics
- Claims that a child should be able to control every emotion through breathing
- Replacing adult support, clinical care, medication, sleep, movement, food, or environmental changes
- School, clinician, or parent surveillance dashboards in Version 1

## 5. Product Principles

1. **Connection before correction:** The app validates the child’s state before offering an activity.
2. **Play, not performance:** The child helps a character complete a gentle action; there is no perfect breath.
3. **Developmentally appropriate:** Words, session length, choices, and visuals adapt by age track.
4. **Child or adult can start:** Both routes reach the same safe activity quickly.
5. **Never force calm:** A child may stop, skip, or choose another activity without failure language.
6. **No deep-breath command:** Use “small,” “easy,” “slow,” or “comfortable” breathing language pending pediatric review.
7. **Safety beats engagement:** No streak, reward, story, or character reaction pressures a child to continue.
8. **Privacy by default:** No account, advertising, social sharing, behavioral profiling, or third-party tracking in the private MVP.
9. **Breathing is one tool:** The app may offer movement, sensory grounding, or “get a grown-up” when breathing is not the right next step.

## 6. Core Experience

### Home question

**What do you need right now?**

The home screen uses large illustrated choices. Working Version 1 goals are:

| Child-facing goal | Working activity | Experience concept | Default length |
|---|---|---|---:|
| I need to settle | Slow the Waves | Character breathes gently as waves rise and fall | 60 sec / 2 min |
| I’m really upset | Tiny Reset | One or two easy sigh-like releases, then normal breathing and adult-support choice | Under 60 sec |
| I need courage | Brave Balloon | Comfortable, even breaths while a balloon gradually lifts | 60 sec / 2 min |
| I need to focus | Feather Mission | Easy paced breathing followed by one simple “what comes next?” prompt | 60 sec / 2 min |
| Time to rest | Moon Journey | Dim, quiet story with slow comfortable breathing | 2 min / 5 min |
| Let’s do it together | Buddy Breaths | Child and caregiver mirror the character together | 60 sec / 3 min |

Lengths before and after the slash indicate Little Explorer and Big Explorer defaults. Names, breathing patterns, and claims require pediatric evidence and safety review before implementation.

### Non-breathing exit routes

Every emotional goal must also allow:

- **Move instead** — a brief stretch, shake, or animal movement
- **Use my senses** — a simple grounding activity
- **Get a grown-up** — prompts the child to find a trusted adult
- **Stop** — immediately ends cues without disappointment language

## 7. Character and Story System

### Character role

The animated coach is a friendly companion who performs the activity with the child. The character never diagnoses, evaluates the child’s emotional state, demands compliance, or claims to know how the child feels.

### Story structure

Each guided activity follows a compact arc:

1. **Notice:** “It looks like we need a pause.”
2. **Invitation:** “Want to help me move the waves?”
3. **Demonstration:** The character shows one complete comfortable cycle.
4. **Play-along:** The child joins for a short series.
5. **Choice:** Continue briefly, choose another tool, get a grown-up, or finish.
6. **Close:** “You practiced. You don’t have to feel different right away.”

### Visual rules

- Simple focal animation with minimal background activity during breathing
- Phase meaning conveyed through movement, shape, text, and sound—not color alone
- No flashing, startling transitions, shrinking countdown pressure, or loss animations
- Reduced-motion version replaces expansion animation with static prompts and gentle progress markers
- Characters do not look distressed when the child stops or skips

## 8. Primary User Journeys

### Child-started

1. Child opens the app.
2. Child selects an illustrated need.
3. Character names the activity and demonstrates once.
4. Child chooses **Play**, **Do something else**, or **Get a grown-up**.
5. Session runs with persistent pause and stop controls.
6. Child chooses a simple optional check-out: same, a little different, or skip.

### Caregiver-started

1. Adult taps **Grown-ups** from Home.
2. Adult selects the child’s presentation track and a goal.
3. Adult sees a one-screen preview: what happens, duration, safety note, and alternatives.
4. Adult starts **Child plays** or **Do it together**.
5. Completion offers a neutral observation note and no diagnostic interpretation.

### Fast path

A returning child can begin the last favorite activity from Home with one tap, subject to any required first-use adult gate.

## 9. Functional Requirements

### FR-01 Profiles without identity

- Support optional local child profiles using a nickname or avatar only.
- Store age track, sensory settings, favorite character, and favorite activities locally.
- Do not request full name, birth date, school, location, photo, voice recording, or contact information.
- Allow an adult to delete a profile and all associated local history.

### FR-02 Goal selection

- Display no more than six primary illustrated choices.
- Provide voiced labels for prereaders.
- Keep **Get a grown-up** continuously accessible.
- Avoid asking a young child to diagnose or precisely label an emotion.

### FR-03 Guided activity engine

- Run configuration-controlled inhale, exhale, normal-breathing, movement, narration, and rest phases.
- Support age-specific scripts and durations without separate hard-coded engines.
- Show and speak the current action in plain language.
- Support pause, resume, restart, skip, make easier, and immediate stop.
- If the app is backgrounded, end active guidance safely rather than resuming unexpectedly.

### FR-04 Character, audio, and haptics

- Animate the character in sync with the activity.
- Independently control narration, music, tones, vibration, captions, and animation.
- Provide a no-music mode and a low-sensory mode.
- Never require audio, color perception, or rapid visual tracking to understand an activity.

### FR-05 Adult area

- Protect adult settings with a parent gate appropriate to the device context.
- Explain each activity, its intended ordinary-use context, and its limits.
- Let adults select age track, disable activities, set sensory defaults, and erase data.
- Show completed activities only as neutral history; do not score mood, compliance, or child behavior.

### FR-06 Reflection

- Reflection is optional and can always be skipped.
- Little Explorers use three neutral illustrated choices: **same**, **a little different**, **not sure**.
- Big Explorers may use a short child-readable scale plus **not sure**.
- Do not tell a child that the activity “worked” or “failed.”

### FR-07 Offline installation

- Operate as an installable Progressive Web App.
- Cache the app shell, approved activities, characters, voice cues, and safety content.
- Run all core activities without a network connection.

### FR-08 Accessibility

- Target WCAG 2.2 AA for the adult interface and child-appropriate equivalent access throughout.
- Support captions, screen readers, large targets, large text, reduced motion, and one-handed adult operation.
- Provide low-sensory presentation without music, haptics, or busy scenery.
- Use plain language and recorded narration for essential child instructions.

## 10. Preliminary Safety Requirements

These are conservative product controls pending a pediatric evidence and clinical review.

- Version 1 uses only gentle breathing with no required breath holds.
- No activity asks a child to inhale maximally, empty the lungs, breathe rapidly, compete, or continue through discomfort.
- A first-use adult screen explains that the product is a general wellness activity, not medical care.
- Child-facing instruction: **Use small, easy breaths. Stop if your body feels funny or uncomfortable.**
- Stop immediately for dizziness, tingling, chest discomfort, unusual shortness of breath, panic, or distress.
- The app must not be used in water, while moving near traffic, during sports, or in any situation requiring full attention.
- A child with a relevant medical or psychological condition should use the product only as appropriate under caregiver and qualified professional guidance.
- **Get a grown-up** is always available; urgent symptoms direct the adult to appropriate emergency services.
- No Power Up/Bellows Lite, breath of fire, Wim Hof-style, or other activating rapid-breath protocol from the adult product carries into the kids MVP.
- Caregiver consent and child privacy requirements must be resolved before any cloud account, analytics, voice input, personalization service, or data transmission is introduced.

## 11. Data and Privacy Boundary

### Stored locally in MVP

- Optional nickname/avatar
- Selected age track
- Accessibility and sensory settings
- Favorites
- Activity name, completion state, and duration
- Optional neutral before/after response

### Not collected in MVP

- Full name, precise birth date, email, phone number, address, school, location, contacts, photos, audio, biometrics, health diagnosis, free-text journal, advertising identifier, or cross-app behavior

### Product rule

The private MVP has no advertising, third-party tracking, behavioral marketing, social sharing, or external analytics. Any future networked data collection requires a separate child-privacy, parental-consent, security, and retention specification before implementation.

## 12. Nonfunctional Requirements

- **Start speed:** first recommended activity begins within ten seconds after opening.
- **Performance:** interactive within two seconds on a typical modern phone after first load.
- **Reliability:** active activities do not depend on a network request.
- **Timing:** cues remain perceptually synchronized and fail safely after browser interruption.
- **Privacy:** local-first with no identity requirement.
- **Accessibility:** essential actions have visual, spoken, and accessible-text equivalents.
- **Maintainability:** activities, scripts, pacing, character actions, and age variants are configuration-controlled and versioned.

## 13. MVP Success Criteria

- At least 90% of tested caregivers can select the appropriate age track and start an activity without instruction.
- At least 80% of children in each age track can follow the central cue without adult correction.
- Median time from Home to activity start is under ten seconds.
- At least 90% of children can find Stop or communicate that they want to stop.
- At least 80% understand that they may stop and do not have to make the character “win.”
- Caregivers understand that the app supports practice rather than treatment or guaranteed emotional change.
- No critical safety, privacy, timing, accessibility, or background-resume defect remains.
- Success is measured separately for ages 3–6 and 7–12; aggregate results cannot hide failure in one group.

## 14. Required MVP

- Two developmental presentation tracks
- One animated coach with a small reusable action set
- Six child-facing goals/activities, subject to evidence review
- Short story wrapper and simple playful visuals
- Child-start and caregiver-start journeys
- Do-it-together mode
- Breathing, movement, grounding, grown-up, and stop choices
- Voice, captions, reduced motion, low-sensory mode, and independent cue controls
- Local favorites, preferences, and minimal neutral history
- Offline PWA installation
- Adult gate, first-use safety explanation, urgent-symptom boundary, and data deletion

## 15. Deferred

- Cloud accounts and synchronization
- Multiple children across devices
- School, therapist, counselor, or pediatrician portals
- AI conversation or generated advice
- Camera, microphone, emotion detection, or biometric inference
- Wearables and heart-rate integration
- Social features, leaderboards, public sharing, streak pressure, and competitive rewards
- Advertising, subscriptions, or monetization experiments
- Clinical positioning or condition-specific programs
- Activating/rapid breathing protocols

## 16. Open Decisions Before UX Specification

1. Character identity, personality, and art direction
2. Whether the same character grows visually between age tracks or each track has a different guide
3. Exact activity set, cadence, duration, and adjustment bounds after pediatric review
4. Parent-gate method for an installable web app
5. Narrator voice strategy and whether caregiver-recorded voices are excluded permanently or only from MVP
6. Reward design limited to cosmetic story progression without pressure or emotional scoring
7. Brand relationship: standalone Kids Breathing Coach or a family product under the Breathing Coach brand
8. Whether school/counselor contexts are supported in the initial public release or deferred

## 17. Pre-Build Gates

Implementation is not yet authorized. The sequence is:

1. Approve this foundation and PRD.
2. Complete pediatric evidence, clinical-safety, child-development, privacy, and regulatory reviews.
3. Revise and approve the activity set and language.
4. Specify information architecture, navigation, parent gate, and all screen states.
5. Produce low-fidelity wireframes for both age tracks.
6. Approve character direction, visual system, narration, and sensory-accessibility behavior.
7. Define technical architecture, timing engine, content configuration, storage, and offline behavior.
8. Write acceptance tests, safety tests, privacy tests, and failure-state requirements.
9. Conduct formative usability sessions with children and caregivers before feature-complete implementation.
10. Approve the build baseline.

## 18. Current Recommendation

Proceed as a separate child-focused, offline-first PWA that shares architectural concepts with the adult product but not its content assumptions. Build one character and two developmental presentations around the same six small activities. Keep Version 1 local-only, noncompetitive, free of rapid breathing and holds, and explicit that a child can stop or seek a grown-up at any time.

The immediate next artifact should be **KBC-SPEC-002 — Pediatric Evidence, Safety, Development, and Privacy Review**. That review must challenge the proposed activity set before wireframing begins.
