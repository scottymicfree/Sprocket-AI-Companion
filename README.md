# 🦊 Meet Sprocket

### A little fox with a big curiosity.

**An animated AI desktop companion from Fenton Lab.**

Sprocket is a small fox with a busy mind, bright blue eyes, and a habit of getting curious about whatever you're working on.

She lives on your Windows desktop, moves and reacts, chats with you, and can help look at documents **you choose to show her**. Underneath the personality is a straightforward idea: your companion should feel alive without treating your computer—or your trust—as an open invitation.

> **Development status:** Sprocket is an experimental Windows prototype. **She is not yet available for purchase or public download.** Follow along as Fenton Lab builds and verifies the first release.

---

## Small companion. Real boundaries.

| What makes Sprocket *Sprocket* | What that means today |
| --- | --- |
| 🦊 **A character, not just a chat box** | A draggable animated desktop fox with expressive reactions and an existing 73-frame animation collection. |
| 💬 **Someone to talk to** | A desktop chat experience with local Ollama or an optional Gemini provider. |
| 🧠 **A memory that lives with you** | Conversation history stored locally in Sprocket's SQLite data store. |
| 📁 **Curious, but asks first** | Owner-selected, bounded, read-only file and folder inspection; cloud submission of selected document content requires separate approval. |
| 🧰 **Built to grow** | Pocket Workshop is an in-development system for optional capabilities, devices and animations—not a released add-on store. |
| 🔍 **Evidence matters** | We design Sprocket to distinguish actual observations from AI-generated explanations. That principle is still being tested and refined. |

She is intended to be enjoyable when you're simply chatting, and useful when you want a hand looking at something on your desktop. She isn't marketed as an autonomous operator or an all-access administrator.

## The idea behind her

**Personality should be expressive. Permissions should be precise.**

Sprocket's animations give her character; they don't give her extra authority. A model saying *“I checked the file”* isn't proof that anything was opened. A file path in a chat isn't permission to read it. And connecting an optional cloud model shouldn't silently turn local files into cloud data.

That's the standard we're working toward: a companion that feels personal **and** respects what belongs to you.

## Meet Pocket Workshop — in development

Sprocket's planned **Pocket Workshop** is where she may gain optional tools, devices, and other capabilities as Fenton Lab develops them. The aim is to update her through authenticated, recoverable packages—not by permanently wiring every new feature into her original application.

Our first test concept is **the Mechanic's Diagnostic Device**: Sprocket opens a tiny circuit-board tool, connects probes, scans an owner-approved file or folder, and reacts to the real result.

**This device pack is a development prototype, not an available product.** The current experiment must still prove independent package installation, activation, restart persistence, uninstall, and rollback.

Regular evolution improvements and character-motion updates are planned to remain free for existing owners. Optional paid capabilities, memory tiers, and pricing have **not** been finalized.

## Where development stands

| Milestone | Status |
| --- | --- |
| Animated Windows companion, chat and local memory | Working prototype; release testing still needed |
| Owner-selected read-only file inspection | Prototype implemented; further security and usability testing needed |
| Update and recovery system (U3 0.7.4) | **Isolated candidate**; internal suite reported 399 passes and 1 skipped, twice |
| First independently installable Workshop device | **In development; not yet verified** |
| Windows installer, commercial rights, real-machine and independent certification | **Not complete** |
| Public release | **Not announced** |

The U3 test count describes automated development testing, **not** public release certification. No production deployment, automatic updater, or network polling has been enabled as part of that candidate.

Read the [detailed development status](docs/DEVELOPMENT_STATUS.md) and [release requirements](docs/V1_RELEASE_GATES.md) for specifics.

## Questions people ask

**Can I install Sprocket today?**  
Not through this public repository. The application is still in private development; there is no approved public installer or store listing.

**Does she work without the cloud?**  
Her desktop companion can run without a cloud model, and development supports a local Ollama option. AI quality and features depend on the provider you choose; optional cloud models can involve third-party data processing and costs.

**Does she read all my files?**  
No. The current document-reading workflow is built around explicit owner-selected, bounded read-only access. Further privacy and security validation remains part of release work.

**Will updates change the companion I've grown attached to?**  
The design goal is to preserve Sprocket's identity, memory and existing motions through verified updates, with backup and recovery checks. That protection must pass real-world certification before release.

**Is the code open source?**  
No. This is Fenton Lab's public product and progress page. Sprocket's application source and commercial artwork are not licensed for public reuse by this repository.

More in the [product FAQ](docs/FAQ.md).

## Follow the build

This is the first Fenton Lab product we're introducing publicly, and we're building it in the open where we can—showing progress **without presenting unfinished work as a shipped feature**.

- [Development status](docs/DEVELOPMENT_STATUS.md) — what has passed and what is still blocked
- [What we're building](docs/PRODUCT_VISION.md) — Sprocket's personality, promises, and Pocket Workshop direction
- [Product FAQ](docs/FAQ.md) — availability, privacy, updates, and ownership
- [Architecture](docs/ARCHITECTURE.md) — technical design boundaries
- [Security policy](SECURITY.md) — how to raise security concerns safely
- [Repository policy](docs/REPOSITORY_POLICY.md) — why source and artwork stay private

**Fenton Lab** · Local-first by design · Evidence before claims

---

*Small fox. Big curiosity. Your computer, your call.* 🦊
