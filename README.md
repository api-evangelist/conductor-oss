# Conductor OSS (conductor-oss)

Conductor OSS is the Netflix-founded, Orkes-stewarded open source workflow and agentic AI orchestration platform. It provides a durable, event-driven workflow engine for coordinating microservices, long-running tasks, human approvals, and LLM-powered agents across any language or cloud, with first class support for HTTP, gRPC, Kafka, AMQP, SQS, and MCP-based tool calling.

**URL:** [Visit APIs.yml URL](https://raw.githubusercontent.com/api-evangelist/conductor-oss/refs/heads/main/apis.yml)

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

**Human URL:** [https://docs.conductor-oss.org/](https://docs.conductor-oss.org/)

**Base URL:** `http://localhost:8080/api`

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
- [OpenAPI](openapi/conductor-oss-openapi.yml)
- [Naftiko Capability — Workflow](capabilities/conductor-workflow.yaml)
- [Naftiko Capability — Tasks](capabilities/conductor-tasks.yaml)
- [Naftiko Capability — Metadata](capabilities/conductor-metadata.yaml)
- [Naftiko Capability — Events](capabilities/conductor-events.yaml)

### Conductor MCP Server

Conductor MCP is an official Model Context Protocol server for Orkes Conductor that exposes workflow execution, task management, and metadata operations as MCP tools so that LLMs and AI agents can orchestrate Conductor workflows directly.

**Human URL:** [https://github.com/conductor-oss/conductor-mcp](https://github.com/conductor-oss/conductor-mcp)

#### Tags

- Agentic AI
- MCP
- Open Source
- Orchestration
- Tools

#### Properties

- [GitHub Repository](https://github.com/conductor-oss/conductor-mcp)
- [Documentation](https://docs.conductor-oss.org/ai-cookbook)

## Common Properties

- [Website](https://conductor-oss.org/)
- [Documentation](https://docs.conductor-oss.org/)
- [Getting Started](https://docs.conductor-oss.org/getting-started)
- [GitHub](https://github.com/conductor-oss)
- [GitHub Organization](https://github.com/conductor-oss)
- [GitHub Repository](https://github.com/conductor-oss/conductor)
- [Blog](https://orkes.io/blog/)
- [Slack](https://join.slack.com/t/orkes-conductor/shared_invite/zt-3dpcskdyd-W895bJDm8psAV7viYG3jFA)
- [YouTube](https://www.youtube.com/@orkesio)
- [License (Apache 2.0)](https://github.com/conductor-oss/conductor/blob/main/LICENSE)
- [Pricing](https://orkes.io/pricing)
- [Portal](https://cloud.orkes.io/)
- [Sign Up](https://cloud.orkes.io/signup)
- [Training / Academy](https://orkes.io/academy/)
- [Java SDK](https://github.com/conductor-oss/java-sdk)
- [Python SDK](https://github.com/conductor-oss/python-sdk)
- [Go SDK](https://github.com/conductor-oss/go-sdk)
- [JavaScript / TypeScript SDK](https://github.com/conductor-oss/javascript-sdk)
- [C# SDK](https://github.com/conductor-oss/csharp-sdk)
- [Clojure SDK](https://github.com/conductor-oss/clojure-sdk)
- [Rust SDK](https://github.com/conductor-oss/rust-sdk)
- [Ruby SDK](https://github.com/conductor-oss/ruby-sdk)
- [CLI](https://github.com/conductor-oss/conductor-cli)

### Features

- **Durable Workflow Execution** — Workflow state is persisted at every step so executions survive worker restarts, server failover, and long human-in-the-loop waits.
- **Polyglot Workers** — Tasks are executed by language-agnostic workers that poll the server, with official SDKs in Java, Python, Go, JavaScript / TypeScript, C#, Clojure, Ruby, and Rust.
- **System Tasks and Operators** — Built-in HTTP, Kafka, JQ, wait, human approval, sub-workflow, fork, join, switch, do-while, and dynamic-fork operators compose workflows without writing code.
- **Agentic AI and LLM Orchestration** — Native LLM tasks for 14+ providers, vector database integrations for RAG, MCP tool calling, and human-in-the-loop checkpoints make Conductor a runtime for agentic AI applications.
- **Event-Driven Triggers** — Event handlers consume from Kafka, AMQP, SQS, NATS, and webhook sources to start workflows or complete tasks from external systems.
- **Horizontal Scalability** — Stateless API servers and worker pools scale horizontally, with pluggable persistence (PostgreSQL, MySQL, Cassandra, Redis) and indexing (OpenSearch / Elasticsearch).
- **Operational Observability** — Built-in metrics, structured logs, distributed tracing, and a Swagger UI on every server expose the workflow surface for operators.

### Use Cases

- **Microservices Orchestration** — Coordinate sagas, compensations, retries, and timeouts across distributed microservices without bespoke orchestration code.
- **AI Agent Orchestration** — Run production-grade agentic workflows with reasoning loops, tool calling, MCP integration, RAG retrieval, and human approvals.
- **Payment and Order Processing** — Reliable long-running flows for payments, fulfillment, KYC, and onboarding — the reference example workload shipped by Conductor.
- **Data and ML Pipelines** — Schedule and orchestrate ETL, model training, and inference pipelines with durable retries and conditional branching.
- **Human-in-the-Loop Approvals** — Pause workflows on human tasks, capture approvals via UI or API, and resume execution deterministically.
- **Event-Driven Integration** — Bridge message brokers and SaaS webhooks into deterministic workflows across the enterprise.

### Integrations

- **Apache Kafka** — System task and event-handler integration for Kafka topics.
- **AMQP / RabbitMQ** — Built-in AMQP system task and event source.
- **AWS SQS** — Native SQS event queue and system task module.
- **NATS** — NATS event queue integration for triggering workflows.
- **PostgreSQL / MySQL / Cassandra / Redis** — Pluggable persistence backends for workflow and task state.
- **OpenSearch / Elasticsearch** — Pluggable indexing backends powering search and history.
- **AWS S3 / Azure Blob** — External payload storage for large workflow inputs and outputs.
- **Model Context Protocol (MCP)** — Official MCP server exposes Conductor to AI agents as tools.
- **gRPC** — gRPC API surface alongside the REST API for high-performance clients.

### Solutions

- **Conductor OSS** — Apache 2.0 open source workflow engine, self-hosted via Docker, Helm, or source build.
- **Orkes Developer Edition** — Free hosted Conductor sandbox by Orkes with all enterprise features enabled for prototyping and learning.
- **Orkes Enterprise / Cloud** — Fully managed Conductor on AWS, Azure, GCP, or on-prem with SOC2, RBAC, SSO, audit logs, and up to 99.99% availability SLA.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
