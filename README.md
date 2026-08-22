# Conductor OSS (conductor-oss)

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
