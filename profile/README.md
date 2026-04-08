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
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

</div>

<br>

We build software that helps nations protect critical infrastructure. Scutum fuses multi-modal sensor data into a unified operating picture, generates ranked courses of action, requires human authorization before execution, validates outcomes through digital twin simulation, and produces cryptographically auditable command trails — deployed entirely within sovereign boundaries.

```
  SENSE               FUSE                DECIDE              AUTHORIZE           VALIDATE            AUDIT
  ┌─────────┐        ┌─────────┐        ┌─────────┐        ┌─────────┐        ┌─────────┐        ┌─────────┐
  │ Video   │──┐     │         │        │ Ranked  │        │ Human   │        │ Digital │        │ Hash-   │
  │ Thermal │──┤     │ Signal  │───────>│ Course  │───────>│ Operator│───────>│  Twin   │───────>│ Chained │
  │ RF      │──┼────>│ Fusion  │        │   of    │        │ Approval│        │  Gate   │        │ Audit   │
  │ OT/SCADA│──┤     │ Engine  │        │ Action  │        │         │        │         │        │ Trail   │
  │ AIS     │──┤     │         │        │         │        │         │        │         │        │         │
  │ ADS-B   │──┘     └─────────┘        └─────────┘        └─────────┘        └─────────┘        └─────────┘
                                                                               scutum-twin        scutum-audit-chain
             scutum-detect             scutum-policy-engine                                      
```

<br>

## Open Source

We publish the building blocks of sovereign infrastructure defense under Apache 2.0.

<table>
<tr><td colspan="3"><h3>Detection & Security</h3></td></tr>
<tr>
<td width="30%">

