# Stream (getstream)

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

Stream (GetStream.io) provides scalable, API-first infrastructure for in-app chat messaging, activity feeds, audio/video calling and livestreaming, and AI moderation. The server-side platform is a documented REST API (base `https://chat.stream-io-api.com` for Chat) authenticated with a JWT in the `Authorization` header plus a `Stream-Auth-Type: jwt` header and the application `api_key` query parameter. Client SDKs additionally open a persistent **WebSocket** connection (`wss://chat.stream-io-api.com/connect`) to receive real-time events - `message.new`, `typing.start`, `reaction.new`, `user.presence.changed`, `notification.*` - and periodic `health.check` heartbeats. Chat and Feeds are metered on Monthly Active Users (MAU); Video is metered on participant minutes.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/apis.yml)

## Tags

- Chat
- Messaging
- Activity Feeds
- Video
- Audio
- Moderation
- WebSocket
- Real Time

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Stream Chat Channels API

Query, get-or-create, update, truncate, and delete chat channels, and mark them read. Channels are the containers that hold messages, members, reads, and reactions, addressed by a channel type and id (e.g. `messaging:general`).

- **Human URL:** [https://getstream.io/chat/docs/](https://getstream.io/chat/docs/)
- **Base URL:** `https://chat.stream-io-api.com`

#### Properties

- [Documentation](https://getstream.io/chat/docs/)
- [API Reference](https://getstream.github.io/protocol/?urls.primaryName=Chat)
- [OpenAPI](openapi/getstream-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/getstream-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/v2.6.0)

### Stream Chat Messages API

Send, get, update, and delete messages within a channel, fetch thread replies and message history, and run message search across an application's channels.

- **Human URL:** [https://getstream.io/chat/docs/node/send_message/](https://getstream.io/chat/docs/node/send_message/)
- **Base URL:** `https://chat.stream-io-api.com`

### Stream Chat Members API

Query channel members with filtering and sorting, and partially update a member's channel-scoped attributes such as role, notifications, and pinned or archived state.

- **Human URL:** [https://getstream.io/chat/docs/node/channel_members/](https://getstream.io/chat/docs/node/channel_members/)
- **Base URL:** `https://chat.stream-io-api.com`

### Stream Chat Reactions API

Add, list, and remove emoji reactions on messages. Reactions carry a type (like, love, haha) and optional score, and emit `reaction.new` and `reaction.deleted` real-time events.

- **Human URL:** [https://getstream.io/chat/docs/node/send_reaction/](https://getstream.io/chat/docs/node/send_reaction/)
- **Base URL:** `https://chat.stream-io-api.com`

### Stream Chat Threads API

Query threads a user participates in, retrieve a single thread by its parent message id, and partially update thread metadata. Threads group replies under a parent message.

- **Human URL:** [https://getstream.io/chat/docs/node/threads/](https://getstream.io/chat/docs/node/threads/)
- **Base URL:** `https://chat.stream-io-api.com`

### Stream Chat Users API

Upsert, query, and partially update users, and deactivate or reactivate them. Users carry custom data and roles and are the identities that connect over the WebSocket and appear as channel members.

- **Human URL:** [https://getstream.io/chat/docs/node/update_users/](https://getstream.io/chat/docs/node/update_users/)
- **Base URL:** `https://chat.stream-io-api.com`

### Stream Chat Devices and Push API

Register, list, and remove a user's push devices (APNs, Firebase) so Stream can deliver offline push notifications, and manage push providers for the application.

- **Human URL:** [https://getstream.io/chat/docs/node/push_devices/](https://getstream.io/chat/docs/node/push_devices/)
- **Base URL:** `https://chat.stream-io-api.com`

### Stream Chat Moderation API

Ban and unban users, flag messages and users for review, and mute or unmute users and channels. Backs Stream's AI-powered trust and safety and content moderation workflows.

- **Human URL:** [https://getstream.io/moderation/docs/](https://getstream.io/moderation/docs/)
- **Base URL:** `https://chat.stream-io-api.com`

### Stream Chat Permissions and Roles API

List permissions, create and delete custom roles, and inspect the role-based access control that governs what users and channel members are allowed to do across the application.

- **Human URL:** [https://getstream.io/chat/docs/node/permissions_reference/](https://getstream.io/chat/docs/node/permissions_reference/)
- **Base URL:** `https://chat.stream-io-api.com`

### Stream Chat Campaigns API

Create, update, and delete bulk messaging campaigns and start or stop their delivery to user segments. Used to send templated messages to targeted audiences at scale.

- **Human URL:** [https://getstream.io/chat/docs/node/campaigns/](https://getstream.io/chat/docs/node/campaigns/)
- **Base URL:** `https://chat.stream-io-api.com`

### Stream Activity Feeds API

Build scalable activity feeds and timelines - add activities to feeds, follow and unfollow feeds, aggregate and rank activities, and fan out to followers. Powers social timelines, notification feeds, and news feeds.

- **Human URL:** [https://getstream.io/activity-feeds/docs/](https://getstream.io/activity-feeds/docs/)
- **Base URL:** `https://api.stream-io-api.com`

### Stream Video and Audio API

Create and manage audio/video calls and livestreams - get-or-create calls, manage call members and permissions, start and stop recording, transcription, and broadcasting. Metered on participant minutes.

- **Human URL:** [https://getstream.io/video/docs/api/](https://getstream.io/video/docs/api/)
- **Base URL:** `https://video.stream-io-api.com`

## Real-Time WebSocket

Stream Chat clients open a WebSocket to `wss://chat.stream-io-api.com/connect` (via `client.connectUser()`) to receive real-time events. The connection is modeled in [asyncapi/getstream-asyncapi.yml](asyncapi/getstream-asyncapi.yml). Stream limits open connections to 50 per user in production (3 in development).

## Common Properties

- [GitHub Organization](https://github.com/GetStream)
- [LinkedIn](https://www.linkedin.com/company/getstream)
- [Website](https://getstream.io)
- [Documentation](https://getstream.io/chat/docs/)
- [Plans](plans/getstream-plans-pricing.yml)
- [Rate Limits](rate-limits/getstream-rate-limits.yml)
- [Fin Ops](finops/getstream-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
