# StangaNet

> [!IMPORTANT]
> **Most libraries are temporarily private and NuGet packages have been removed.**
> A major refactor of the suite is underway. Packages are restored as they reach stability.

Personal software organization — projects built for learning, experimentation, and craft.

---

## About

StangaNet is a one-person organization. Projects span tooling, automation, web development, and system programming.

Repositories are published under the Apache License 2.0. You may use, modify, and distribute the code (including commercially), provided you comply with the license terms.

---

## Documentation

Official docs: **https://stanganet.github.io/**

Centralized guides and technical references for StangaNet projects. Documentation is AI-assisted and always reviewed manually before publication; updates may lag releases by a few days.

---

## Libraries

.NET libraries published to [GitHub Packages](https://github.com/orgs/StangaNet/packages).

| Package | Description |
| --- | --- |
| [StangaNetLib.Core](https://github.com/StangaNet/StangaNetLib.Core) | Clean Architecture / DDD primitives for .NET: `Result<T>`, entities, domain events, specifications, guards, pagination. |
| [StangaNetLib.Concurrency](https://github.com/StangaNet/StangaNetLib.Concurrency) | Keyed locks, throttling, work queues, debouncing, and atomic counters. |
| [StangaNetLib.Resilience](https://github.com/StangaNet/StangaNetLib.Resilience) | Named Polly / `Microsoft.Extensions.Resilience` pipelines that surface failures as `Result<T>`. |
| [StangaNetLib.Caching](https://github.com/StangaNet/StangaNetLib.Caching) | InMemory / Redis cache and distributed locks, cache-aside with thundering-herd protection. |
| [StangaNetLib.Storage](https://github.com/StangaNet/StangaNetLib.Storage) | Blob storage (Local, S3, Azure Blob) with streaming, pre-signed URLs, and `Result<T>`. |
| [StangaNetLib.Auth](https://github.com/StangaNet/StangaNetLib.Auth) | JWT auth with refresh-token rotation, BCrypt, cache-backed revocation, and Auth0 integration. |
| [StangaNetLib.Observability](https://github.com/StangaNet/StangaNetLib.Observability) | ASP.NET Core middleware: correlation IDs, request logging, ProblemDetails, ETag, security headers, PII masking. |
| [StangaNetLib.Gdpr](https://github.com/StangaNet/StangaNetLib.Gdpr) | Consent, DSAR, objection/restriction, breach audit, and AES-GCM pseudonymization building blocks. |
| [StangaNetLib.ContentFlow](https://github.com/StangaNet/StangaNetLib.ContentFlow) | Content lifecycle state machine (Draft → Published) with scheduling and audit trail. |
| [StangaNetLib.Media](https://github.com/StangaNet/StangaNetLib.Media) | Image variants (JPEG/WebP), magic-byte validation, and photo storage (local / Azure / Storage-backed). |

Additional libraries are in progress and will be listed here as they stabilize.

---

## Philosophy

- Prefer simplicity over complexity
- Build things that last
- Document as you go
- Ship when it is ready, not before

---

## License

All StangaNet projects use the **Apache License 2.0** unless a repository states otherwise.

Full license: https://github.com/StangaNet/.github/blob/main/LICENSE

---

## Contact

Use GitHub Issues or Discussions on the relevant repository.  
For security issues, use [GitHub Private Vulnerability Reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability).
