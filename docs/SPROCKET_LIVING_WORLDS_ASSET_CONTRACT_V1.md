# Sprocket Living Worlds — Asset Contract V1 (Design Proposal)

**Status:** Proposed architecture, not implemented, tested, or available for sale.  
**Publisher:** Fenton Lab  
**Scope:** Optional Windows desktop environments, independent of the core Sprocket companion.

## Product boundaries

Sprocket remains a standalone desktop companion. Living Worlds are separately installable and removable wallpaper environments, potentially offered as paid add-ons. Pricing, entitlement terms, and availability are not yet announced. The wallpaper player should also be capable of running without launching the full companion.

**Single Presence:** Only the normal companion owns Sprocket's conversation, memory, AI provider access, permissions, and effectful actions. A Living World may render a lightweight *visual simulation* of Sprocket, but cannot create a second AI companion or write companion memory.

## Shared engine, variable assets

One reusable player loads declarative world packages. Each package declares its own number of background layers, objects, animations, effects, and event rules; no global fixed asset count is required. World-specific fox sprites need only preserve the approved Sprocket visual identity (silhouette, colors, proportions, recognizable features and movement character). They do **not** need to duplicate the full existing companion animation collection.

Assets and behaviors are referenced by stable symbolic IDs, not sheet positions or frame counts. Each manifest records frame geometry, timing, resource budgets, dependency versions, and required versus optional references. Existing character animations remain independently versioned. Missing optional animations disable only dependent events; missing required assets block activation.

## Proposed world packages

- **The Laboratory:** motherboard, RAM, GPU, cooling pump, wires and panels. When eligible and idle, the visual fox may sniff, inspect RAM, hide behind panels or wires, cause a purely cartoon spark/puff, and run back to watch the mouse. These are cosmetic events: no real hardware diagnostics or device control.
- **Whispering Woods:** forest, trees, den, lights, and a mysterious moving shadow. During eligible idle periods, the fox can search and play hide-and-seek but never catch the shadow. Typing, companion work, or active interaction suppresses distractions. On companion close, the fox may visually return to her den. The den light follows host local time when the world player is running; no full AI process is needed.
- Future worlds may contain different counts and types of assets, animations, and events.

## Presence and resource coordinator

A single coordinator decides which representation is allowed to run:

- **WORLD_ACTIVE:** Desktop is visibly in use; optional lightweight visual simulation and world events can run.
- **WORLD_DORMANT:** Desktop is obscured or user is working in another application; suspend animation and unnecessary rendering.
- **COMPANION_ACTIVE:** User invokes normal Sprocket; companion receives focus and exclusive control of real character behavior. The wallpaper must not duplicate the companion.
- **CLOSED:** Explicitly closing Sprocket does not relaunch her automatically. If independently enabled, the wallpaper may show a resting den and time-aware light without starting Sprocket.

Handle partially visible desktops, virtual desktops, multiple monitors, focus changes, fullscreen apps, display scaling, and rapid Alt+Tab. A click to open Sprocket must never wait for a decorative exit animation. Wallpaper events must never steal focus, intercept typing, cover app controls, or impede work.

## Packaging and security

Proposed `.sprocketworld` bundles contain a versioned manifest, preview, approved artwork, optional sound/effects, declarative event rules, compatibility requirements, hashes and publisher signature. No arbitrary executable scripts by default. Reject traversal paths, symlinks escaping install roots, unsupported file types, invalid signatures, and resource-budget violations. Keep world content separate from executable companion updates.

Installation and updates should be user initiated initially: stage, verify, validate, atomically activate, and preserve rollback. No automatic polling or downloads by default. Installed worlds should remain usable offline subject to final licensing policy. Preserve the original Windows wallpaper and support clean restoration/uninstall.

## Performance design

Favor optimized static images, 2D sprite layers, and event-driven scheduling rather than full game engines or second AI models. Pause animations when hidden, limit CPU/GPU/memory usage, support reduced motion, and recover gracefully after player crashes. The coordinator should be lightweight even while worlds are dormant. Quantitative budgets require real Windows measurements before release.

## Acceptance gates (not yet passed)

1. Existing Sprocket builds and asset registry remain unchanged until isolated integration passes.
2. Install, switch, update, roll back and uninstall packages of different asset counts.
3. Reject missing required assets; gracefully disable optional events with missing assets.
4. No duplicate companion, AI inference, memory writes, or permissions from the wallpaper simulation.
5. Correct visibility and presence transitions during typing, chat, Alt+Tab, fullscreen, multiple monitors and scaling changes.
6. No click interception, focus theft, blocked windows, or forced companion launch.
7. Host-local-time den light works without running the AI companion.
8. Real-machine performance, sleep/wake, crash recovery, signature verification and offline use are independently tested.
9. All commercial rights, asset provenance, installer signing and licensing are reviewed before release.

This document is a public design contract, **not** evidence of completed implementation or certification.
