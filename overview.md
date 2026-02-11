# GLO Event Stream Platform Overview

GLO Industries provides a cloud-native event streaming platform that allows applications to ingest, store, and deliver real-time event data.

## Core Components

- **Event Ingestion API** — Send structured JSON events to GLO.
- **Sources** — Logical containers that group events by application or domain.
- **Subscriptions** — Deliver events to downstream systems via webhooks.
- **Event Store** — Durable, queryable storage for all ingested events.

## Architecture

```mermaid
flowchart LR
    A[Client App] --> B[Ingestion API]
    B --> C[Event Store]
    C --> D[Subscription Engine]
    D --> E[Webhook Destinations]
