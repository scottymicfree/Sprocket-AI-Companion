# Security policy — Sprocket

Sprocket is an **experimental pre-release companion**. No production support window or independent security audit has been claimed.

Do not disclose keys, private file contents, exploit details or personal data in public GitHub issues. If GitHub's private vulnerability reporting is enabled here, use that channel; otherwise contact the maintainers privately.

## Intended security boundaries

- Owner-selected file/folder inspection, bounded and read-only.
- A chat message containing a file path never authorizes file access.
- Cloud transmission of selected content requires separate informed approval.
- A language model response does not authorize process execution or access to Lucy AIOS/E.M.M.A.
- No developer-wide inference secret distributed inside a client.
- Local memory must remain scoped to Sprocket and separate from unrelated apps.

These describe design requirements and prototype properties; they are not guarantees of a certified or audited v1.0 implementation.

See [v1.0 release gates](docs/V1_RELEASE_GATES.md).
