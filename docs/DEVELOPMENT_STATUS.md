# Sprocket development status — updated October 16, 2026

**Project:** Sprocket AI Desktop Companion · **Publisher:** Fenton Lab  
**Public status:** Experimental development; **no commercial release or certified installer**.

This is a public product-status summary, **not** a downloadable release, source distribution, or independent certification report. Engineering source, detailed evidence, and candidate builds remain in private development.

## Release/update development

| Gate | Reported development result | Public release status |
| --- | --- | --- |
| U1 — Memory and backup protection | Development candidate accepted (0.7.1) | Not certified |
| C1 — Capability registry | Development candidate accepted (0.7.2) | Not certified |
| U2 — Authenticated release verification | Development candidate accepted (0.7.3), with cryptographic/runtime remediation outstanding | Not certified |
| U3 — Update and recovery integration | Isolated 0.7.4 candidate; internal receipt reports 399 passes and 1 privilege-dependent skip in each of two 400-test runs | **Not deployed** |
| P5 — Windows x64 installer packaging (0.7.5) | Genuine x64 installer compiled; 30,357,997 bytes; SHA-256 `426870E39F093DE4089E30068301E880E2C5D3EA3FD5A35B52F9A1D45419C2F2`; 1,089 accepted-candidate hashes matched. Installer **not executed**. | **Gate incomplete**: isolated VM lifecycle tests, signing, Workshop production trust key, and commercial compiler licensing unresolved |
| U4 — Future entitlement foundation | Not started | Not authorized |
| U5 — Real release certification | Not started | Not authorized |

The U3 prototype is designed to verify update signatures, install side-by-side, back up local user data, obtain consent, check health, and recover after interrupted or failed updates. These capabilities have development test receipts, but **isolated installer lifecycle, production-runtime, UI, hardware-interruption, anti-rollback, and independent certification work remains**. No automatic updates or network polling have been enabled.

## Parallel product tracks

Sprocket Desktop 0.7.5 packaging and release verification continue independently of Sprocket Family and Living Worlds work, which do not expand the current installer acceptance scope. See the [unified product plan](UNIFIED_PRODUCT_PLAN.md).

### Sprocket Family: update of October 16, 2026

| Milestone | Internal development result | Public status |
| --- | --- | --- |
| Guardian dashboard, nickname-only profiles, PIN, time limits and breaks | Implemented; automated and real-window tests | Owner testing; not released |
| Reading, math, science, beginner coding, guided homework help, offline conversation | Implemented with built-in, reviewed content | Owner testing; not released |
| Sprocket's teaching presence and motion variety | Implemented with existing frames; checked in real-window recordings | Owner testing; new artwork still needed |
| Learning Library: Study Builder, parent approval, Fractions Adventure (10 sessions, ages 7–9) | Implemented; 137 automated tests pass, including 12,000 generated fraction questions checked with exact arithmetic | Owner testing; not released |
| Child-safety, privacy, accessibility and educator review | Not started | Required before any pilot or release |

The Family prototype runs fully offline, with no cloud AI, analytics, advertising, purchases or camera. These results are internal development evidence, not certification. See [Sprocket Family](SPROCKET_FAMILY.md).

## Next experiment — Pocket Workshop device animation

The next planned isolated experiment is a **Mechanic's Diagnostic Device** animation pack: Sprocket operates a small electronic board while carrying out owner-authorized file or folder inspection.

The experiment must demonstrate that the new motion/device is distributed as a **separate optional Workshop update package**, not permanently inserted into the original app. The intended demonstration is:

1. Upgrade an isolated host copy using the development update mechanism.
2. Install and authenticate the external animation package.
3. Verify activation, compatibility with existing typing/walking animations, and restart persistence.
4. Verify disable/uninstall, interruption recovery, and rollback without disturbing local memories or the original artwork.

**Publicly verified status of this specific independent device demonstration:** not established by this status document. No independent device lifecycle certification is claimed here. The supplied reference artwork and sprite sheet are not included in this public repository.

This device is a visual representation of authorized inspection; it grants no new filesystem, system-command, or security privileges.

## Release policy

- Public repository: documentation, roadmap, approved announcements.
- Private repository: proprietary application source, internal candidate tests and implementation.
- No public app package, paid entitlement system, production signing keys, customer data, or commercial artwork is published here.
- Future evolution and animation improvements are intended to remain free for base owners; optional paid capabilities and specific pricing remain undecided.
- Production deployment and commercial distribution require separate owner approval and release certification.

See [repository policy](REPOSITORY_POLICY.md) and [v1.0 release gates](V1_RELEASE_GATES.md).

**P5 evidence provenance:** status above is based on the October 12 engineering handoff, not an independent execution of the installer or inspection of the local private reports. The compiler's explicit 'Non-commercial use only' status must be resolved before commercial distribution. No installation, deployment, or protected-host modification is authorized by this documentation update.

**Evidence standard:** an accepted internal development candidate is not a certified public release.
