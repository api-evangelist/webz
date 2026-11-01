# Webz.io

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Webz.io provides structured web-data feeds and APIs covering the open, deep, and dark web for AI, cybersecurity, and intelligence use cases. Content is collected at scale, normalized, enriched with metadata, and delivered through machine-readable data feeds and token-authenticated REST APIs.

**Areas:** News Data · Web Data · Web Scraping · Dark Web · deep-web · Cybersecurity · Threat Intelligence · Data Breaches · pii-monitoring · OSINT · reviews-data · AI Training Data

## Webz.io on APIs.io

Everything profiled for Webz.io is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/webz/](https://apis.io/providers/webz/)** — or go straight to one of the APIs or properties below.

### APIs (13)

- [Webz.io API](https://apis.io/apis/webz/webzio-api/) — Token-authenticated REST endpoints under https://api.webz.io covering seven products: News, Blogs and Forums (/api/news, /api/blogs, /api/forums plus…
- [Webz.io News Search MCP Server](https://apis.io/apis/webz/webzio-news-search-mcp-server/) — A first-party remote Model Context Protocol server that exposes Webz.io semantic news search to any MCP client. It ships one tool, news_search_by_webz, and…
- [Webz.io News, Blogs & Forums API](https://apis.io/apis/webz/webzio-news-blogs-forums-api/) — Live open-web content split by source type. One base URL, six GET endpoints (`/api/news`, `/api/blogs`, `/api/forums` for posts and `/seg_api/news`,…
- [Webz.io News Search API](https://apis.io/apis/webz/webzio-news-search-api/) — Contextual, natural-language news search. Single `POST /api/news/context` endpoint that returns ranked article excerpts matching a free-text query. Backs…
- [Webz.io Cyber API](https://apis.io/apis/webz/webzio-cyber-api/) — Deep and dark web content for threat intelligence. Search endpoint `/cyberFilter`, segmentation `/cyberSeg`, and helper endpoints `/dark-cache` (cached page…
- [Webz.io Data Breaches API](https://apis.io/apis/webz/webzio-data-breaches-api/) — Search compromised records and look up known breaches. Two GET endpoints, `/breaches` (main search) and `/breachCatalog` (breach lookup by name to UUID),…
- [Webz.io Leaked Cookies API](https://apis.io/apis/webz/webzio-leaked-cookies-api/) — Look up leaked session cookies matched to a domain. Single GET endpoint `/cookies` with token authentication and domain-scoped credit consumption.
- [Webz.io Non-Human Identities (NHI) API](https://apis.io/apis/webz/webzio-non-human-identities-nhi-api/) — Detect leaked machine credentials (API keys, tokens, secrets) tied to a domain. Single GET endpoint `/nhi` with token authentication.
- [Webz.io Firehose API](https://apis.io/apis/webz/webzio-firehose-api/) — REST-delivered curated firehose of enriched open-web posts. Preconfigured per-customer feeds via `/firehose?token=&client_feed=`; paginated with `nextPage`.…
- [Webz.io Archive API](https://apis.io/apis/webz/webzio-archive-api/) — Build and deliver historical datasets in three steps - set query and date range at `/setArchiveQuery`, confirm at `/confirmArchiveQuery`, then poll…
- [Webz.io Reviews API](https://apis.io/apis/webz/webzio-reviews-api/) — Customer reviews and ratings collected from across the open web as structured JSON - rating, author, language, and the item being reviewed. Shares the…
- [Webz.io Domain Exposure API (DEA)](https://apis.io/apis/webz/webzio-domain-exposure-api-dea/) — Analyze a domain's exposure across breach, leaked-cookie, and NHI datasets. Served from `api.lunarcyber.com` (Webz.io's Lunar-branded cyber intelligence…
- [Webz.io Web Content API (deprecated)](https://apis.io/apis/webz/webzio-web-content-api-deprecated/) — Legacy unified `/filterWebContent` endpoint (GET or POST) that returned any open-web content type in one call. Deprecated in favor of the split News, Blogs…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Webz.io News Search MCP](https://apis.io/servers/webz/webz-io-news-search-mcp/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Webz Authentication](https://apis.io/security/webz/webz-authentication/)
- [Webz Domain Security](https://apis.io/security/webz/webz-domain-security/)
- [Webz Trust Center](https://apis.io/security/webz/webz-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Webz Scopes](https://apis.io/scopes/webz/webz-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Webz Plans Pricing](https://apis.io/plans/webz/webz-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Webz Rate Limits](https://apis.io/rate-limits/webz/webz-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.webz.io/)
- [Documentation](https://docs.webz.io/docs/webz)
- [Getting started](https://docs.webz.io/docs/webz/start-here)
- [API reference](https://docs.webz.io/docs/webz/news-blogs-forums-api-reference)
- [Pricing](https://webz.io/pricing)
- [Sign up](https://app.webz.io/auth/signup)
- [Support](https://webz.io/contact-us)
- [Blog](https://webz.io/blog)
- [Terms of service](https://webz.io/tos/)
- [Privacy policy](https://webz.io/privacy/)
- [GitHub](https://github.com/Webhose)
- [Status](https://status.webz.io)

## API Evangelist rating

**Kin Score 54.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 80.0 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 57.9 |
| Developer ergonomics | 71.4 |
| Access clarity | 92.1 |

**Agent readiness 36.3** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 39.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/webz/](https://apis.io/providers/webz/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Webz.io: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/webz/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
