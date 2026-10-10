# 🦊 Sprocket — AI Desktop Companion

### A little fox with a big curiosity.

**Developed at Fenton Lab**

Sprocket is an experimental, local-first AI desktop companion designed to make artificial intelligence more interactive, accessible, and accountable.

What started as a custom animated pet has evolved into an independent Windows application with a conversational interface, multiple AI providers, local memory, and permission-controlled document inspection.

Sprocket isn't intended to be just another chatbot.

The goal is to build a companion that understands the difference between **what it knows, what it assumes, and what it can actually verify.**

## Current Features

- 🦊 **Animated Desktop Companion** — Custom pixel-art fox with 73 animation frames.
- 💬 **Interactive Chat** — Independent desktop conversation interface.
- 🧠 **Multiple AI Providers** — Local Ollama models or Google Gemini API.
- 💾 **Local Memory** — Persistent conversation history.
- 📄 **Document Reading** — Owner-selected, read-only document inspection, including Word documents.
- 🔐 **Permission Controls** — Approval before transmitting selected document text to a cloud AI provider.
- 🧾 **Evidence Awareness** — Designed to distinguish observed file content from model-generated assumptions.
- 🖥️ **Windows Integration** — Draggable desktop character and lightweight Python interface.

## Architecture

```text
Sprocket Desktop Companion
          |
     Chat Interface
          |
   Companion Controller
          |
    +-----+------+
    |            |
Local Memory   AI Provider
    |            |
  SQLite      +-- Ollama
              |
              +-- Gemini API

Owner-approved
Document Reader
```

The desktop companion remains usable without an active AI provider. Cloud reasoning is optional.

## Design Principles

**1. Local-first by default**

Keep companion state, animation, and saved memory on the owner's device.

**2. Evidence over assumption**

A model's statement is not proof that a file was accessed or an action was completed.

**3. Permission before access**

Documents are selected by the owner. Cloud transmission requires explicit authorization.

**4. AI reasoning is not execution authority**

Sprocket does not automatically receive command execution, unrestricted filesystem access, or Lucy AIOS governance permissions.

**5. One companion, multiple providers**

The AI reasoning provider can change without replacing the companion's identity or appearance.

## Relationship to Lucy AIOS

Sprocket is being developed as an independent experimental companion within the broader Fenton Lab ecosystem.

Future integration may allow Sprocket to display approved task activity from Lucy AIOS and its Coding Studio.

Lucy and E.M.M.A. retain their own governance and verification boundaries.

Sprocket is not a replacement for E.M.M.A. and does not independently authorize system operations.

## Roadmap

- [x] Standalone Windows companion
- [x] Animated desktop character
- [x] Local Ollama integration
- [x] Gemini API integration
- [x] Persistent local chat history
- [x] Initial permission-controlled document reading
- [ ] Persistent, revocable document sessions
- [ ] Source-level evidence citations
- [ ] Stronger coding evaluations
- [ ] Owner-approved project inspection
- [ ] Browser-based companion
- [ ] Optional secure cloud hosting
- [ ] Governed Lucy Coding Studio integration

## Project Status

**Experimental prototype — Active development**

Sprocket currently demonstrates desktop animation, AI chat, and basic document-reading workflows.

The application is not yet a fully autonomous coding agent, a security-audited production system, or a verified replacement for a governed execution platform.

Windows compatibility, cloud quotas, security protections, and long-running reliability require continued testing.

## Technology

- Python
- Tkinter
- SQLite
- Ollama REST API
- Google Gemini API
- Windows desktop environment

## Security and Privacy

Sprocket is designed to minimize unnecessary access.

Do not commit API keys, private conversation databases, credentials, personal documents, or production Lucy state to this repository.

Cloud model use may transmit authorized conversation or document content to an external provider.

## Repository arrangement

The source code and internal development work for Sprocket are intended to remain in a **separate private repository**. This public repository is for product documentation, public feedback, and approved release announcements. It does not distribute the paid Windows app or imply an open-source license.

Read the [repository policy — proprietary development, public product](docs/REPOSITORY_POLICY.md) and [v1.0 release requirements](docs/V1_RELEASE_GATES.md).

## Development

Created and developed at **Fenton Lab** as part of ongoing experimentation with local-first artificial intelligence, governed agents, and human-centered interfaces.

**Build in public. Verify before claiming success.**

---

*Small fox. Big questions. Evidence first.* 🦊
