# Stream (getstream)

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
