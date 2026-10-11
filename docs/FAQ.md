# Sprocket — Frequently asked questions

*Current as of October 11, 2026. This is a development FAQ, not a set of finalized commercial terms.*

## What is Sprocket?

Sprocket is an animated, conversational fox companion for Windows, developed at Fenton Lab. Her existing prototype combines expressive desktop motions, chat, local conversation history, optional AI providers, and owner-selected read-only document inspection.

## Can I download or buy her now?

Not from this public GitHub repository. There is currently **no authorized public installer, storefront listing, commercial launch date, or final price**.

## Is Sprocket a standalone app or part of Lucy?

She is a separate companion. Lucy AIOS and E.M.M.A. have distinct governance and execution responsibilities. Sprocket does not automatically gain access to them.

## Does Sprocket need internet access?

Her animated desktop experience does not depend on a cloud model. She has a local Ollama integration for AI responses and an optional Gemini integration that can use an internet connection. Actual capability, performance and cost depend on the provider and configuration. Not every AI feature is guaranteed to work fully offline.

## Where is memory kept?

The working prototype uses a local SQLite conversation store. Memory limits and upgrade options are still being determined. Backups, retention disclosures, recovery and deletion semantics are subjects of the current release-verification work. We will not advertise unlimited memory.

## Can Sprocket browse my folders or read personal files without asking?

The current file-inspection design uses explicit owner selection and bounded, read-only inspection. The companion isn't meant to grant herself unrestricted filesystem or shell access. A chat message containing a path is not authorization to open it.

## Will my files be sent to an AI provider?

Optional cloud providers may process content you authorize them to receive. The prototype's document workflow requires separate approval before sending selected document text to a cloud AI provider. Privacy disclosures, provider behavior and real release packaging still require verification before launch.

## What is Pocket Workshop?

Pocket Workshop is a proposed official upgrade system for optional devices, character motions, and capabilities. It is **not yet a published catalog or completed external add-on installer**.

## What is the mechanic's diagnostic device?

It is the first proposed Workshop animation-package test. Sprocket will visually unpack a small electronics board, connect probes, scan during an authorized inspection, and react to the outcome. It is a character animation, **not an exploit tool or permission bypass**. Independent package installation and rollback are not yet certified.

## Do I have to buy Sprocket again every time she improves?

The intended ownership model includes free evolution improvements and character animation updates for existing base owners. Optional capabilities and larger memory tiers could be offered separately in the future. Specific paid features, prices and final terms remain undecided.

## Is Sprocket open source?

No. The public repository contains approved product documentation and development updates; it does not license the proprietary application source or character artwork for reuse.

## What is the latest tested version?

An **isolated 0.7.4 U3 development candidate** has a private internal receipt reporting 399 passed, 1 skipped, in each of two 400-test suite runs. This is not a finished or deployed consumer product. See [development status](DEVELOPMENT_STATUS.md) for the current gate matrix.

## Can I use Sprocket as a fully autonomous coding or security agent?

No such production capability is being claimed. Her planned diagnostic device provides visual feedback; any actual file inspection must use separately authorized, bounded operations.

## How do I report a security concern or follow progress?

Please read the [security policy](../SECURITY.md) before sharing anything sensitive; do not place exploit instructions, personal data, API keys or private files in public issues. For normal product feedback, follow this repository and its public issue tracker when available.

---

[Back to Sprocket](../README.md) · [Product vision](PRODUCT_VISION.md) · [Release gates](V1_RELEASE_GATES.md)
