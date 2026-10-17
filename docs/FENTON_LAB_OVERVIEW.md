# Fenton Lab: overview

*For partners, software distributors, journalists, interested investors and future customers. Updated October 16, 2026.*

> This is a product and business overview. It is not an offer of securities or an investment solicitation.

## Mission

Fenton Lab develops character-driven software companions that combine expressive interaction with practical functionality and user-controlled permissions.

We think software companions should be good company and genuinely useful, while staying within clear limits that the user sets and can see.

## Products

| Product | What it is | Stage |
| --- | --- | --- |
| **Sprocket Desktop** | An animated fox companion for Windows. She chats through a local AI model, keeps a local memory, and helps with files you choose to show her | Pre-release; working development builds; not yet available |
| **Sprocket Family** | A learning companion for ages 7–12. Parents control profiles, time limits and study plans; the child learns reading, math, science and beginner coding with Sprocket, entirely offline | Working development prototype in owner testing; not released |
| **Liberty, The Desktop Eagle** | A separate eagle companion. Patriot Lens (planned) would research, explain, improve or teach about a part of the screen the user deliberately selects | Early development. Milestone 0.2 has a working desktop window and animation system with placeholder graphics. AI chat, screen research and final artwork are not built. [Details](LIBERTY.md) |

## How we build

Sprocket Desktop remains our first release priority. The products are at different stages and are separate codebases today. [Engineering approach](ENGINEERING_APPROACH.md)

- **Shared patterns now, a shared engine later.** Sprocket Family reuses a verified part of Sprocket Desktop's animation core. Liberty is a separate codebase built on the same principles and patterns. A single shared companion runtime is planned but not built. Each character keeps its own identity, art, personality and data.
- **Characters stay separate from abilities.** An animation is just an animation. Capabilities such as reading a file need explicit permission, and a character's reply is never treated as proof that something happened.
- **Content and capabilities come as checked modules.** Sprocket Family's Learning Library adds parent-approved learning packages that contain data only, never code. Sprocket Desktop's planned Pocket Workshop takes the same approach for optional add-ons.
- **Data stays local.** Conversations, notes and learning records stay on the user's computer. The child edition runs fully offline, with no cloud AI, analytics, ads or purchases.
- **Evidence before claims.** Every milestone is backed by automated tests and real-window checks. We label features as working, in testing or planned, and we don't call internal tests certification.

## Commercial direction

- **Sprocket Desktop:** a planned one-time purchase.
- **Free character and motion updates** for existing owners.
- **Possible optional extras later:** paid capabilities, and educational content packages for Sprocket Family.
- **Exact pricing, terms and availability are not set.**

## Status

- **No product is released yet.** The first Windows release is in preparation. It depends on:
  - commercial clearance of the character artwork;
  - a verified, signed installer tested on clean machines;
  - Microsoft Store requirements;
  - a published privacy policy and support contact;
  - for Sprocket Family, child-safety and privacy reviews.
- **No release date has been announced.**
- **Fenton Lab has no customers, revenue, partnerships or outside investment to report.**

## Contact

- **Public project:** [github.com/scottymicfree/Sprocket-AI-Companion](https://github.com/scottymicfree/Sprocket-AI-Companion)
- **General questions:** [GitHub Issues](https://github.com/scottymicfree/Sprocket-AI-Companion/issues)
- **Business and press contact:** a dedicated address will be published here once it is set up.

See also the [press and partner overview](PRESS_AND_PARTNER_OVERVIEW.md).
