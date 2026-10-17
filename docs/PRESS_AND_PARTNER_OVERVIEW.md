# Press and partner overview: Fenton Lab and Sprocket

*Updated October 16, 2026. A preview for journalists, partners and interested investors. It is not an offer of securities.*

## In one paragraph

Fenton Lab is building **Sprocket**, an animated fox who lives on the Windows desktop and is designed to be both good company and useful, without taking more access than the user gives her. Alongside her, **Sprocket Family** brings the same character to children aged 7–12. It is an offline learning companion with parent-controlled profiles, time limits and study plans. Both are working development builds and are being prepared for release. **Neither is available yet.**

## The problem

- **Assistants tend toward one of two extremes.** Most are either a plain chat box with no personality, or an assistant that asks for broad access to your computer and your data.
- **Families face a similar choice.** Many learning apps rely on ads, accounts and cloud services, which is a poor fit for young children and the parents responsible for them.

## Our approach

- **A character worth having around.** Sprocket's animations, reactions and timing make her feel present. In Sprocket Family she takes part in the lesson: she looks at the question, encourages after a mistake and celebrates real progress.
- **Personality never means more permission.** She reads only the files you pick. A typed file path is never permission, and a confident reply is never treated as proof that something was done.
- **Local first.** Memory, notes and learning records stay on the user's computer. The child edition needs no internet at all.
- **Parents in charge.** Parents choose which subjects each child can use, set daily limits and breaks, and approve every study plan before a child sees it. Progress is shown skill by skill.

## Why expressive companions may be commercially interesting

These are our working assumptions, not results:
- people respond to software with a personality;
- a companion that is careful with permissions and privacy can earn trust that general-purpose AI tools struggle to earn;
- a reusable companion engine lets one investment support several characters and editions (Sprocket Desktop, Sprocket Family and Liberty), plus add-on packages, without rebuilding each one.

We haven't yet tested these with paying customers.

## What exists today

- **Sprocket Desktop (pre-release build 0.7.5):**
  - the animated desktop character;
  - the Comm-Link chat window, using a local AI model, with an Offline mode that makes no AI calls;
  - local memory with verified safety backups;
  - read-only help with a file or folder the user chooses;
  - a verified update and recovery system, tested only on an isolated development copy.
- **Sprocket Family (development prototype, in owner testing):**
  - **Parent controls:** parent PIN, child profiles that use nicknames only, daily limits and required breaks.
  - **Learning:** reading, math, science, beginner coding and guided homework help, all with offline content.
  - **Sprocket in the lesson:** context-aware teaching reactions.
  - **Learning Library:** Study Builder, parent approval, and the first package, *Fractions Adventure* (10 sessions for ages 7–9). Its practice questions are made on the computer from reviewed question types and checked with exact arithmetic.

Screenshots of the working interfaces are in the [README](../README.md#screenshots). The character artwork is still under rights review, so the published images show the app's screens only.

## Verified engineering milestones

These are internal development evidence from Fenton Lab's own automated tests, **not independent certification**.

| Area | Result |
| --- | --- |
| Desktop update and recovery system (isolated development copy) | 399 of 400 automated tests passed, 1 skipped, in each of two runs |
| Desktop 0.7.5 build | All 133 files match the accepted build's recorded fingerprints |
| Sprocket Family with Learning Library (Oct 16, 2026) | 137 automated tests pass, including real-window tests of the parent and child journeys run with networking blocked |
| Fractions question generation | 12,000 generated questions checked: each picture matches its fraction, exactly one option is right, and no wrong option equals the answer |
| Family resource use | About 2% of one CPU core while a child works on a question, with Sprocket animating (one development PC) |

## How we plan to make money

- **Sprocket Desktop:** a one-time purchase.
- **Free character and motion updates** for existing owners.
- **Possibly later:** optional paid capabilities, and educational content packages for Sprocket Family.

**Prices, terms and dates are not set.**

## Roadmap

These are plans, not commitments:
1. **First Windows release of Sprocket Desktop,** once the remaining release requirements below are met.
2. **Sprocket Family:** owner testing, then educator, child-safety, privacy and accessibility reviews before any pilot.
3. **More Learning Library packages and subjects.**
4. **Pocket Workshop add-ons and new Sprocket motions,** once the new artwork is cleared.
5. **Liberty,** the bald eagle companion.

## What could hold up release

- **Artwork rights:** commercial clearance of the current character artwork is open. New artwork may be needed.
- **Packaging:** a signed, verified Windows installer tested on clean machines; installer tooling licensing; Microsoft Store requirements.
- **Policies and support:** a published privacy policy, a support contact, and AI-response reporting where required.
- **Sprocket Family:** child-safety, privacy and accessibility reviews and an educator review of the content. These are not started, and Sprocket Family is not certified as child-safe.
- **Business:** setting up the business, which is a separate step from being cleared to distribute the software.

## Contact

- **Public project and updates:** [github.com/scottymicfree/Sprocket-AI-Companion](https://github.com/scottymicfree/Sprocket-AI-Companion)
- **Questions and feedback:** [GitHub Issues](https://github.com/scottymicfree/Sprocket-AI-Companion/issues)
- **Press and business enquiries:** a dedicated contact will be published once it is confirmed. Until then, please use GitHub Issues, and don't include personal information.

See also the [Fenton Lab overview](FENTON_LAB_OVERVIEW.md).
