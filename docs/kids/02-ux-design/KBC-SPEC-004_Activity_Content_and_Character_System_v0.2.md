# Kids Breathing Coach — Activity, Content, and Character System

**Document ID:** KBC-SPEC-004  
**Version:** 0.2  
**Status:** Animal-mechanic prototype baseline  
**Depends on:** KBC-SPEC-002, KBC-SPEC-003

## 1. Character Decision

Use a small ensemble of animal guides across both age tracks. The selected animal embodies the breathing mechanic, making the cue easier to understand without adding technical explanation. Presentation is warmer and more expressive for Little Explorers and calmer and less babyish for Big Explorers. No animal claims friendship, secrecy, expertise, feelings about the child's behavior, or a need for the child to return.

The home guide may still be **Pip**, while activity animals rotate by mechanic. Final species and visual direction remain open.

## 2. Reusable Character Actions

- idle and welcome;
- demonstrate easy inhale;
- demonstrate relaxed exhale;
- normal unpaced breathing;
- wave motion;
- feather float;
- balloon lift without inflating lungs maximally;
- simple stretch/shake;
- point to Stop or Get a Grown-up;
- quiet Moon Journey pose;
- neutral goodbye.

## 2.1 Animal mechanic library

| Animal/scene | Approved mechanic | Role |
|---|---|---|
| Flower + candle | Easy inhale, gently longer exhale | First-use onboarding |
| Snake | Soft continuous `ssss` exhale | Controlled exhale |
| Bumblebee | Soft humming exhale | Voiced exhale |
| Bear | Gentle belly rise and fall without holds | Quiet/rest |
| Bunny | One small inhale and normal exhale only | Brief reset, not looping |
| Tiger | Stretch plus one easy `haa` | Movement/expression alternative |
| Cow | Quiet `moo` exhale | Optional voiced variation |
| Duck | One gentle long quack | Optional voiced variation |

Detailed evidence and cadence governance are defined in KBC-RES-001.

## 3. Script Rules

- One instruction per sentence.
- Little Explorer sentence target: 3–7 words.
- Big Explorer sentence target: 4–12 words.
- Say **easy**, **small**, **comfortable**, and **let it out**.
- Never say deep, full, empty, perfect, harder, longer, win, fail, or control.
- Validate the moment without labeling the child.
- Demonstrate before requesting imitation.
- End with agency, not an asserted outcome.

## 4. Activity Matrix

| Activity | Little Explorer default | Big Explorer default | Core cue | Close |
|---|---:|---:|---|---|
| Slow the Waves | 45 sec | 90 sec | Snake or wave: easy in, controlled out | Notice what is here now |
| Tiny Reset | 30 sec | 45 sec | Bunny: one easy cycle, then normal breathing | Choose the next tool |
| Try It With Me | 45 sec | 90 sec | Bumblebee: soft humming exhale | Pick one small next step |
| Ready for the Next Thing | 45 sec | 75 sec | Flower/candle: smell, then make flame dance | Name the next thing |
| Moon Journey | 2 min | 4 min | Bear: quiet rise and fall without holds | Dim all-done state |
| Buddy Breaths | 60 sec | 2 min | Child/adult choose an approved animal | Grown-up connection prompt |

Durations are prototype defaults, not physiological prescriptions.

## 5. Little Explorer Sample Script: Slow the Waves

1. **The water feels wiggly.**
2. **Watch Pip first.**
3. **A small breath comes in.**
4. **The wave slides out.**
5. **Want to try with Pip?**
6. Repeat gentle animation without performance feedback.
7. **You practiced. What next?**

## 6. Big Explorer Sample Script: Slow the Waves

1. **Let's take a short pause. Watch one easy breath.**
2. **Breathe in comfortably.**
3. **Let the breath out as the wave settles. Don't force it.**
4. Continue for the short progress path.
5. **Notice what is here now. It is okay if nothing changed.**

## 7. Tiny Reset Logic

Tiny Reset is not a physiological-sigh protocol for children. It uses:

1. normal breathing for five seconds;
2. one comfortable inhale;
3. one relaxed, unforced exhale;
4. normal unpaced breathing for 10–15 seconds;
5. choice: Move / Senses / Grown-up / Done.

It never loops automatically.

## 8. Rewards

MVP reward: reveal a small cosmetic story detail after participation, such as a star appearing in Pip's sky. No streak, scarcity, locked therapeutic content, score, punishment, or reward tied to reported mood change. All six activities remain available.

## 9. Content Configuration Contract

Each activity definition includes ID, version, track, display text, narration asset, ordered phases, flexible phase window, maximum duration, character action, sensory alternatives, interruption behavior, safety copy, reflection options, and evidence/approval status.

No content may ship without a version and approval state.

## 10. Change History

| Version | Date | Change |
|---|---|---|
| 0.1 | 2026-09-19 | Established character role, activity matrix, scripts, reward boundary, and content contract. |
| 0.2 | 2026-09-19 | Replaced single-character activity model with evidence-governed animal mechanics and cadence references. |
