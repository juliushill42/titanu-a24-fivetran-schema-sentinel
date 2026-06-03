# titanu-a24-fivetran-schema-sentinel

> Monitors Fivetran connector schemas for drift, alerts on breaking changes, auto-maps.

**Track:** FIVETRAN | **Author:** Julius Cameron Hill — TitanU AI LLC | **Patent:** JCH-2026-001

## Overview

Built for the **Google Cloud Rapid Agent Hackathon** using **Gemini 2.5 Flash** + **Vertex AI** + **Fivetran MCP Server**.

## Architecture

```
User Query → Gemini 2.5 Flash (Vertex AI)
                    ↓
         FIVETRAN MCP Server
                    ↓
         Structured JSON Response
```

## Setup

```bash
npm install
cp .env.example .env
# Set GOOGLE_CLOUD_PROJECT, GOOGLE_APPLICATION_CREDENTIALS
node src/index.js
```

## Environment

| Variable | Description |
|---|---|
| `GOOGLE_CLOUD_PROJECT` | GCP project ID |
| `GOOGLE_CLOUD_LOCATION` | Region (default: us-central1) |
| `MCP_URL` | Fivetran MCP endpoint |

## Tech Stack

- **AI:** Gemini 2.5 Flash via Vertex AI / Google ADK
- **Partner:** Fivetran MCP Server
- **Runtime:** Node.js
- **Cloud:** Google Cloud

## License

MIT — see [LICENSE](LICENSE)

## IP Notice

TitanU AI LLC — Julius Cameron Hill. JCH-2026-001.
