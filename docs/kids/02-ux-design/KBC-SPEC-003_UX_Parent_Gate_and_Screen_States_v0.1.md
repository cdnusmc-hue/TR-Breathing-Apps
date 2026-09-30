# Kids Breathing Coach — UX, Parent Gate, and Screen States

**Document ID:** KBC-SPEC-003  
**Version:** 0.1  
**Status:** Approved for wireframing  
**Depends on:** KBC-SPEC-001, KBC-SPEC-002

## 1. UX Baseline

One app serves two tracks: **Little Explorers (3–6)** and **Big Explorers (7–12)**. The child experience is task-first, voiced, visual, and usable without reading. Adult configuration and explanations remain behind a parent gate.

## 2. Navigation

### Child space

- Home
- Activity preview
- Guided activity
- Neutral check-out
- Something Else
- Get a Grown-up

### Grown-up space

- First-use setup
- Child profile and age track
- Activities and favorites
- Sound, motion, captions, and low-sensory settings
- Local activity history
- Safety and privacy
- Erase data

No child-facing hamburger menu, account screen, store, social surface, or settings maze.

## 3. First-Run Flow

1. Welcome: **A small tool for big feelings and busy moments.**
2. Grown-up gate.
3. Adult wellness/safety boundary and unsafe-context notice.
4. Choose track: 3–6 or 7–12; explain that it can be changed.
5. Choose narration, music, captions, reduced motion, and low-sensory defaults.
6. Optional local nickname/avatar; default is no name.
7. For ages 3–6, launch **Buddy Breaths** as the first experience.
8. Return to child Home.

## 4. Parent Gate

MVP gate: press and hold the grown-up icon for three seconds, then answer a randomized reading/math prompt such as **What is 7 + 5?** The prompt is friction, not identity verification or legal parental consent.

Gate is required for:

- creating or deleting a local profile;
- changing age track;
- viewing history;
- disabling activities;
- changing persistent accessibility defaults;
- reading detailed safety/privacy information;
- erasing all data.

The gate is not required to Stop, Get a Grown-up, make a session easier, mute sound, or enable captions.

## 5. Home

Header: **What do you need right now?**

Six large illustrated cards:

| Need | Activity |
|---|---|
| Help me slow down | Slow the Waves |
| I need a tiny pause | Tiny Reset |
| Something feels hard | Try It With Me |
| Help me get ready | Ready for the Next Thing |
| Quiet time | Moon Journey |
| Let's do it together | Buddy Breaths |

Persistent footer actions: **Something Else**, **Get a Grown-up**, and grown-up gate icon.

Little Explorers see two columns of picture cards with voiced labels. Big Explorers see the same cards with one-line descriptions.

## 6. Activity Preview

Required elements:

- character demonstration loop;
- activity name and plain purpose;
- approximate length stated as **very short**, **short**, or **quiet time** to children;
- **Start**, **Something Else**, and **Get a Grown-up**;
- first-use message: **Small, easy breaths. You can stop anytime.**

Big Explorers may open **Why this?** for one evidence-safe sentence. No seconds-based breathing pattern is shown.

## 7. Guided Activity

### Layout priority

1. Character and focal object
2. Current instruction: **Breathe in easy**, **Let it float out**, or **Let your breathing do its own thing**
3. Gentle progress path with no countdown pressure
4. Controls: Pause, Stop, Something Else, Get a Grown-up

### Behavior

- Demonstrate one cycle before inviting participation.
- Never grade synchronization.
- Pause freezes story and cues; resume begins with normal breathing.
- Stop immediately ends pacing and says: **Okay. Let your breathing do its own thing.**
- Backgrounding or locking ends the active session.
- Low-sensory mode uses static images, captions, and optional soft tones.

## 8. Check-Out

Prompt: **What do you notice?**

Little Explorers: Same / A little different / Not sure / Skip.  
Big Explorers: Same / A little calmer / A little more ready / Something else / Not sure / Skip.

Completion response: **You practiced. You don't have to feel different right away.**

Actions: Done / Do another / Favorite. Moon Journey replaces this screen with a dim **All done** control.

## 9. Something Else

Three large choices:

- **Move** — short stretch or animal shake
- **Use My Senses** — name or find simple things nearby
- **Get a Grown-up** — voiced prompt to find a trusted adult

These are peers to breathing, not failure fallbacks.

## 10. Error and Interruption States

| State | Required response |
|---|---|
| Audio unavailable | Continue visually with captions |
| Haptics unavailable | No warning to child; continue |
| App backgrounded | End active pacing; offer Start Again on return |
| Asset missing | Use static character and text/voice fallback |
| Storage unavailable | Run sessions without saving history |
| Motion reduced | Replace expansion with static phase cards |
| Child taps repeatedly | Debounce; never accelerate breathing cues |
| Session stopped | Neutral close; no loss or retry pressure |

## 11. Accessibility Controls

- Minimum 48×48 CSS-pixel child targets
- Text resizing without clipped controls
- Captions for every essential spoken instruction
- Phase communicated by words, shape, and movement—not color alone
- Screen-reader names that describe action, not decorative art
- Reduced motion, no music, no vibration, and low-sensory presets
- No time-limited decisions

## 12. Acceptance Gate

Wireframes may proceed when every screen supports Stop/Get a Grown-up, both tracks can complete all six activities, adult controls are gated, and no screen exposes scores, precise breathing performance, medical claims, or network identity.

## 13. Change History

| Version | Date | Change |
|---|---|---|
| 0.1 | 2026-09-19 | Initial UX, navigation, parent-gate, accessibility, and screen-state specification. |
