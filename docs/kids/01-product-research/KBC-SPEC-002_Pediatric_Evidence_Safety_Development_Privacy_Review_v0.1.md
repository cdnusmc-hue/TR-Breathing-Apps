# Kids Breathing Coach
## Pediatric Evidence, Safety, Development, and Privacy Review

**Document ID:** KBC-SPEC-002  
**Version:** 0.1  
**Status:** Review complete; product changes required  
**Scope:** General-wellness application for ages 3–12  
**Review date:** 2026-09-19

## 1. Executive Decision

The product may proceed to UX specification as a conservative general-wellness tool, but it must not be built as a direct reskin of the adult Breathing Coach.

The evidence base for breathing activities in children is promising but less direct, less standardized, and more dependent on broader mindfulness, biofeedback, procedural-anxiety, or multi-component programs than the adult slow-breathing literature. Version 1 therefore requires:

- ordinary-use positioning rather than treatment claims;
- short, gentle, noncompetitive activities;
- no fixed adult breathing rate imposed across ages 3–12;
- no breath holds or activating rapid-breathing modes;
- developmentally different presentation for ages 3–6 and 7–12;
- a persistent path to stop, switch strategies, or get a trusted adult;
- no network collection of child personal information in the MVP.

### Gate decision

**Authorized:** UX specification, wireframing, prototype timing research, and supervised usability testing.  
**Not authorized:** Public clinical claims, condition-specific programs, remote child accounts, third-party analytics, advertising, voice capture, emotion detection, or unsupervised public launch.

## 2. Evidence Standard

Evidence was weighted in this order:

1. Pediatric systematic reviews and controlled trials
2. Pediatric physiological or biofeedback studies
3. Pediatric clinical guidance from established institutions
4. Adult evidence used only as indirect support
5. Tradition, popularity, and commercial practice

Because the direct literature does not validate one universal child tempo or story mechanic, the review distinguishes between:

- evidence for broad, gentle breathing or mindfulness practices;
- evidence for a particular pace or duration;
- evidence for the app's specific consumer outcome claim.

## 3. Evidence Conclusions

### 3.1 Gentle paced breathing as a regulation practice

**Evidence position: Limited-to-moderate for broader pediatric interventions; limited for a standalone app protocol.**

Pediatric mindfulness, relaxation, and HRV-biofeedback programs commonly include breath awareness or paced breathing and report potential benefits for stress, anxiety, or physiological regulation. However, programs often combine breathing with education, movement, attention training, therapist support, or biofeedback. Results do not establish that a single app-guided breathing pattern reliably changes a child's emotional state.

**Product decision:** Gentle paced breathing may be offered as one regulation skill. Copy uses “practice,” “pause,” “settle,” and “may help,” never “treat,” “fix,” “stop anxiety,” or “control your emotions.”

### 3.2 Exact cadence across ages 3–12

**Evidence position: Insufficient for one universal fixed rate.**

Children's spontaneous respiratory rates and ability to follow abstract timing change with age, state, health, and individual development. Adult defaults near five or six breaths per minute may feel unnatural or create air hunger, especially for younger children.

**Product decision:** Do not expose seconds-based patterns to Little Explorers. The character demonstrates comfortable relative timing—easy inhale, slightly longer relaxed exhale—without requiring exact synchronization. Big Explorers may receive gentle visual pacing only after prototype testing. The engine records timing for validation, but the child is never scored against it.

### 3.3 Longer exhalation

**Evidence position: Plausible and common, but exact pediatric ratios are not established.**

A comfortably longer exhale can be used as a design cue, but the app must not require a child to prolong or empty the breath. A child who returns to normal breathing has completed the activity successfully.

**Product decision:** Use soft exhale imagery such as cooling cocoa, moving a feather, or lowering a wave. Never use forceful blowing, maximum duration, or “keep going until the lungs are empty.”

### 3.4 Breath holds

**Evidence position: No MVP benefit sufficient to justify added complexity or discomfort.**

Holds add cognitive load and may create air hunger, distress, or competitive behavior. They are unnecessary for the core product promise.

**Product decision:** No inhale or exhale holds anywhere in the Kids MVP, including hidden customization.

### 3.5 Rapid or activating breathing

**Evidence position: Not appropriate for the general-child MVP.**

