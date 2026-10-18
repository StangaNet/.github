# StangaNet — Organization defaults

Default community health files, reusable GitHub Actions, and workflow templates for every repository under [StangaNet](https://github.com/StangaNet).

GitHub applies root-level health files from this public `.github` repository to any org repo that does not define its own copy.

---

## Authorship

| What | How |
| --- | --- |
| **Library source** (`StangaNetLib.*` and related library code) | Written **by hand**, after careful research and personal development. This is the core of the organization. |
| **Code documentation** (XML comments, API prose), **README** files, and **[stanganet.github.io](https://stanganet.github.io)** | Written **with AI**. Useful for discovery and onboarding; not treated as the key deliverable of StangaNet. |

The organization profile text lives in [`profile/README.md`](./profile/README.md).

---

## Contents

| Path | Purpose |
| --- | --- |
| `profile/README.md` | Organization profile (`github.com/StangaNet`) |
| `CONTRIBUTING.md` | Contribution policy (read-only; no external PRs) |
| `CODE_OF_CONDUCT.md` | Behavior standards |
| `SECURITY.md` | Vulnerability reporting |
| `SUPPORT.md` | How to get help |
| `GOVERNANCE.md` | Decision-making model |
| `DISCUSSIONS.md` | How to use Discussions vs Issues |
| `LICENSE` / `NOTICE` | Default Apache-2.0 license materials |
| `CODEOWNERS` | Default ownership for this repo |
| `labeler.yml` | Label rules for PRs on this repo |
| `.github/ISSUE_TEMPLATE/` | Org-default issue forms |
| `.github/PULL_REQUEST_TEMPLATE.md` | Org-default PR template |
| `.github/workflows/` | **Reusable** workflows (`workflow_call`) |
| `workflow-templates/` | Starter workflows offered in “Add workflow” |

---

## Reusable workflows

Call these from a repository workflow with `secrets: inherit`.

| Workflow | For |
| --- | --- |
| `.github/workflows/dotnet-lib.yml` | .NET libraries: restore → build → test → pack → (optional) publish to GitHub Packages |
| `.github/workflows/ci.yml` | Node.js: `npm ci` → `npm test` |

Reference path (repo name is `.github`):

```text
StangaNet/.github/.github/workflows/<file>.yml@main
```

### Example — .NET library

```yaml
name: .NET CI

on:
  workflow_dispatch:
  push:
    branches: [main]
  pull_request:
    branches: [main]

concurrency:
  group: ${{ github.workflow }}-${{ github.ref }}
  cancel-in-progress: true

permissions:
  contents: read
  packages: write

jobs:
  ci:
    uses: StangaNet/.github/.github/workflows/dotnet-lib.yml@main
    with:
      library-name: 'StangaNetLib.Core'
      artifact-name: 'stanganetlib-core-nuget'
      needs-github-packages-source: true
      publish: ${{ github.event_name != 'pull_request' }}
    secrets: inherit
```

### Example — Node.js

```yaml
jobs:
  ci:
    uses: StangaNet/.github/.github/workflows/ci.yml@main
    with:
      node-version: '20'
    secrets: inherit
```

---

## License

Apache License 2.0 — see [LICENSE](./LICENSE).
