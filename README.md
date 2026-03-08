# StangaNet — Community Health Files

This repository contains organization-wide defaults for all **StangaNet** projects on GitHub.

Files stored here are automatically applied to any repository in the organization that does not define its own equivalent file.

---

## What's in here

| File / Folder | Purpose |
| --- | --- |
| `profile/README.md` | Public organization profile (shown on github.com/StangaNet) |
| `CONTRIBUTING.md` | Contribution guidelines (read-only, no external PRs) |
| `CODE_OF_CONDUCT.md` | Community behavior standards |
| `SECURITY.md` | Vulnerability reporting process |
| `SUPPORT.md` | How to get help |
| `GOVERNANCE.md` | Decision-making structure |
| `LICENSE` | Default license (StangaNet Source-Available License v1.0) |
| `FUNDING.yml` | Sponsorship/donation links |
| `CODEOWNERS` | Code ownership assignments |
| `ISSUE_TEMPLATE/` | Structured templates for bugs and feature requests |
| `PULL_REQUEST_TEMPLATE.md` | Template shown when opening a pull request |
| `workflows/` | Shared reusable GitHub Actions workflows |
| `workflow-templates/` | Starter workflow templates for org repositories |

---

## Reusable Workflows

Workflows in `workflows/` are called from individual repository pipelines via `workflow_call`.

| Workflow | Use for |
| --- | --- |
| `workflows/dotnet-lib.yml` | .NET library repositories (build → test → pack → publish to GitHub Packages) |
| `workflows/ci.yml` | Node.js repositories (install → test) |

### Example — .NET library

```yaml
jobs:
  ci:
    uses: StangaNet/.github/workflows/dotnet-lib.yml@main
    with:
      library-name: 'StangaNetLib.Auth'
      artifact-name: 'stanganetlib-auth-nuget'
      needs-github-packages-source: true
```

### Example — Node.js

```yaml
jobs:
  ci:
    uses: StangaNet/.github/workflows/ci.yml@main
    with:
      node-version: '20'
```

---

## License

All StangaNet projects are published under the **StangaNet Source-Available License v1.0** unless stated otherwise in the individual repository.

You may view and use the code for personal non-commercial purposes with mandatory attribution. Modification, redistribution, and commercial use are not permitted.

---

## References

- [GitHub: Creating a default community health file](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [GitHub: Customizing your organization's profile](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/customizing-your-organizations-profile)
- [GitHub: Reusable workflows](https://docs.github.com/en/actions/sharing-automations/reusing-workflows)