Rapid or forceful breathing can cause lightheadedness, tingling, discomfort, and anxiety and creates avoidable safety and context risks. The adult Power Up/Bellows Lite decision does not transfer to children.

**Product decision:** No bellows breathing, breath of fire, deliberate hyperventilation, maximal breaths, or retention practices.

### 3.6 Bedtime activity

**Evidence position: Limited for breathing alone; more defensible as part of a low-stimulation routine.**

Pediatric sleep benefits reported in mindfulness research generally arise from broader programs rather than one exact breathing tempo.

**Product decision:** Keep **Moon Journey**, but position it as quiet bedtime practice. Do not claim faster sleep onset, insomnia treatment, or guaranteed sleep. End without bright celebration, rewards, or activating audio.

### 3.7 Focus and courage

**Evidence position: Insufficient for direct performance or confidence claims.**

Breathing may create a structured pause before a task, but evidence does not support promising improved attention, school performance, bravery, or executive function from a short session.

**Product decision:** Rename outcome language around preparation rather than transformation. “Feather Mission” becomes **Ready for the Next Thing**; “Brave Balloon” becomes **Try It With Me**. The close asks the child to choose one next action.

## 4. Developmental Review

### 4.1 Ages 3–6: Little Explorers

- Use one-step concrete imitation, not abstract physiology.
- Default activities last 30–60 seconds; continuation is optional.
- Demonstrate before asking the child to join.
- Essential instructions must be voiced and visually modeled.
- Offer no numeric tempo controls, breath counts, or performance feedback.
- Use two or three choices per screen.
- Adult co-use is encouraged for first use and distress contexts.
- The app never asks the child to identify a diagnosis or explain why they feel upset.

### 4.2 Ages 7–12: Big Explorers

- Use plain explanations and optional short “why this may help” content.
- Default activities last 60–120 seconds; bedtime may extend to five minutes.
- Allow narration, captions, visual-only guidance, and low-sensory presentation.
- Provide choice without turning customization into physiological experimentation.
- Reflection may ask what the child notices, but must allow “not sure” and skip.

### 4.3 Required adult role

The adult area controls profile creation, age track, activity availability, data deletion, privacy information, and any future consent. A parent gate is not proof of legal consent; if the product later collects personal information, a compliant verifiable-parental-consent design and legal review are required.

## 5. Activity Review and Required Changes

| Proposed activity | Decision | Required Version 1 change |
|---|---|---|
| Slow the Waves | Approve with testing | Comfortable relative pacing; no fixed adult cadence for ages 3–6 |
| Tiny Reset | Modify | Remove prescribed double-inhale pattern from default; use one easy breath-out plus normal breathing and adult-support choice |
| Brave Balloon | Rename/modify | Use **Try It With Me**; frame as preparation, not courage production |
| Feather Mission | Rename/modify | Use **Ready for the Next Thing**; no focus-performance claim |
| Moon Journey | Approve with claim limit | Quiet bedtime routine; no sleep or insomnia claim |
| Buddy Breaths | Approve | Make this the preferred first-use path for ages 3–6 |

### Approved initial set

1. **Slow the Waves** — settle with easy breaths
2. **Tiny Reset** — pause, one easy release, return to normal breathing
3. **Try It With Me** — prepare for something that feels hard
4. **Ready for the Next Thing** — short pause followed by one chosen action
5. **Moon Journey** — quiet bedtime wind-down
6. **Buddy Breaths** — child and caregiver practice together

## 6. Safety Controls

### 6.1 Mandatory child-facing safety behavior

- Use: **Small, easy breaths. You can stop anytime.**
- Never direct a maximal inhale, complete exhale, rapid cycle, or breath hold.
- Never say “push through,” “try harder,” “beat your score,” or “don't stop.”
- Persistent **Stop** and **Get a grown-up** controls remain available.
- Stopping produces a neutral response: **Okay. Let's let your breathing do its own thing.**
- If dizziness, tingling, pain, unusual shortness of breath, panic, or significant discomfort occurs, guidance ends immediately.
- Backgrounding, locking, or losing audio focus ends timed guidance rather than resuming invisibly.

### 6.2 Context exclusions

Do not use while:

- in water or bathing;
- walking near traffic;
- riding a bicycle or wheeled device;
- exercising or climbing;
- eating or drinking;
- doing anything that requires full attention or where dizziness could cause injury.

