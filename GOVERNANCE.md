# Governance

## Overview

StangaNet is a personal organization with a single maintainer.
Technical, directional, and operational decisions are made by that maintainer.

**Library code** is hand-written following research and personal development — that is the organization’s primary craft.
**Documentation** (in-code docs, READMEs, and [stanganet.github.io](https://stanganet.github.io)) is produced with AI assistance and is not treated as the core of the organization.

## Roles

| Role | Who | Responsibilities |
| --- | --- | --- |
| Maintainer | Organization owner (`stangherlin-enrico`) | Releases, code ownership, all decisions |

There are no external maintainers, committers, or governance committees.
A `maintainers` team may be created for future structure; currently it contains only the owner.

## Technical controls

All `StangaNetLib.*` repositories have an active ruleset on `main`:

- Require a pull request before merging
- At least 1 approving review
- Dismiss stale reviews when new commits are pushed
- Block force pushes
- Block branch deletions

Wiki is disabled on all repositories.
Discussions are enabled **only** on the `.github` repository.

## Decision making

Changes are decided by the maintainer. There is no voting process.

Community feedback via Issues and Discussions (on `.github`) is welcome but does not imply a commitment to act on it.

## Contributions

External pull requests are **not** accepted. Repositories are published for reference and learning.

See [CONTRIBUTING.md](./CONTRIBUTING.md).

## Licensing

Default license: **Apache License 2.0**. Individual repositories may document exceptions in their own `LICENSE` file.
See [LICENSE](./LICENSE).
