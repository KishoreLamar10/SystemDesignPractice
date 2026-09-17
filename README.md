# System Design Practice

A collection of system design practice write-ups — each subfolder works through the requirements, capacity estimation, API design, data model, and architecture for a classic system design interview problem.

## Contents

| Design | Description |
|---|---|
| [URL Shortener](./url-shortener/README.md) | A Bitly/TinyURL-style service: shorten long URLs, redirect on visit, expire links over time, and track click analytics. |
| [Rate Limiter](./rate-limiter/README.md) | A server-side rate limiter enforced at the API gateway: per-client limits via Token Bucket in Redis, sharded for 1M RPS, with fail-open resilience. |
| [Unique ID Generator](./unique-id-generator/README.md) | A Snowflake-style distributed ID generator: coordination-free, time-ordered 64-bit IDs packing a timestamp, machine ID, and sequence number. |
| [Distributed Cache](./distributed-cache/README.md) | A sharded, cache-aside caching layer: LRU eviction, consistent hashing with virtual nodes and replicas, and mitigations for stampedes, inconsistency, and hot keys. |
| [Notification System](./notification-system/README.md) | A multi-channel (email/SMS/push) notification service: per-channel queues and workers, retry with dead-lettering, idempotent delivery, and opt-out-aware rate limiting. |
| [Design Twitter](./design-twitter/README.md) | A Twitter-style social feed: sharded tweet storage, hybrid fan-out (write for normal users, read for celebrities), Kafka-driven async timeline generation, and Redis-cached feeds. |

More designs will be added here as they're completed.
