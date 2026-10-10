# Repository policy — proprietary development, public product

**Decision:** Fenton Lab will keep Sprocket's application source private while maintaining this public repository for product documentation, community feedback, and approved release announcements.

**Current status:** Public documentation repository exists. A separate **private** development repository has not yet been created or verified. No v1.0 commercial release is approved.

## Private development repository (planned)

Use a new GitHub repository under the authorized owner account with **Private** visibility. The private repository will contain:

- Sprocket Python application and UI/animation engine source.
- Automated tests, workflows and build/packaging scripts.
- Internal release notes, technical reviews and developer work.
- Artwork only **after** the redistribution and commercial rights review is completed. Private hosting does not cure uncertain IP rights.

No live API keys, customer chat data, local databases, personal documents, credentials, or private Lucy state should be committed to *either* repository.

Suggested development defaults: protected `main`, short-lived feature branches, pull-request review, secret scanning, restricted collaborators, and private CI artifacts. Automation must not push the private tree into the public repository.

## Public product repository (this repository)

Permitted content:

- Product README, high-level architecture, privacy/security guidance and roadmap.
- Publicly appropriate issues and feature requests.
- Screenshots, demonstrations, and branding **only** after commercial rights and privacy review.
- Verified release notes, version history and a link to the approved Microsoft Store distribution.
- Optional free/demo download only if separately approved, licensed and intentionally offered.

**Not permitted:** source bundles, developer credentials, chat memory, unredacted test logs, confidential vulnerability details, source art with uncertain rights, or unrestricted downloads of the paid commercial installer.

This public repository is **not an open-source license grant**. Do not infer rights to reuse Fenton Lab code or character assets merely because the documentation is visible. Any future license must be selected and published explicitly.

## Release promotion contract

A release is promoted from private development to public announcement only after:

1. Confirmed source revision, test receipt and signed-off feature scope.
2. Real Windows installation, update and uninstall verification.
3. Privacy/secret review and commercial asset/dependency clearance.
4. Windows packaging and Store submission/certification as applicable.
5. Explicit owner approval for exactly the assets and claims being published.

The public release announcement should include a version, date, supported Windows versions, changes, known limitations and an official storefront link. Do not publish a `v1.0.0` tag or claim a certified Store release before evidence supports it.

See [release gates](V1_RELEASE_GATES.md) and [Microsoft Store plan](STORE_PLAN.md).
