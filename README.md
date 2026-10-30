# Stream

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

Stream (GetStream.io) provides scalable, API-first infrastructure for in-app chat messaging, activity feeds, audio/video calling and livestreaming, and AI moderation. The server-side platform is a documented REST API (base https://chat.stream-io-api.com for Chat) with JWT authentication, complemented by client SDKs that open a persistent WebSocket connection to receive real-time events - message.new, typing.start, user.presence.changed, reaction.new, notification.* and periodic health.check heartbeats. Products are metered on monthly active users (Chat) and participant minutes (Video), with Free/Maker, Standard (Startup) and Enterprise tiers.

**Areas:** Chat · Messaging · Activity Feeds · Video · Audio · Moderation · WebSocket · Real-Time

## Stream on APIs.io

Everything profiled for Stream is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/getstream/](https://apis.io/providers/getstream/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Stream Activity Feeds API](https://apis.io/apis/getstream/getstream-activity-feeds-api/) — Build scalable activity feeds and timelines - add activities to feeds, follow and unfollow feeds, aggregate and rank activities, and fan out to followers.…
- [Stream Video and Audio API](https://apis.io/apis/getstream/getstream-video-audio-api/) — Create and manage audio/video calls and livestreams - get-or-create calls, manage call members and permissions, start and stop recording, transcription, and…
- [Stream Product:chat API](https://apis.io/apis/getstream/getstream-product-chat-api/) — The product:chat API from Stream — 194 operation(s) for product:chat.
- [Stream Product:common API](https://apis.io/apis/getstream/getstream-product-common-api/) — The product:common API from Stream — 54 operation(s) for product:common.
- [Stream Product:feeds API](https://apis.io/apis/getstream/getstream-product-feeds-api/) — The product:feeds API from Stream — 69 operation(s) for product:feeds.
- [Stream Product:moderation API](https://apis.io/apis/getstream/getstream-product-moderation-api/) — The product:moderation API from Stream — 56 operation(s) for product:moderation.
- [Stream Product:video API](https://apis.io/apis/getstream/getstream-product-video-api/) — The product:video API from Stream — 121 operation(s) for product:video.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (2)

Event-driven and webhook contracts.

- [Stream Chat Realtime WebSocket API](https://apis.io/asyncapis/getstream/getstream-asyncapi/)
- [Stream Chat WebSocket API](https://apis.io/asyncapis/getstream/stream-io-asyncapi/)

#### Event channels (2)

Individual events and webhooks the provider emits.

- [/connect](https://apis.io/channels/getstream/connect/)
- [/connect](https://apis.io/channels/getstream/stream-chat-websocket-api-connect/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Getstream Agentic Access](https://apis.io/agentic-access/getstream/getstream-agentic-access/)

#### Collections (13)

Postman and Open Collection request collections.

- [Stream Chat API (Server-side REST)](https://apis.io/collections/getstream/open-getstream/)
- [Stream Chat API (Server-side REST) Application API](https://apis.io/collections/getstream/open-getstream-application-api/)
- [Stream Chat API (Server-side REST) Application Campaigns API](https://apis.io/collections/getstream/open-getstream-campaigns-api/)
- [Stream Chat API (Server-side REST) Application Channels API](https://apis.io/collections/getstream/open-getstream-channels-api/)
- [Stream Chat API (Server-side REST) Application Devices API](https://apis.io/collections/getstream/open-getstream-devices-api/)
- [Stream Chat API (Server-side REST) Application Members API](https://apis.io/collections/getstream/open-getstream-members-api/)
- [Stream Chat API (Server-side REST) Application Messages API](https://apis.io/collections/getstream/open-getstream-messages-api/)
- [Stream Chat API (Server-side REST) Application Moderation API](https://apis.io/collections/getstream/open-getstream-moderation-api/)
- [Stream Chat API (Server-side REST) Application Permissions API](https://apis.io/collections/getstream/open-getstream-permissions-api/)
- [Stream Chat API (Server-side REST) Application Reactions API](https://apis.io/collections/getstream/open-getstream-reactions-api/)
- [Stream Chat API (Server-side REST) Application Roles API](https://apis.io/collections/getstream/open-getstream-roles-api/)
- [Stream Chat API (Server-side REST) Application Threads API](https://apis.io/collections/getstream/open-getstream-threads-api/)
- [Stream Chat API (Server-side REST) Application Users API](https://apis.io/collections/getstream/open-getstream-users-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Stream — asyncapi rules](https://apis.io/rules/getstream/getstream-asyncapi-spectral-rules/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Getstream Authentication](https://apis.io/security/getstream/getstream-authentication/)
- [Getstream Domain Security](https://apis.io/security/getstream/getstream-domain-security/)
- [Getstream Trust Center](https://apis.io/security/getstream/getstream-trust-center/)
- [Getstream Vulnerability Disclosure](https://apis.io/security/getstream/getstream-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Getstream Plans Pricing](https://apis.io/plans/getstream/getstream-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Getstream Rate Limits](https://apis.io/rate-limits/getstream/getstream-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Getstream Finops](https://apis.io/finops/getstream/getstream-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://getstream.io)
- [Documentation](https://getstream.io/chat/docs/)
- [Blog](https://getstream.io/blog/rss.xml)
- [GitHub](https://github.com/GetStream)

## API Evangelist rating

**Kin Score 44.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 58.4 |
| Contract governance | 11.4 |
| Operational transparency | 21.1 |
| Developer ergonomics | 38.1 |
| Access clarity | 15.8 |

**Agent readiness 28.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | paginated |
| Operation Distinctiveness | — |

**Regulatory alignment 22.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/getstream/](https://apis.io/providers/getstream/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Stream: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/getstream/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
