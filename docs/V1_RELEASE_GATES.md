# Sprocket v1.0 release gates

**Status: NOT READY FOR SALE OR A v1.0.0 TAG.**

Updated October 11, 2026. The historical v0.5 baseline below is retained; newer U1/C1/U2/U3 development status is summarized in [Development status](DEVELOPMENT_STATUS.md).

| Gate | Verified evidence | Remaining work |
|---|---|---|
| Code / behavior baseline | v0.5: 40/40 offline Python unit tests passed | Regression suite on final source |
| Animation and chat | Manifest validates 73 sprites; offline reaction tests pass | Actual Windows focus, transparency, timing, DPI, cancellation and accessibility tests |
| Document access | Explicit read-only file and shallow folder pickers | Persistent sessions, source-cited answers, PDF/export support if advertised |
| Cloud/provider | Gemini key read from user environment; Ollama loopback mode | Provider live test, secret/storage security review, cost and consent disclosure |
| Safety | No shell authority in prototype; bounded reads | Full threat review, injection/reparse tests, independent Windows QA |
| Artwork | Original sheet hash recorded in prototype | Commercial redistribution/license approval — **BLOCKING** |
| Windows delivery | U3 isolated 0.7.4 update/recovery candidate; internal suite reported 399/400 tests passed, 1 skipped, twice | Real packaged-runtime/MSIX, visual consent dialogs, hardware interruption, anti-rollback and independent certification; **not deployed** |
| Customer release | GitHub repository exists | Privacy terms, AI reporting, support channel, Store account, certification, purchase verification |

## Do not ship until

- Real Windows smoke and endurance tests pass.
- Installer and upgrade behavior is verified and documented.
- No embedded API secrets, local conversations or private files are included.
- Artwork and dependencies are cleared for commercial distribution.
- Store, content policy, privacy, and AI response reporting requirements are implemented.
- A release receipt identifies commit SHA, package digest, test outputs, limitations, and approval.

**Keep `v1.0.0` and any public Store download announcement reserved for a verified release.**

## Work order

1. Finish Windows chat responsiveness and reaction timing.
2. Add owner-controlled persistent document sessions with evidence references.
3. Review local storage, file permissions, cloud transfers, and provider authentication.
4. Package and verify a Windows installation and updates.
5. Complete beta tests, commercial rights review, and Microsoft Store submission.