**[scutum-detect](https://github.com/scutum-defense/scutum-detect)**

Declarative threat detection rules engine. Threshold, sequence, and correlation matchers with MITRE ATT&CK mapping.

`rules-engine` `mitre-attack`

</td>
<td width="30%">

**[scutum-policy-engine](https://github.com/scutum-defense/scutum-policy-engine)**

Policy-as-code evaluation. Operational, safety, and sovereignty policies with allow/deny/warn/require_approval verdicts.

`policy-as-code` `opa`

</td>
<td width="30%">

**[scutum-audit-chain](https://github.com/scutum-defense/scutum-audit-chain)**

Tamper-evident, SHA-256 hash-chained audit trails. Cryptographic integrity verification for command records.

`hash-chain` `sha256`

</td>
</tr>
<tr><td colspan="3"><h3>Simulation & Geospatial</h3></td></tr>
<tr>
<td>

**[scutum-twin](https://github.com/scutum-defense/scutum-twin)**

Digital twin simulation framework. Validate proposed actions against infrastructure models before execution.

`digital-twin` `simulation`

</td>
<td>

**[scutum-geo](https://github.com/scutum-defense/scutum-geo)**

Geospatial primitives. Zone classification, corridor deviation analysis, threat corridor projection, haversine calculations.

`geospatial` `gis`

</td>
<td>

**[scutum-schemas](https://github.com/scutum-defense/scutum-schemas)**

Canonical schema registry. Versioned event models, entity types, workflow state machines, geospatial primitives.

`json-schema` `ontology`

</td>
</tr>
<tr><td colspan="3"><h3>Platform Integration</h3></td></tr>
<tr>
<td>

**[scutum-sdk](https://github.com/scutum-defense/scutum-sdk)**

TypeScript SDK. Type-safe API client, SSE event streaming, authentication, and domain types for platform integration.

`sdk` `api-client`

</td>
<td>

**[scutum-cli](https://github.com/scutum-defense/scutum-cli)**

Command-line interface. Platform health, incident inspection, audit trail queries, and schema/policy validation.

`cli` `devops`

</td>
<td>

</td>
</tr>
</table>

<br>

## Architecture

```
┌──────────────────────────────────────────────────────────────────────────────┐
│                         SCUTUM COMMAND PLATFORM                             │
│                                                                              │
│    Operator Surfaces                                                         │
│    ┌────────────┐  ┌────────────┐  ┌────────────┐  ┌────────────┐          │
│    │  Command   │  │  Decision  │  │  Twin      │  │  Audit &   │          │
│    │  Console   │  │  Workspace │  │  Validation│  │  Sovereignty│          │
│    └─────┬──────┘  └─────┬──────┘  └─────┬──────┘  └─────┬──────┘          │
│          └───────────────┴───────────────┴───────────────┘                   │
│                               SSE Event Bus                                  │
│          ┌───────────────┬───────────────┬───────────────┐                   │
│    ┌─────┴─────┐   ┌─────┴─────┐   ┌─────┴─────┐   ┌─────┴─────┐         │
│    │  Signal   │   │  AI COA   │   │  Approval  │   │  Audit    │         │
│    │  Ingestion│   │  Engine   │   │  Service   │   │  Logger   │         │
│    └───────────┘   └───────────┘   └───────────┘   └───────────┘         │
│                                                                              │
│    Core Libraries (open source)                                              │
│    ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐       │
│    │ detect   │ │ policy-  │ │ audit-   │ │  twin    │ │   geo    │       │
│    │          │ │ engine   │ │ chain    │ │          │ │          │       │
│    └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘       │
│                                                                              │
│    ┌──────────────────────────────────────────────────────────────────┐     │
│    │  schemas  ·  sdk  ·  cli  ·  Domain Ontology  ·  Event Bus      │     │
│    └──────────────────────────────────────────────────────────────────┘     │
│                                                                              │
│    Infrastructure                                                            │
│    ┌──────────────────────────────────────────────────────────────────┐     │
│    │  PostgreSQL  ·  Redis  ·  Docker  ·  Sovereign Single-Tenant    │     │
│    └──────────────────────────────────────────────────────────────────┘     │
└──────────────────────────────────────────────────────────────────────────────┘
```

<br>

## Principles

| | |
|:--|:--|
| **Sovereign by default** | All data, compute, and audit trails remain within national boundaries. Single-tenant. No shared infrastructure. No data exfiltration. |
| **Human-in-the-loop** | No autonomous action without explicit operator authorization. AI recommends, humans decide. Every approval is identity-bound. |
| **Auditable by design** | Every signal, decision, approval, and execution produces a hash-chained, policy-labeled, tamper-evident record. |
| **One platform** | One ontology, one workflow engine, one release train. No sector-specific forks. Extend through schemas, not branches. |
| **Safe by construction** | No live OT write path without twin validation. Policy engine enforces safety constraints at every decision boundary. |

<br>

## Repository Map

| Repository | Visibility | Purpose | License |
|:--|:--|:--|:--|
| **[scutum-detect](https://github.com/scutum-defense/scutum-detect)** | Public | Threat detection rules engine | Apache-2.0 |
| **[scutum-geo](https://github.com/scutum-defense/scutum-geo)** | Public | Geospatial defense primitives | Apache-2.0 |
| **[scutum-audit-chain](https://github.com/scutum-defense/scutum-audit-chain)** | Public | Cryptographic audit trails | Apache-2.0 |
| **[scutum-policy-engine](https://github.com/scutum-defense/scutum-policy-engine)** | Public | Policy-as-code evaluation | Apache-2.0 |
| **[scutum-twin](https://github.com/scutum-defense/scutum-twin)** | Public | Digital twin simulation | Apache-2.0 |
| **[scutum-schemas](https://github.com/scutum-defense/scutum-schemas)** | Public | Canonical schema registry | Apache-2.0 |
| **[scutum-sdk](https://github.com/scutum-defense/scutum-sdk)** | Public | Platform integration SDK | Apache-2.0 |
| **[scutum-cli](https://github.com/scutum-defense/scutum-cli)** | Public | Platform CLI | Apache-2.0 |
| **scutum-mvp** | Private | Production command platform | Proprietary |
| **scutum-infra** | Private | Infrastructure-as-code | Proprietary |
| **scutum-demo** | Private | Investor demo artifact | Proprietary |

<br>

---

<div align="center">

Abu Dhabi, UAE &nbsp;&nbsp;·&nbsp;&nbsp; [scutum.defense](https://scutum.defense)

</div>