### 6.3 Medical boundary

Adult-facing copy:

> Kids Breathing Coach is a general wellness activity, not medical or mental-health care. If a child has breathing, heart, neurological, fainting, panic-related, developmental, or other needs that may affect comfortable breathing or use of the app, ask the child's qualified healthcare professional what is appropriate. Stop immediately if the child feels unwell or becomes more distressed.

### 6.4 Urgent boundary

The app does not coach through severe or new trouble breathing, blue or gray lips, chest pain, fainting, seizure, signs of a serious allergic reaction, altered responsiveness, or an acute safety or mental-health crisis. The adult interface directs the caregiver to local emergency services or appropriate crisis support.

## 7. Emotional and Behavioral Safety

- Validate without assigning: “Something feels hard” rather than “You are angry.”
- Never tell a child that calm is required before receiving support.
- Never use compliance language, behavior grades, mood scores, or parent-facing judgments.
- Never imply that ongoing distress means the child performed incorrectly.
- Do not ask children to disclose secrets, trauma, fears, diagnoses, family conflict, or free-text emotional narratives.
- The animated coach is a guide, not a friend who needs the child, a therapist, an authority figure, or a confidential confidant.
- Character dialogue must not create emotional dependency, guilt about leaving, or fear of losing progress.
- Rewards may acknowledge participation but never emotional outcome or breath performance.

## 8. Privacy and Consent Review

### 8.1 U.S. child-directed status

The product is intentionally directed to children under 13 and should be designed on the assumption that COPPA applies if personal information is collected online. COPPA requires clear notice and, with limited exceptions, verifiable parental consent before collection, use, or disclosure of children's personal information.

The FTC rule and guidance treat more than obvious identifiers as personal information; persistent identifiers, photos, videos, audio containing a child's voice, precise geolocation, and other data can trigger obligations.

### 8.2 MVP decision: avoid collection

Version 1 remains offline-first and does not transmit child information. It stores preferences and minimal activity history locally on the device. The MVP excludes:

- account registration;
- child email or messaging;
- advertising identifiers;
- third-party analytics or crash tools that transmit persistent identifiers;
- cloud backups controlled by the product;
- voice recordings or speech recognition;
- photos, camera access, or facial analysis;
- precise location;
- free-text child entries;
- social sharing;
- push-notification personalization based on child behavior.

Local-only design materially reduces exposure but does not replace privacy-policy, security, app-store, and legal review.

### 8.3 Data minimization

The default MVP stores only:

- nonunique local avatar selection;
- age track selected by the adult;
- accessibility and sensory settings;
- favorites;
- activity identifier, duration, and completion status;
- optional neutral response: same, a little different, not sure, or skipped.

No exact age or birth date is required. The adult can erase all data from one clearly labeled control.

### 8.4 Future networked features

Any cloud sync, analytics, school dashboard, clinician portal, account, microphone feature, or personalized notification is a new privacy architecture. It requires:

1. data inventory and purpose limitation;
2. COPPA applicability and consent analysis;
3. parent notice and control design;
4. vendor and SDK review;
5. retention and deletion rules;
6. security threat model;
7. applicable state and international child-privacy analysis;
8. app-store policy review;
9. updated child-facing explanation and testing.

## 9. UX Requirements Created by This Review

1. Create separate Little Explorer and Big Explorer scripts for every activity.
2. Default first use for ages 3–6 to Buddy Breaths with an adult.
3. Keep **Stop**, **Something Else**, and **Get a grown-up** available throughout.
4. Replace countdown timers with gentle progress for child-facing screens.
5. Do not display breathing rate, seconds, accuracy, scores, or physiological claims to children.
6. Provide a low-sensory mode without music, haptics, busy backgrounds, or character chatter.
7. End Moon Journey in a dim static state with no celebration.
8. Keep adult explanations behind the parent gate and child instructions short.
9. Allow every optional reflection to be skipped.
10. If a child stops early, do not ask why unless an adult chooses a structured safety feedback option.

## 10. Validation Plan

### 10.1 Formative testing groups

Test separately with:

- ages 3–4;
- ages 5–6;
- ages 7–9;
- ages 10–12;
- caregivers;
- children with a range of sensory, reading, attention, and motor-access needs, with appropriate consent and specialist guidance.

