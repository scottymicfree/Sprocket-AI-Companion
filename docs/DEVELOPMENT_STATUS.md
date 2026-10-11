# Sprocket development status — October 11, 2026

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
| U4 — Future entitlement foundation | Not started | Not authorized |
| U5 — Real release certification | Not started | Not authorized |

The U3 prototype is designed to verify update signatures, install side-by-side, back up local user data, obtain consent, check health, and recover after interrupted or failed updates. These capabilities have development test receipts, but **real installer, production-runtime, UI, hardware-interruption, anti-rollback, and independent certification work remains**. No automatic updates or network polling have been enabled.

## Next experiment — Pocket Workshop device animation

The next planned isolated experiment is a **Mechanic's Diagnostic Device** animation pack: Sprocket operates a small electronic board while carrying out owner-authorized file or folder inspection.

The experiment must demonstrate that the new motion/device is distributed as a **separate optional Workshop update package**, not permanently inserted into the original app. The intended demonstration is:

1. Upgrade an isolated host copy using the development update mechanism.
2. Install and authenticate the external animation package.
3. Verify activation, compatibility with existing typing/walking animations, and restart persistence.
4. Verify disable/uninstall, interruption recovery, and rollback without disturbing local memories or the original artwork.

**Current result:** planned / assigned for development. The independent add-on installation, new animation playback, and recovery tests have **not yet been reported as passing**. The supplied reference artwork and sprite sheet are not included in this public repository.

This device is a visual representation of authorized inspection; it grants no new filesystem, system-command, or security privileges.

## Release policy

- Public repository: documentation, roadmap, approved announcements.
- Private repository: proprietary application source, internal candidate tests and implementation.
- No public app package, paid entitlement system, production signing keys, customer data, or commercial artwork is published here.
- Future evolution and animation improvements are intended to remain free for base owners; optional paid capabilities and specific pricing remain undecided.
- Production deployment and commercial distribution require separate owner approval and release certification.

See [repository policy](REPOSITORY_POLICY.md) and [v1.0 release gates](V1_RELEASE_GATES.md).

**Evidence standard:** an accepted internal development candidate is not a certified public release.
