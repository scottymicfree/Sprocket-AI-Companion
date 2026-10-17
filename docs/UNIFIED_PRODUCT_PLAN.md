# Sprocket — Unified Product Plan
**Fenton Lab | Public product direction | updated 2026-10-16 | Planning document**

> Sprocket is an experimental Windows desktop companion. This document describes current prototypes and intended product directions, not a feature availability promise, public release announcement, or certification.

## Product promise
**A little fox with a big curiosity.** Sprocket is an expressive, local-first AI companion whose personality does not grant hidden access to a user's computer. Permissions remain explicit; model-generated claims are not evidence of completed actions.

## Product family
| Experience | Intended audience | Role | Public status |
| --- | --- | --- | --- |
| Sprocket Desktop | General desktop users | Animated fox, conversation, local memory, owner-selected file assistance | Experimental Windows prototype |
| Pocket Workshop | Sprocket owners | Modular official devices, animation and capability packs | In development; not a released marketplace |
| Living Worlds | Sprocket owners | Optional lightweight wallpaper scenes sharing one character identity | Design proposal |
| Sprocket Family | Families with children ages 7–12 | Guided learning, healthy companionship, guardian controls | Working development prototype in owner testing; not released |

## Shared design principles
1. **One character, one core engine:** reuse identity, animation, events, and rendering; do not run a second hidden companion in wallpaper mode.
2. **Local-first:** local Ollama and local storage are primary design choices; optional external AI requires transparent consent and appropriate controls.
3. **Explicit authority:** approved files and capabilities only; no ambient filesystem scanning, covert recording, or privilege escalation.
4. **Evidence before claims:** differentiate observed results from simulated or generated explanations.
5. **Modular growth:** verified, recoverable updates and separately governed add-ons.
6. **Resource respect:** idle wallpaper and character animations must not steal focus or obstruct other applications.
7. **Clear commercial boundaries:** application source and character artwork are not open source. Pricing and optional paid Workshop packs or content packages remain undecided; there are no plans to charge for memory. Free character evolution and motion updates are intended for existing owners.

## Sprocket Desktop
The base experience is a draggable animated fox with expressive reactions, desktop chat, local SQLite conversation history, optional Ollama/Gemini providers, and explicitly owner-selected bounded read-only file inspection. The existing 73-frame animation collection is part of prototype history, not a claim that every motion is release-certified.

## Pocket Workshop
A Fenton Lab-controlled extension surface for approved devices, behaviors, learning aids, and optional capability packs. The Mechanic's Diagnostic Device is the initial prototype concept. Independent installation, restart persistence, rollback, uninstall, entitlement rules, and signing are release gates—not completed product claims.

## Living Worlds
Planned independently managed scenes include The Laboratory and Whispering Woods. One Sprocket identity spans the companion and wallpaper presentation. Wallpaper activity becomes dormant when not relevant; scene assets and declarative events must remain lightweight and nonintrusive.

## Sprocket Family (ages 7–12)

> **Update, October 16, 2026:** a camera-free, fully offline Family prototype now exists and is in owner testing: guardian dashboard, nickname-only profiles, time limits and breaks, reading, math, science, coding, homework guidance, Sprocket's teaching reactions, and the Learning Library with parent-approved study plans. See [Sprocket Family](SPROCKET_FAMILY.md). The goals and gates below remain the plan for any release.
**Product goal:** a curious fox who supports learning and companionship without replacing parents, teachers, or human friendships.

### Child experience
- Math, reading, writing, science, and introductory coding with guided hints, worked examples, visual explanations, and understanding checks.
- Playful conversation, storytelling, discovery challenges, and character reactions without dependency-building, exclusivity, or secrecy.
- Optional explicitly selected worksheets, with constrained processing and no unrestricted file access.
- Age-adjusted explanations, breaks, and progress summaries; no claims to diagnose learning ability.

### Guardian experience
- Protected dashboard for child profiles, study-time limits, approved AI providers, file permissions, learning summaries, alerts, retention, export, and deletion.
- Default camera off and cloud off; no purchases or administrative privilege from child profiles.
- Separate child memory scopes; switching profiles invalidates old permissions and outstanding requests.
- The current prototype has no camera or biometric features. Optional future **local** face matching for profile selection only remains a separate proposal, subject to consent, spoofing tests, and deletion controls. Face matching never authorizes parent actions; camera-free selection must remain available.

### Safety and privacy gates
- Enforce policy before and after model generation, including when a local model is used; fail closed for unsafe capabilities.
- No targeted advertising to children, unnecessary collection of sensitive information, or use of child chats for model training.
- Safety responses must be age-appropriate; disclosures and escalation for genuine danger need expert review, including cases where notifying a parent may be unsafe.
- Complete COPPA/child privacy legal review, provider assessments, guardian consent where required, data retention and deletion verification, accessibility testing, and independent adversarial evaluations **before** child-facing release.

### Proposed Family phases
| Phase | Deliverable | Release criterion |
| --- | --- | --- |
| F1 | Camera-free guardian and child profiles, isolated memory, permission broker | Cross-profile and privilege-boundary tests |
| F2 | Homework advisor and basic parent dashboard | Curriculum, safety, and offline tests |
| F3 | Learning progress, alerts, retention/export/deletion | Guardian usability and privacy verification |
| F4 | Optional face recognition | Consent, liveness/spoofing, false-match, deletion tests |
| F5 | Controlled family pilot and release review | Legal, safety, accessibility, reliability and packaging sign-off |

## Release and evidence policy
Prototype tests are not equivalent to a production-ready product. The existing U1–U3 candidate receipts and Windows installer work must remain accurately dated and scoped. Open blockers include commercial art rights, real-machine endurance and accessibility, privacy/AI disclosures, independent validation, and Microsoft Store readiness. Family introduces additional child-safety gates. No Family feature should be described as shipped until verified.

## Public communication and discovery
- Main project: https://github.com/scottymicfree/Sprocket-AI-Companion
- Publisher: https://github.com/scottymicfree
- Questions and feedback: https://github.com/scottymicfree/Sprocket-AI-Companion/issues
- Microsoft Store: planned distribution channel, **no approved listing yet**.
- Add only verified official websites, demos, and social channels. Do not imply third-party affiliation.

## Next actions
1. Keep the base Sprocket release gates independent of Family research.
2. Publish a documented Family requirements and threat-model review before writing biometric code.
3. Prototype camera-free guardian and child profiles with simulated data.
4. Benchmark local tutoring quality and child-safety failure cases on realistic hardware.
5. Validate Workshop and Living Worlds as modular surfaces with measurable resource budgets.
6. Maintain dated evidence and update the public status table as each gate actually closes.

**Fenton Lab — local-first by design; evidence before claims.**