### 10.2 Required observations

- Can the child understand the cue without coaching?
- Does the child strain, overinhale, blow forcefully, or hold breath unintentionally?
- Can the child find Stop and Get a grown-up?
- Does the story distract from the breathing cue?
- Does animation increase stimulation or distress?
- Does the child believe there is a correct score or required emotional outcome?
- Can the caregiver understand the activity's limits and emergency boundary?

### 10.3 Promotion criteria

- At least 80% of children in each tested age band follow the core action safely without corrective coaching.
- At least 90% can stop independently or clearly indicate they want to stop.
- No moderate or severe breathing-related adverse experience occurs in supervised testing.
- At least 80% understand there is no requirement to feel calm afterward.
- Caregivers correctly understand the product is a wellness practice, not treatment or emergency support.
- Privacy inspection confirms no child data or persistent identifier leaves the device in the MVP.

Failure in one age band blocks that track even if aggregate results pass.

## 11. Claims Rules

### Allowed

- “Practice an easy breathing pause.”
- “A short activity to help your child slow down.”
- “Designed for a quiet transition before bedtime.”
- “Try one gentle tool, or choose something else.”
- “Some children find slow, comfortable breathing settling.”

### Prohibited without new evidence and regulatory review

- “Treats anxiety, panic, ADHD, autism, trauma, or insomnia”
- “Stops tantrums” or “fixes behavior”
- “Improves grades, focus, courage, or executive function”
- “Activates the vagus nerve” as an assured child outcome
- “Boosts oxygen to the brain”
- “Clinically proven” for this app or protocol
- “Works in 60 seconds”
- Any claim that shifts responsibility for persistent distress onto the child

## 12. Required Reviews Before Public Launch

- Licensed pediatric clinician review of final breathing content and contraindication language
- Child-development specialist review of scripts, choices, reward mechanics, and character behavior
- Child-privacy attorney or qualified compliance review for COPPA and launch jurisdictions
- Accessibility review with children and caregivers who use assistive features
- Security and SDK audit confirming no undisclosed network collection
- Supervised usability testing by age band
- App-store policy review at submission time

## 13. Authoritative Privacy Sources

- [FTC Children's Online Privacy Protection Rule](https://www.ftc.gov/legal-library/browse/rules/childrens-online-privacy-protection-rule-coppa)
- [FTC Children's Privacy guidance](https://www.ftc.gov/business-guidance/privacy-security/childrens-privacy)
- [FTC COPPA compliance FAQs](https://www.ftc.gov/business-guidance/resources/complying-coppa-frequently-asked-questions)
- [Electronic Code of Federal Regulations, 16 CFR Part 312](https://www.ecfr.gov/current/title-16/chapter-I/subchapter-C/part-312)

## 14. Evidence References and Limits

- Yetwin AK, et al. Pediatric HRV-biofeedback pilot literature illustrates feasibility but does not validate the proposed standalone app or all ages 3–12. [PubMed record](https://pubmed.ncbi.nlm.nih.gov/?term=Heart+Rate+Variability+biofeedback+therapy+for+children+and+adolescents)
- Pediatric mindfulness and sleep studies commonly combine breathing with movement and attention training; they support cautious program-level hypotheses rather than a precise breathing prescription. [Stanford Medicine summary](https://med.stanford.edu/news/all-news/2021/07/mindfulness-training-helps-kids-sleep-better.html)
- Adult slow-breathing evidence may inform safety hypotheses but cannot establish pediatric efficacy. See the Adult branch's BC-SPEC-002 for the adult evidence base.

The literature review is sufficient to define a conservative prototype boundary, not to certify clinical effectiveness or safety for every child.

## 15. Resulting Product Baseline

Version 1 is a character-led practice tool with six short activities, two developmental presentations, no holds, no rapid breathing, no performance scoring, and no network collection of child data. Breathing remains one choice alongside movement, grounding, stopping, and finding a trusted adult.

The next authorized artifact is **KBC-SPEC-003 — UX, Parent Gate, and Screen-State Specification**.

## 16. Change History

| Version | Date | Change |
|---|---|---|
| 0.1 | 2026-09-19 | Initial pediatric evidence, safety, development, privacy, activity, and release-gate review. |
