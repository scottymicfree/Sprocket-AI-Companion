# Sprocket architecture

## Verified prototype baseline — v0.5 Workshop Reactions

| Layer | Implementation currently evidenced |
|---|---|
| Desktop | Python 3 / Tkinter, draggable transparent fox |
| Animation | 73 frames across 11 existing strips |
| Chat history | Sprocket-local SQLite |
| AI options | Offline companion, local Ollama, optional Gemini Cloud |
| File observations | User-selected, bounded read-only text/DOCX and top-level folder listing |
| Cloud submission | Separate approval before sending selected excerpts |
| External authority | No general shell execution or Lucy/E.M.M.A. control |

**Evidence:** 40/40 offline unit tests passed when the v0.5 archive was retested, October 2026. Those tests do not prove live Windows UI, provider connectivity, packaging, or commercial licensing.

## v1.0 invariants

1. **Identity and compute are separate.** Buying the companion never implies unlimited cloud inference.
2. **Observation is not execution.** The model cannot grant itself access to the file system or shell.
3. **File permission is explicit.** No chat-supplied file path authorizes a read.
4. **Document receipts are honest.** Identify source, hash, excerpt, and truncation; distinguish from memory or assumptions.
5. **User memory stays local by default.**
6. **Reply progress is truthful.** Full-buffer progressive display is not called token streaming.
7. **Original artwork provenance and licensing must be resolved** before any public distribution.

## Incomplete as of v0.5

Persistent document follow-up sessions, detailed source citations, export, Windows installer/MSIX testing, secure retail onboarding, accessible UI checks, and store compliance.

This file describes what has been observed in the prototype and the architecture intended for v1.0. It does not assert that planned functionality exists.
