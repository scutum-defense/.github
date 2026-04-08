<div align="center">

<br>

```
  ███████╗ ██████╗██╗   ██╗████████╗██╗   ██╗███╗   ███╗
  ██╔════╝██╔════╝██║   ██║╚══██╔══╝██║   ██║████╗ ████║
  ███████╗██║     ██║   ██║   ██║   ██║   ██║██╔████╔██║
  ╚════██║██║     ██║   ██║   ██║   ██║   ██║██║╚██╔╝██║
  ███████║╚██████╗╚██████╔╝   ██║   ╚██████╔╝██║ ╚═╝ ██║
  ╚══════╝ ╚═════╝ ╚═════╝    ╚═╝    ╚═════╝ ╚═╝     ╚═╝
```

### Sovereign Infrastructure Defense

<br>

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

</div>

<br>

Scutum builds software that helps nations protect critical infrastructure. We fuse multi-modal sensor data into a unified operating picture, generate ranked courses of action, require human authorization before execution, and produce cryptographically auditable command trails — deployed entirely within sovereign boundaries.

```
  SENSE             FUSE              DECIDE            AUTHORIZE         VALIDATE          AUDIT
  ┌────────┐       ┌────────┐       ┌────────┐       ┌────────┐       ┌────────┐       ┌────────┐
  │ Video  │──┐    │        │       │ Ranked │       │ Human  │       │Digital │       │Immutable│
  │Thermal │──┤    │ Signal │──────>│ Course │──────>│Operator│──────>│ Twin   │──────>│Command │
  │ RF     │──┼───>│ Fusion │       │   of   │       │Approval│       │  Gate  │       │ Trail  │
  │OT/SCADA│──┤    │        │       │ Action │       │        │       │        │       │        │
  │AIS/ADSB│──┘    └────────┘       └────────┘       └────────┘       └────────┘       └────────┘
```

<br>

## Engineering

<table>
<tr><td width="50%" valign="top">

**[scutum-mvp](https://github.com/scutum-defense/scutum-mvp)** &nbsp; ![CI](https://github.com/scutum-defense/scutum-mvp/actions/workflows/ci.yml/badge.svg)

Production command platform. Operator console, decision workspace, real-time event bus, AI course-of-action engine, digital twin validation, and sovereign audit trail. Monorepo with shared domain ontology across all services.

`Next.js` `Fastify` `PostgreSQL` `Redis` `pnpm`

</td><td width="50%" valign="top">

**[scutum-infra](https://github.com/scutum-defense/scutum-infra)**

Infrastructure-as-code for sovereign single-tenant deployments. Environment definitions, reusable modules, policy-as-code enforcement, and deployment automation across dev, staging, and pilot environments.

`Terraform` `Docker` `IaC`

</td></tr>
<tr><td valign="top">

**[scutum-schemas](https://github.com/scutum-defense/scutum-schemas)**

Canonical schema registry. Versioned event models, entity types, workflow state machines, and geospatial primitives. Single source of truth for all platform contracts.

`TypeScript` `JSON Schema` `Apache-2.0`

</td><td valign="top">

**[scutum-sdk](https://github.com/scutum-defense/scutum-sdk)**

Platform integration toolkit. Type-safe API client, SSE event streaming, authentication, and domain types for partner and field system integration.

`TypeScript` `Apache-2.0`

</td></tr>
</table>

<br>

## Architecture

```
┌───────────────────────────────────────────────────────────────────────┐
│                      SCUTUM COMMAND PLATFORM                         │
│                                                                       │
│  ┌────────────┐  ┌────────────┐  ┌────────────┐  ┌────────────┐    │
│  │  Operator  │  │  Decision  │  │  Digital   │  │  Audit &   │    │
│  │  Console   │  │  Workspace │  │  Twin      │  │  Sovereignty│    │
│  └─────┬──────┘  └─────┬──────┘  └─────┬──────┘  └─────┬──────┘    │
│        └────────────────┴───────────────┴───────────────┘            │
│                              SSE Event Bus                           │
│        ┌────────────────┬───────────────┬───────────────┐            │
│  ┌─────┴──────┐  ┌─────┴──────┐  ┌─────┴──────┐  ┌─────┴──────┐   │
│  │  Signal    │  │  AI COA    │  │  Approval  │  │  Audit     │   │
│  │  Ingestion │  │  Engine    │  │  Service   │  │  Logger    │   │
│  └────────────┘  └────────────┘  └────────────┘  └────────────┘   │
│                                                                       │
│  ┌────────────────────────────────────────────────────────────────┐  │
│  │  Domain Ontology  ·  Event Schemas  ·  Scenario Data  ·  ORM  │  │
│  └────────────────────────────────────────────────────────────────┘  │
│                                                                       │
│  ┌────────────────────────────────────────────────────────────────┐  │
│  │  PostgreSQL  ·  Redis  ·  Docker  ·  Sovereign Infrastructure  │  │
│  └────────────────────────────────────────────────────────────────┘  │
└───────────────────────────────────────────────────────────────────────┘
```

<br>

## Principles

| | |
|:--|:--|
| **Sovereign by default** | All data, compute, and audit trails remain within national boundaries. Single-tenant. No shared infrastructure. |
| **Human-in-the-loop** | No autonomous action without explicit operator authorization. AI recommends, humans decide. |
| **Auditable by design** | Every signal, decision, approval, and execution produces an immutable, policy-labeled record. |
| **One platform** | One ontology, one workflow engine, one release train. No sector-specific forks. |

<br>

## Open Source

We publish platform integration tools and schema contracts under Apache 2.0:

- **[@scutum/schemas](https://github.com/scutum-defense/scutum-schemas)** — Event models, entity types, workflow contracts, geospatial primitives
- **[@scutum/sdk](https://github.com/scutum-defense/scutum-sdk)** — TypeScript SDK for platform integration

<br>

---

<div align="center">

Abu Dhabi, UAE

</div>
