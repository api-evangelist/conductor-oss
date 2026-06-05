# Conductor OSS (conductor-oss)

Conductor OSS is the Netflix-founded, Orkes-stewarded open source workflow and agentic AI orchestration platform. It provides a durable, event-driven workflow engine for coordinating microservices, long-running tasks, human approvals, and LLM-powered agents across any language or cloud, with first class support for HTTP, gRPC, Kafka, AMQP, SQS, and MCP-based tool calling.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/conductor-oss/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/conductor-oss/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Agentic AI
- Durable Execution
- Event-Driven
- Microservices
- Netflix
- Open Source
- Orchestration
- Workflow Engine
- Workflows

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Conductor OSS REST API

The Conductor OSS REST API is the canonical control plane for the workflow engine — registering and versioning workflow and task definitions, starting and querying workflow executions, polling and updating tasks from workers, and wiring external event sources into workflows. It is served by the Conductor Server (Java / Spring Boot) and is the same surface used by every official Conductor SDK and the Orkes-hosted Conductor Cloud.

- **Human URL:** [https://docs.conductor-oss.org/](https://docs.conductor-oss.org/)
- **Base URL:** `http://localhost:8080/api`

#### Tags

- Agentic AI
- Durable Execution
- Event-Driven
- Microservices
- Open Source
- Orchestration
- Workflow Engine
- Workflows

#### Properties

- [Documentation](https://docs.conductor-oss.org/)
- [API Reference](https://docs.conductor-oss.org/reference)
- [Quickstart](https://docs.conductor-oss.org/getting-started)
- [Authentication](https://docs.conductor-oss.org/devguide/running/configuration/security)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/conductor-oss/refs/heads/main/openapi/conductor-oss-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/conductor-oss.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/conductor-oss.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Conductor MCP Server

Conductor MCP is an official Model Context Protocol server for Orkes Conductor that exposes workflow execution, task management, and metadata operations as MCP tools so that LLMs and AI agents can orchestrate Conductor workflows directly.

- **Human URL:** [https://github.com/conductor-oss/conductor-mcp](https://github.com/conductor-oss/conductor-mcp)

#### Tags

- Agentic AI
- MCP
- Open Source
- Orchestration
- Tools

#### Properties

- [GitHub Repository](https://github.com/conductor-oss/conductor-mcp)
- [Documentation](https://docs.conductor-oss.org/ai-cookbook)
- [Postman Collection](collections/conductor-oss.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/conductor-oss.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://conductor-oss.org/)
- [Documentation](https://docs.conductor-oss.org/)
- [Getting Started](https://docs.conductor-oss.org/getting-started)
- [Git Hub](https://github.com/conductor-oss)
- [GitHub Organization](https://github.com/conductor-oss)
- [GitHub Repository](https://github.com/conductor-oss/conductor)
- [Blog](https://orkes.io/blog/)
- [Slack](https://join.slack.com/t/orkes-conductor/shared_invite/zt-3dpcskdyd-W895bJDm8psAV7viYG3jFA)
- [YouTube](https://www.youtube.com/@orkesio)
- [License](https://github.com/conductor-oss/conductor/blob/main/LICENSE)
- [Pricing](https://orkes.io/pricing)
- [Portal](https://cloud.orkes.io/)
- [Sign Up](https://cloud.orkes.io/signup)
- [Training](https://orkes.io/academy/)
- [SDK](https://github.com/conductor-oss/java-sdk)
- [SDK](https://github.com/conductor-oss/python-sdk)
- [SDK](https://github.com/conductor-oss/go-sdk)
- [SDK](https://github.com/conductor-oss/javascript-sdk)
- [SDK](https://github.com/conductor-oss/csharp-sdk)
- [SDK](https://github.com/conductor-oss/clojure-sdk)
- [SDK](https://github.com/conductor-oss/rust-sdk)
- [SDK](https://github.com/conductor-oss/ruby-sdk)
- [C L I](https://github.com/conductor-oss/conductor-cli)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
