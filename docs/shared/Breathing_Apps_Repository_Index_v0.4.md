# Breathing Apps Document Repository

**Document ID:** BA-CTRL-001  
**Version:** 0.4  
**Status:** Active index  
**Updated:** 2026-09-19

## 1. Repository Purpose

This repository governs two related but independently validated products:

- **Breathing App Adult** — general-wellness breathing coach for adults
- **Breathing App Kids** — child-focused breathing and regulation companion for ages 3–12

The products may share technical components, but pediatric content, safety, claims, consent, and testing do not inherit automatically from the adult product.

## 2. Controlled Folder Standard

Each product branch uses:

| Folder | Purpose |
|---|---|
| 00 Program Controls | Indexes, decision logs, roadmap, risks, release gates |
| 01 Product and Research | Foundation, PRD, evidence, safety, privacy, content decisions |
| 02 UX and Design | Information architecture, user flows, screen states, wireframes, design system |
| 03 Architecture | Technical architecture, data model, session engine, offline behavior, security |
| 04 Validation and Release | Acceptance tests, usability plans/results, clinical review, release checklist |

## 3. Current Controlled Documents

### Adult branch

| Document | ID | Status | Location |
|---|---|---|---|
| Foundation and PRD | BC-SPEC-001 | Working Draft | 01 Product and Research |
| Evidence and Safety Review | BC-SPEC-002 | Review complete; changes required | 01 Product and Research |
| Energy + Focus Mode Decision | BC-ADR-001 | Accepted | 01 Product and Research |

### Kids branch

| Document | ID | Status | Location |
|---|---|---|---|
| Foundation and PRD | KBC-SPEC-001 | Working Draft | 01 Product and Research |
| Pediatric Evidence, Safety, Development, and Privacy Review | KBC-SPEC-002 | Review complete; changes required | 01 Product and Research |
| Animal Breathing Techniques: Evidence and Cadence | KBC-RES-001 | Prototype prescriptions approved with validation requirements | 01 Product and Research |
| Animal Cast and Visual Direction | KBC-ADR-001 | Accepted for prototype | 01 Product and Research |
| UX, Parent Gate, and Screen States | KBC-SPEC-003 | Approved for wireframing | 02 UX and Design |
| Activity, Content, and Character System | KBC-SPEC-004 v0.2 | Animal-mechanic prototype baseline | 02 UX and Design |
| Low-Fidelity Wireframes | KBC-WF-001 | Ready for interactive prototype | 02 UX and Design |
| Technical Architecture | KBC-ARCH-001 | Proposed MVP baseline | 03 Architecture |
| Validation and Phased Build Map | KBC-PLAN-001 | Working execution plan | 04 Validation and Release |
| Visual Design System | KBC-DS-001 | Prototype design baseline | 02 UX and Design |
| Interaction and Animation Storyboard | KBC-SB-001 | Ready for clickable prototype | 02 UX and Design |
| Six-Activity Script and Cadence Pack | KBC-CONTENT-001 | Prototype content approved; clinical review pending | 02 UX and Design |

## 4. Build Sequence

### Adult

1. Reconcile BC-SPEC-001 with BC-SPEC-002 and BC-ADR-001.
2. Create BC-SPEC-003 UX, Navigation, and Screen-State Specification.
3. Produce low-fidelity wireframes.
4. Define visual direction and design system.
5. Define technical architecture and acceptance tests.
6. Approve build baseline.

### Kids

1. Reconcile KBC-SPEC-001 with KBC-SPEC-002.
2. Freeze the initial activity set and child-safe language.
3. Create KBC-SPEC-003 UX, Parent Gate, and Screen-State Specification.
4. Produce separate wireframes for ages 3–6 and 7–12.
5. Define character system, narration, accessibility, and low-sensory behavior.
6. Define shared technical architecture and pediatric-specific controls.
7. Run child/caregiver usability and safety validation before public release.

## 5. Document Rules

- Markdown is the default specification format.
- Each controlled document has an ID, version, status, and change history.
- Architecture decisions that supersede a specification must identify the exact affected requirement.
- Adult evidence cannot be represented as pediatric evidence without explicit review.
- Product claims must trace to an approved evidence review.
- Public release requires completed safety, privacy, accessibility, and usability gates.
- Build work may begin only after the relevant baseline is approved.

## 6. Immediate Next Work

- **Kids:** Approve character direction, then build the clickable prototype and golden vertical slice
- **Adult:** BC-SPEC-003 UX, Navigation, and Screen-State Specification

The Kids UX specification proceeds first in the Kids project thread. The Adult UX specification proceeds independently in the Adult project thread.

## 7. Change History

| Version | Date | Change |
|---|---|---|
| 0.1 | 2026-09-19 | Established two-branch repository, controlled folders, current inventory, and build sequence. |
| 0.2 | 2026-09-19 | Added Kids UX, content system, wireframes, architecture, and validation/build plan. |
| 0.3 | 2026-09-19 | Added animal-breathing evidence/cadence review and revised the content system around approved mechanics. |
| 0.4 | 2026-09-19 | Added animal-cast decision, visual system, interaction storyboard, and complete script pack. |
