# StangaNet

Personal software organization — projects built for learning, experimentation, and craft.

---

## About

StangaNet is a one-person organization. Projects span tooling, automation, web development, and system programming.

Repositories are published under the Apache License 2.0. You may use, modify, and distribute the code (including commercially), provided you comply with the license terms.

---

## How things are built

**Libraries are the craft.** Every line of library source code is written by hand, after careful research and personal development — design, implementation, tests, and packaging included. That work is the point of StangaNet.

**Documentation is support material.** XML/API comments in the libraries, repository README files, and the documentation site **[stanganet.github.io](https://stanganet.github.io)** are produced with AI assistance. They are useful for discovery and onboarding, but they are **not** treated as the core of the organization: the libraries are. Docs may lag releases by a few days.

---

## Documentation

Official docs: **https://stanganet.github.io/**

Centralized guides and technical references for the StangaNetLib suite (and related projects). Authored with AI as described above.

---

## Libraries

.NET libraries (`net8.0` / `net9.0` / `net10.0`) published to [GitHub Packages](https://github.com/orgs/StangaNet/packages). Shared CI lives in [StangaNet/.github](https://github.com/StangaNet/.github).

Hand-written source; AI-assisted docs and READMEs (see [How things are built](#how-things-are-built)).

### Foundation

| Package | Description |
| --- | --- |
| [StangaNetLib.Core](https://github.com/StangaNet/StangaNetLib.Core) | Clean Architecture / DDD primitives: `Result<T>`, entities, domain events, specifications, guards, pagination. |
| [StangaNetLib.Concurrency](https://github.com/StangaNet/StangaNetLib.Concurrency) | Keyed locks, throttling, work queues, debouncing, and atomic counters. |
| [StangaNetLib.Resilience](https://github.com/StangaNet/StangaNetLib.Resilience) | Named Polly / `Microsoft.Extensions.Resilience` pipelines that surface failures as `Result<T>`. |

### Platform

| Package | Description |
| --- | --- |
| [StangaNetLib.Caching](https://github.com/StangaNet/StangaNetLib.Caching) | InMemory / Redis cache and distributed locks, cache-aside with thundering-herd protection. |
| [StangaNetLib.Storage](https://github.com/StangaNet/StangaNetLib.Storage) | Blob storage (Local, S3, Azure Blob) with streaming, pre-signed URLs, and `Result<T>`. |
| [StangaNetLib.Media](https://github.com/StangaNet/StangaNetLib.Media) | Image variants (JPEG/WebP), magic-byte validation, and photo storage. |
| [StangaNetLib.Auth](https://github.com/StangaNet/StangaNetLib.Auth) | JWT auth with refresh-token rotation, cache-backed revocation, and Auth0 integration. |
| [StangaNetLib.Observability](https://github.com/StangaNet/StangaNetLib.Observability) | Correlation IDs, request logging, ProblemDetails, ETag, security headers, PII masking. |
| [StangaNetLib.Cryptography](https://github.com/StangaNet/StangaNetLib.Cryptography) | Hashing, KDF, HMAC, signatures, and secure token helpers. |
| [StangaNetLib.Tenancy](https://github.com/StangaNet/StangaNetLib.Tenancy) | Tenant resolve (header / host / path / claims) and store abstractions. |
| [StangaNetLib.FeatureFlags](https://github.com/StangaNet/StangaNetLib.FeatureFlags) | Feature flags with percentage rollout, tenant allow-lists, and live reload. |
| [StangaNetLib.Jobs](https://github.com/StangaNet/StangaNetLib.Jobs) | Background jobs — in-memory backend and Hangfire adapter. |
| [StangaNetLib.RequestProtection](https://github.com/StangaNet/StangaNetLib.RequestProtection) | Rate limiting and idempotency (Caching-backed). |
| [StangaNetLib.SchemaRegistry](https://github.com/StangaNet/StangaNetLib.SchemaRegistry) | Versioned JSON Schema validation. |
| [StangaNetLib.Notifications](https://github.com/StangaNet/StangaNetLib.Notifications) | Multi-channel notification dispatch with templates and delivery tracking. |
| [StangaNetLib.Search](https://github.com/StangaNet/StangaNetLib.Search) | Search abstractions with an in-memory BM25 backend. |
| [StangaNetLib.EventBus](https://github.com/StangaNet/StangaNetLib.EventBus) | Pub/sub event bus — InMemory and RabbitMQ, with Jobs integration. |

### Domain

| Package | Description |
| --- | --- |
| [StangaNetLib.Gdpr](https://github.com/StangaNet/StangaNetLib.Gdpr) | Consent, DSAR, objection/restriction, breach audit, and AES-GCM pseudonymization. |
| [StangaNetLib.ContentFlow](https://github.com/StangaNet/StangaNetLib.ContentFlow) | Content lifecycle state machine (Draft → Published) with scheduling and audit trail. |

---

## Philosophy

- Prefer simplicity over complexity
- Build things that last
- Invest the careful work in the libraries; keep docs helpful but secondary
- Ship when it is ready, not before

---

## License

All StangaNet projects use the **Apache License 2.0** unless a repository states otherwise.

Full license: https://github.com/StangaNet/.github/blob/main/LICENSE

---

## Contact

Use GitHub Issues or Discussions on the relevant repository.  
For security issues, use [GitHub Private Vulnerability Reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability).
