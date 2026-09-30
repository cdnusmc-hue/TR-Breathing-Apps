# Kids Breathing Coach — Visual Design System

**Document ID:** KBC-DS-001  
**Version:** 0.1  
**Status:** Prototype design baseline

## 1. Design Intent

The interface should feel safe, playful, spacious, and immediately understandable. It must not resemble a medical tool, high-stimulation game, or preschool worksheet.

## 2. Color Tokens

| Token | Value | Use |
|---|---|---|
| Creek Navy | `#18364A` | Primary text and dark controls |
| Sky Blue | `#D9F1F5` | General background |
| Meadow Green | `#6FAF85` | Positive navigation accents |
| Sun Gold | `#F6C85F` | Pip glow and selection highlight |
| Coral | `#E98473` | Warm secondary accent |
| Lavender | `#9B8BC4` | Quiet/Moon Journey accent |
| Cloud | `#F8FBFA` | Cards and panels |
| Stop Red | `#B33A3A` | Stop only; paired with label/icon |

Every foreground/background pairing must meet WCAG 2.2 AA. Color never carries phase or state alone.

## 3. Typography

- Primary: rounded humanist sans-serif with open counters; bundle locally.
- Little: 24–32 px headings, 20–24 px instructions, minimal body copy.
- Big: 22–28 px headings, 18–22 px instructions, 16–18 px explanations.
- Adult: 16 px minimum body size.
- Avoid all-caps except very short control labels.
- Maximum child-facing line length: roughly 28 characters for Little, 45 for Big.

## 4. Shape and Layout

- 16 px base corner radius; 24 px on primary child cards.
- Minimum target: 48×48 CSS px; primary cards at least 104 px high.
- 8 px spacing grid with 24 px outer mobile margin.
- One dominant focal character per active screen.
- No more than six Home choices; two-column Little grid and flexible Big list/grid.
- Stop remains bottom-center or bottom-right in a consistent safe area.

## 5. Motion Language

- Inhale: character/object rises or expands 4–8%, never rapidly.
- Exhale: longer smooth travel, glide, curl, dim, or settle.
- Normal breathing: small ambient loop without timing demand.
- Transition duration: 250–400 ms.
- Breathing phase easing uses smooth in/out curves without bounce.
- Reduced motion replaces scaling/travel with static phase cards and gentle opacity shifts.
- No flashes, confetti, camera shake, sudden zoom, or urgent countdown.

## 6. Iconography

Rounded, filled-line icons with text labels. Required icons: Home, Pause, Resume, Stop, Sound, Captions, Low Sensory, Grown-up, Move, Senses, Favorite, Back. Stop uses a square inside a circle, never color alone.

## 7. Component Inventory

- AnimalActivityCard
- PrimaryActionButton
- SafetyActionRow
- CharacterStage
- PhaseInstruction
- GentleProgressTrail
- SensoryToggle
- ParentGatePrompt
- ReflectionChoice
- StaticFallbackCard
- AdultSettingRow
- SafetyNotice

Each component has default, pressed, focused, disabled, loading, and error states where applicable.

## 8. Audio and Haptics

- Narration is warm and direct, not whispery or theatrical.
- Music defaults off during first-use safety setup; adults may enable it.
- Essential meaning is never encoded in music.
- Phase tones are optional and distinct but soft.
- Haptic inhale/exhale patterns remain optional and are not used on every cycle for Little Explorers.

## 9. Track Adaptation

| Dimension | Little 3–6 | Big 7–12 |
|---|---|---|
| Copy | Concrete, voiced, 3–7 words | Concise explanation, 4–12 words |
| Cards | Large picture-first | Picture plus purpose |
| Animation | Clear environmental response | Subtler character movement |
| Choice count | 2–3 per decision screen | Up to 4 |
| Progress | Visual trail | Visual trail plus optional time category |
| Rewards | One gentle world detail | Optional collection view without streaks |

## 10. Acceptance

The design system passes when all required screens can be composed from the inventory, both tracks remain recognizable as one product, Stop/Grown-up are unmistakable, and reduced-motion/low-sensory variants preserve the full journey.

## 11. Change History

| Version | Date | Change |
|---|---|---|
| 0.1 | 2026-09-19 | Initial tokens, typography, layout, motion, components, sensory behavior, and track adaptation. |
