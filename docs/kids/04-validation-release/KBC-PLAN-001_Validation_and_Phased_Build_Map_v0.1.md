# Kids Breathing Coach — Validation and Phased Build Map

**Document ID:** KBC-PLAN-001  
**Version:** 0.1  
**Status:** Working execution plan

## 1. Delivery Strategy

Build one golden vertical slice first: Big Explorer **Slow the Waves**, including Home, preview, demonstration, session, Stop, Something Else, Get a Grown-up, check-out, local settings, offline behavior, and failure states. Then add the Little Explorer script and remaining content.

## 2. Phases

| Phase | Deliverable | Exit gate |
|---|---|---|
| 0 Baseline | Approve specs, character direction, claims, and safety copy | No unresolved P0 decision |
| 1 Clickable prototype | Both Home variants, Slow the Waves journey, adult gate | Caregiver walkthrough succeeds |
| 2 Golden slice | Runnable offline Big Explorer Slow the Waves | Timing, Stop, background, accessibility tests pass |
| 3 Two-track engine | Little Explorer variant and content registry | Both tracks run from one engine |
| 4 Activity set | All six activities plus alternatives | Content/safety review passes |
| 5 Hardening | Storage, install, offline, low sensory, reduced motion, browser coverage | Automated acceptance suite passes |
| 6 Formative beta | Supervised child/caregiver testing | Age-band thresholds pass |
| 7 Release candidate | Privacy, security, clinical, accessibility, app-store review | Signed release checklist |

## 3. P0 Acceptance Tests

### Safety

- Stop ends pacing and all cues immediately.
- Backgrounding ends rather than resumes an active activity.
- No content includes holds, rapid breathing, maximal inhale, forced exhale, or competitive instruction.
- Get a Grown-up is reachable from every child activity screen.
- Repeated taps cannot accelerate cue timing.

### Privacy

- No request sends child/profile/activity data to a remote endpoint.
- No analytics, ads, remote fonts, embedded media, microphone, camera, or location permission exists.
- Erase Data removes all app-created local records.

### Accessibility

- Essential journeys work with screen reader, text enlargement, reduced motion, no audio, and no haptics.
- Controls meet target size and contrast requirements.
- Meaning never depends on color alone.

### Reliability

- Core sessions work after installation with network disabled.
- Unsupported audio/haptics/storage degrade without blocking the activity.
- Timing remains within defined perceptual tolerance on supported devices.

## 4. Formative Test Plan

Test separately with ages 3–4, 5–6, 7–9, and 10–12 plus caregivers. Begin with five child/caregiver pairs per band for discovery; iterate before larger validation.

Observe comprehension, accidental breath holding, forceful breathing, stopping, adult-support discovery, sensory response, story distraction, and beliefs about scores or required calm.

## 5. Release Thresholds

- 80% in each age band follow the core action without corrective coaching.
- 90% stop independently or clearly signal a wish to stop.
- No moderate/severe breathing-related adverse event.
- 80% understand they need not feel different afterward.
- 90% of caregivers correctly state product limits.
- Zero undeclared child-data network transmission.
- No critical accessibility, offline, timing, privacy, or safety defect.

## 6. Initial Build Backlog

| Priority | Work item |
|---|---|
| P0 | Repository, dependency lock, CI, lint, unit and browser test shell |
| P0 | Design tokens and accessible app shell |
| P0 | Versioned activity schema and validator |
| P0 | Monotonic timing engine and interruption state machine |
| P0 | Home, preview, active, stop, alternatives, check-out |
| P0 | Adult gate and local settings |
| P0 | Offline cache and install manifest |
| P0 | Slow the Waves assets and both age scripts |
| P1 | Remaining five activities |
| P1 | Low-sensory, reduced-motion, captions, haptics |
| P1 | Local favorites/history and erase-data control |
| P1 | Automated privacy/network and accessibility suites |
| P2 | Cosmetic story progression after validation |

## 7. Decisions Still Needed Before Coding

1. Final character species, name, and visual direction
2. Brand name and relationship to Adult Breathing Coach
3. Narrator voice and production method
4. Supported minimum iOS/Safari and Android/Chrome versions
5. Whether first prototype uses temporary geometric animation or finished character art

Recommended: use temporary geometric art for the golden slice, validate the interaction, then invest in finished character animation.

## 8. Laptop Handoff Point

Laptop becomes necessary at Phase 2 when creating the repository, running Node tooling, previewing the PWA across browsers, and executing automated tests. All Phase 0 and most Phase 1 review work can be completed on mobile.

## 9. Change History

| Version | Date | Change |
|---|---|---|
| 0.1 | 2026-09-19 | Initial validation gates, phased build map, backlog, and laptop handoff. |
