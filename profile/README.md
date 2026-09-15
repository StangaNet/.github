# StangaNet

> [!IMPORTANT]
> **Most libraries are temporarily private and NuGet packages have been removed.**
> A major refactor of the entire suite is underway. New packages are being restored as they reach stability.

Personal software organization — projects built for learning, experimentation, and craft.

---

## About

StangaNet is a one-person organization maintained by a single developer.
Projects here span a range of domains: tooling, automation, web development, and system programming.

All repositories are published for public use under the Apache License 2.0.
You are free to use, modify, and distribute the code (including commercially), provided you comply with the license terms.

See the [license](#license) section for details.

---

## Documentation

The official StangaNet documentation website is available at:

**https://stanganet.github.io/**

It provides centralized documentation, guides, and technical references for StangaNet projects and libraries.

---

## Libraries

.NET libraries published to [GitHub Packages](https://github.com/orgs/StangaNet/packages).

For detailed documentation and technical references, see the
[official StangaNet documentation](https://stanganet.github.io/).

| Package                           | Description                                                                                                                                                                                                             |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| StangaNetLib.Core                 | A lightweight, zero-dependency foundation for implementing Clean Architecture and DDD in .NET, providing essential primitives like `Result<T>`, entities, domain events, specifications, guard clauses, and pagination. |
| StangaNetLib.Concurrency          |                                                                                                                                                                                                                         |
| StangaNetLib.Resilience           | Cross-cutting resilience for .NET built on `Microsoft.Extensions.Resilience` (Polly v8), executing operations through named pipelines and converting pipeline failures into `Result<T>`.                                |
| StangaNetLib.Caching              |                                                                                                                                                                                                                         |
| StangaNetLib.Storage              |                                                                                                                                                                                                                         |
| StangaNetLib.Cryptography         |                                                                                                                                                                                                                         |
| StangaNetLib.Jobs                 |                                                                                                                                                                                                                         |
| StangaNetLib.EventBus             |                                                                                                                                                                                                                         |
| StangaNetLib.SchemaRegistry       |                                                                                                                                                                                                                         |
| StangaNetLib.Auth                 |                                                                                                                                                                                                                         |
| StangaNetLib.Observability        |                                                                                                                                                                                                                         |
| StangaNetLib.RequestProtection    |                                                                                                                                                                                                                         |
| StangaNetLib.Tenancy              |                                                                                                                                                                                                                         |
| StangaNetLib.Notifications        |                                                                                                                                                                                                                         |
| StangaNetLib.FeatureFlags         |                                                                                                                                                                                                                         |
| StangaNetLib.FeatureFlags.Tenancy |                                                                                                                                                                                                                         |
| StangaNetLib.Audit                |                                                                                                                                                                                                                         |
| StangaNetLib.Gdpr                 |                                                                                                                                                                                                                         |
| StangaNetLib.ContentFlow          | A state-machine based workflow engine for content lifecycle management (Draft $\rightarrow$ Published) with background scheduling and auditing.                                                                         |
| StangaNetLib.Media                |                                                                                                                                                                                                                         |
| StangaNetLib.Search               |                                                                                                                                                                                                                         |
| StangaNetLib.Search.Elasticsearch |                                                                                                                                                                                                                         |
| StangaNetLib.Search.Meilisearch   |                                                                                                                                                                                                                         |

### 🚀 Latest Milestones

* **Sept 08, 2026**: 🎉 **Official Release of StangaNetLib.Core v1.0.0!**
* **Sept 09, 2026**: 🚀 **Official Release of StangaNetLib.ContentFlow v1.0.0!**
* **Sept 14, 2026**: 📚 **Official StangaNet documentation website launched!**
* **Sept 14, 2026**: 🛡️ **Official Release of StangaNetLib.Resilience v1.0.0!**

---

## Philosophy

* Prefer simplicity over complexity
* Build things that last
* Document as you go
* Ship when it is ready, not before

---

## License

All StangaNet projects are released under the **Apache License 2.0**.

You are free to use, modify, and distribute the code (including commercially), provided you comply with the license terms (including attribution).

Full license: [LICENSE](https://github.com/StangaNet/.github/blob/main/LICENSE)

---

## Contact

Use GitHub Issues or Discussions on the relevant repository.
For security issues, use [GitHub Private Vulnerability Reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability).
