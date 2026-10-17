# Fenton Lab's engineering approach

Fenton Lab builds distinct companion characters: Sprocket Desktop, Sprocket Family and Liberty. They share principles and engineering patterns. **They don't yet share one complete production runtime.** This page separates what exists today from what we plan.

## Principles in all three products

1. **A character's personality never gives it access.** Animations and replies don't count as permission, or as proof that something happened.
2. **Local first.** Each product keeps its data on the user's computer, in its own separate store.
3. **Explicit, visible permissions.** Files, screen content and other capabilities are used only when the user chooses them.
4. **Content and artwork must pass checks before use.** Anything that fails is rejected and never shown.
5. **Evidence before claims.** Features are tested in automated suites and real windows, and labelled working, in testing or planned.

## What exists today

| Pattern | Sprocket Desktop | Sprocket Family | Liberty |
| --- | --- | --- | --- |
| Character animation from a validated manifest | Yes | Yes. It uses an unchanged, verified copy of Sprocket Desktop's frame loader and look-direction table | Yes. Its own state machine and manifest, independent of Sprocket |
| Behaviour that reacts to what's happening | Idle behaviour and chat reactions | Teaching reactions, varied motions and pacing rules | Eight planned animation states, scheduled in code |
| Local data store with safety rules | Local memory with verified backups | Local profiles and progress, upgraded with verified backups | Its own settings and database |
| Checks on artwork and content before use | Animation frames validated at start-up | New motion art needs automated checks and owner approval; learning packages are checked data, never code | Production artwork needs format checks and an owner-approved provenance record |
| Permission-controlled capabilities | Read-only files only when the user picks them | Parent PIN guards all settings and study plans; the child edition is fully offline | No file, screen or AI access yet; consent-based screen selection is planned |
| Automated tests | Yes | Yes | Yes |

The three apps are separate codebases. Sprocket Family reuses a small, verified part of Sprocket Desktop's core; Liberty doesn't import Sprocket at all.

## Planned shared infrastructure (not built)

- **One companion runtime:** shared animation scheduling, presence and rendering that each character can use with its own art and personality.
- **One package format and trust system** for learning packages, add-ons and motion packs, with signed releases.
- **A shared permission broker** for files, screen selections and AI providers, with the same consent screens in every product.
- **Shared update and recovery,** building on Sprocket Desktop's development work.

Each of these would need its own testing and review before it reaches a released product.

See also: [Fenton Lab overview](FENTON_LAB_OVERVIEW.md) · [Liberty](LIBERTY.md) · [Sprocket Family](SPROCKET_FAMILY.md) · [Architecture of Sprocket Desktop](ARCHITECTURE.md)
