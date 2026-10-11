# How Sprocket is put together

*A high-level public architecture overview — October 2026*

Sprocket is a standalone Windows desktop companion. The goal is to keep the **character**, **conversation**, **memory**, **permissions**, and **optional capabilities** separate enough that a change to one doesn't silently change the others.

## Product layers

| Layer | Current prototype or development direction |
| --- | --- |
| Character and interface | Python/Tkinter desktop companion; draggable fox with an existing 73-frame animation set and independent chat interface |
| Conversation | Controller connects to local Ollama or optionally Gemini; the on-screen companion can remain present without a cloud AI provider |
| Local memory | Sprocket-scoped SQLite conversation history and settings |
| Owner-selected observation | Bounded read-only text/DOCX and top-level folder inspection, with separate approval before sending chosen excerpts to cloud AI |
| Pocket Workshop | Current prototype contains optional UI modules; **generic independent package delivery is still being developed** |
| Release updates (U3) | Isolated 0.7.4 candidate supports signed-release checks, separate updater, data backups and recovery orchestration; not deployed or certified |

```text
                Sprocket on Windows
                        |
             Character and Chat UI
                        |
              Companion Controller
                  /           \
          Local Memory      AI Provider
            (SQLite)      /          \
                       Ollama      Gemini*
                         |
               *optional cloud processing

    Owner-selected file observation:
      permission -> bounded read -> evidence -> optional
      separate cloud-transmission approval

    Update and Workshop work:
      development verifier -> staged content -> checks
      -> activation / recovery
      (independent Workshop packages not yet verified)
```

This diagram is conceptual. It is not a claim that all planned components are production-ready.

## Boundaries we do not want to blur

1. **Identity is separate from the AI provider.** Sprocket remains the same desktop companion when the chosen model changes.
2. **Observation is not execution.** Seeing a file or folder is not permission to run commands, edit data, or control other applications.
3. **A chat path is not consent.** The owner chooses what she may inspect.
4. **A visual reaction is not proof.** An inspection animation should only reflect real application events. It must not invent a success result.
5. **User memory is local by default.** Cloud model use requires disclosure of the data and provider involved.
6. **An update is not merely a file copy.** Verified package bytes, compatibility, consent, backups and recovery must be accounted for.
7. **Workshop content must stay separate.** New devices and animations should be installable without embedding each one directly into the core app.

## What has been demonstrated

The earlier v0.5 reaction prototype recorded **40/40 offline tests passing** and verified a 73-frame art manifest. Subsequent isolated U1/C1/U2/U3 development candidates extended memory protection, capability registration, release verification and updates.

For U3 0.7.4, the internal engineering receipt reports **399 passes and 1 privilege-dependent skip, twice**. That test result is for the isolated host updater, **not** the independent Workshop animation package. The latter remains a separate experiment.

## What is still missing before release

The public release requires real Windows packaged-installer tests, UI and accessibility checks, reliable device-level interruption and recovery tests, security and dependency reviews, commercial artwork clearance, and independent certification. Pricing, future paid add-ons, and exact memory tiers are not finalized.

See [Development status](DEVELOPMENT_STATUS.md), [Release gates](V1_RELEASE_GATES.md), and [Product vision](PRODUCT_VISION.md).

---

*Fenton Lab — Small fox. Big curiosity. Evidence first.*
