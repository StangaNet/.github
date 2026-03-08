# StangaNet

Personal software organization — projects built for learning, experimentation, and craft.

---

## About

StangaNet is a one-person organization maintained by a single developer.
Projects here span a range of domains: tooling, automation, web development, and system programming.

All repositories are published in **read-only** mode.
You can explore the code, learn from it, and share it with attribution —
but modifications and commercial use are not permitted.

See the [license](#license) section for details.

---

## Libraries

.NET libraries published to [GitHub Packages](https://github.com/orgs/StangaNet/packages).

| Package | Description |
| --- | --- |
| [StangaNetLib.Core](https://github.com/StangaNet/StangaNetLib.Core) | Shared primitives, result types, and base abstractions used across all StangaNet libraries |
| [StangaNetLib.Auth](https://github.com/StangaNet/StangaNetLib.Auth) | JWT authentication with refresh token rotation, BCrypt hashing, and revocation middleware |
| [StangaNetLib.Caching](https://github.com/StangaNet/StangaNetLib.Caching) | `ICacheService` abstraction over in-memory, Redis, and null cache backends |
| [StangaNetLib.Observability](https://github.com/StangaNet/StangaNetLib.Observability) | Structured logging, tracing, and metrics helpers for ASP.NET Core |
| [StangaNetLib.RateLimit](https://github.com/StangaNet/StangaNetLib.RateLimit) | Rate limiting middleware and policy builder for ASP.NET Core |
| [StangaNetLib.Idempotency](https://github.com/StangaNet/StangaNetLib.Idempotency) | Idempotency key middleware for HTTP APIs |
| [StangaNetLib.Gdpr](https://github.com/StangaNet/StangaNetLib.Gdpr) | GDPR data-handling utilities (anonymization, retention, consent) |
| [StangaNetLib.Media](https://github.com/StangaNet/StangaNetLib.Media) | Media upload, validation, and storage abstractions |
| [StangaNetLib.ContentFlow](https://github.com/StangaNet/StangaNetLib.ContentFlow) | Content pipeline and workflow engine for structured content management |

All packages target **net8.0** and **net9.0** and are installed via the StangaNet GitHub Packages NuGet feed.

---

## Philosophy

- Prefer simplicity over complexity
- Build things that last
- Document as you go
- Ship when it is ready, not before

---

## License

All StangaNet projects are released under the
**StangaNet Source-Available License v1.0**.

**In plain language:**
- You **can** view and study the code
- You **can** use it in personal, non-commercial projects
- You **must always** credit StangaNet as the original author
- You **cannot** distribute modified versions
- You **cannot** use it commercially
- You **cannot** claim authorship or remove attribution

Full license: [LICENSE](https://github.com/StangaNet/.github/blob/main/LICENSE)

---

## Contact

Use GitHub Issues or Discussions on the relevant repository.
For security issues, use [GitHub Private Vulnerability Reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability).
