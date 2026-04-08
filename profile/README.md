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
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

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
                     scutum-detect       scutum-policy       scutum-policy      scutum-twin       scutum-audit
                                         -engine             -engine                               -chain
```

<br>

## Open Source

We publish the building blocks of sovereign infrastructure defense under Apache 2.0. Each library is independently versioned, tested, and security-scanned.

<table>
<tr><td colspan="3"><h3>Detection & Security</h3></td></tr>
<tr>
<td width="33%">

**[scutum-detect](https://github.com/scutum-defense/scutum-detect)**

Declarative threat detection rules engine. Threshold, sequence, and correlation matchers with built-in rules across perimeter, airspace, OT, and maritime.

`rules-engine` `mitre-attack`

</td>
<td width="33%">

**[scutum-policy-engine](https://github.com/scutum-defense/scutum-policy-engine)**

Policy-as-code evaluation. Operational, safety, and sovereignty constraints with deny/require_approval/warn/allow verdicts.

`policy-as-code` `safety`

</td>
<td width="33%">

**[scutum-safe-logging](https://github.com/scutum-defense/scutum-safe-logging)**

Structured safe logging with SafeArg/UnsafeArg distinction. Prevents sensitive data leakage with automatic field detection guards.

`safe-logging` `security`

</td>
</tr>
<tr><td colspan="3"><h3>Simulation & Geospatial</h3></td></tr>
<tr>
<td>

**[scutum-twin](https://github.com/scutum-defense/scutum-twin)**

Digital twin simulation framework. Validate proposed actions against infrastructure models. Outcomes: safe, unsafe, uncertain, degraded.

`digital-twin` `simulation`

</td>
<td>

**[scutum-geo](https://github.com/scutum-defense/scutum-geo)**

Geospatial primitives. Zone classification, corridor deviation, threat corridor projection, haversine, point-in-polygon.

`geospatial` `gis`

</td>
<td>

**[scutum-audit-chain](https://github.com/scutum-defense/scutum-audit-chain)**

Tamper-evident SHA-256 hash-chained audit trails. Cryptographic verification and tamper detection for command records.

`hash-chain` `cryptography`

</td>
</tr>
<tr><td colspan="3"><h3>Platform & Integration</h3></td></tr>
<tr>
<td>

**[scutum-event-kit](https://github.com/scutum-defense/scutum-event-kit)**

Type-safe event bus with middleware pipeline, typed subscriptions, and the Scutum event protocol (12 event types).

`event-bus` `messaging`

</td>
<td>

**[scutum-schemas](https://github.com/scutum-defense/scutum-schemas)**

Canonical schema registry. 15 versioned schemas across events, entities, workflows, and geospatial primitives.

`json-schema` `ontology`

</td>
<td>

**[scutum-codegen](https://github.com/scutum-defense/scutum-codegen)**

Contract-first code generation. Generates TypeScript interfaces + clients and Python Pydantic models from schema definitions.

`codegen` `contracts`

</td>
</tr>
<tr><td colspan="3"><h3>Developer Tools</h3></td></tr>
<tr>
<td>

**[scutum-sdk](https://github.com/scutum-defense/scutum-sdk)**

TypeScript SDK. Type-safe API client, SSE event streaming, authentication, and domain types for platform integration.

`sdk` `api-client`

</td>
<td>

**[scutum-cli](https://github.com/scutum-defense/scutum-cli)**

Command-line interface. Platform health, incident inspection, audit trail queries, and validation.

`cli` `devops`

</td>
<td>

**[scutum-terraform-provider](https://github.com/scutum-defense/scutum-terraform-provider)**

Terraform provider for managing platform resources — zones, corridors, detection rules, policies — as infrastructure-as-code.

`terraform` `go`

</td>
</tr>
<tr><td colspan="3"><h3>Deployment</h3></td></tr>
<tr>
<td>

**[scutum-helm](https://github.com/scutum-defense/scutum-helm)**

Kubernetes Helm charts for sovereign single-tenant deployment. Network policies, security contexts, sovereignty configuration.

`helm` `kubernetes`

</td>
<td></td>
<td></td>
</tr>
</table>

<br>

## Architecture

```
┌───────────────────────────────────────────────────────────────────────────────┐
│                          SCUTUM COMMAND PLATFORM                             │
│                                                                               │
│    Operator Surfaces                                                          │
│    ┌────────────┐  ┌────────────┐  ┌────────────┐  ┌────────────┐           │
│    │  Command   │  │  Decision  │  │  Twin      │  │  Audit &   │           │
│    │  Console   │  │  Workspace │  │  Validation│  │  Sovereignty│           │
│    └─────┬──────┘  └─────┬──────┘  └─────┬──────┘  └─────┬──────┘           │
│          └───────────────┴───────────────┴───────────────┘                    │
│                            Event Bus (event-kit)                              │
│          ┌───────────────┬───────────────┬───────────────┐                    │
│    ┌─────┴─────┐   ┌─────┴─────┐   ┌─────┴─────┐   ┌─────┴─────┐          │
│    │  Signal   │   │  AI COA   │   │  Approval  │   │  Audit    │          │
│    │  Ingestion│   │  Engine   │   │  Service   │   │  Logger   │          │
│    └───────────┘   └───────────┘   └───────────┘   └───────────┘          │
│                                                                               │
│    Core Libraries (open source · Apache-2.0)                                  │
│    ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐      │
│    │ detect │ │ policy │ │ audit  │ │  twin  │ │  geo   │ │  safe  │      │
│    │        │ │ engine │ │ chain  │ │        │ │        │ │ logging│      │
│    └────────┘ └────────┘ └────────┘ └────────┘ └────────┘ └────────┘      │
│                                                                               │
│    ┌─────────────────────────────────────────────────────────────────┐       │
│    │  event-kit · schemas · codegen · sdk · cli · terraform-provider │       │
│    └─────────────────────────────────────────────────────────────────┘       │
│                                                                               │
│    Infrastructure & Deployment                                                │
│    ┌─────────────────────────────────────────────────────────────────┐       │
│    │  PostgreSQL · Redis · Docker · Helm · Sovereign Single-Tenant   │       │
│    └─────────────────────────────────────────────────────────────────┘       │
└───────────────────────────────────────────────────────────────────────────────┘
```

<br>

## Principles

| | |
|:--|:--|
| **Sovereign by default** | All data, compute, and audit trails remain within national boundaries. Single-tenant. No shared infrastructure. |
| **Human-in-the-loop** | No autonomous action without explicit operator authorization. AI recommends, humans decide. |
| **Auditable by design** | Every signal, decision, approval, and execution produces a hash-chained, policy-labeled, tamper-evident record. |
| **Safe by construction** | No live OT write path without twin validation. Policy engine enforces safety constraints at every boundary. |
| **One platform** | One ontology, one workflow engine, one release train. No sector-specific forks. Extend through schemas, not branches. |
| **Open core** | Defense primitives are open source. Product platform is proprietary. Partners build on our published libraries. |

<br>

## Engineering Standards

Every public repository ships with:

- CI/CD pipeline (GitHub Actions)
- Security scanning (CodeQL, dependency review, TruffleHog)
- Test suite (vitest / Go test)
- Automated dependency updates (Renovate)
- Code ownership (CODEOWNERS)
- Semantic versioning and changelog
- Apache-2.0 license

<br>

## Repository Map

| Repository | Language | Purpose | License |
|:--|:--|:--|:--|
| **[scutum-detect](https://github.com/scutum-defense/scutum-detect)** | TypeScript | Threat detection rules engine | Apache-2.0 |
| **[scutum-policy-engine](https://github.com/scutum-defense/scutum-policy-engine)** | TypeScript | Policy-as-code evaluation | Apache-2.0 |
| **[scutum-safe-logging](https://github.com/scutum-defense/scutum-safe-logging)** | TypeScript | Structured safe logging | Apache-2.0 |
| **[scutum-twin](https://github.com/scutum-defense/scutum-twin)** | TypeScript | Digital twin simulation | Apache-2.0 |
| **[scutum-geo](https://github.com/scutum-defense/scutum-geo)** | TypeScript | Geospatial defense primitives | Apache-2.0 |
| **[scutum-audit-chain](https://github.com/scutum-defense/scutum-audit-chain)** | TypeScript | Cryptographic audit trails | Apache-2.0 |
| **[scutum-event-kit](https://github.com/scutum-defense/scutum-event-kit)** | TypeScript | Event bus and protocol | Apache-2.0 |
| **[scutum-schemas](https://github.com/scutum-defense/scutum-schemas)** | TypeScript | Canonical schema registry | Apache-2.0 |
| **[scutum-codegen](https://github.com/scutum-defense/scutum-codegen)** | TypeScript | Contract-first code generation | Apache-2.0 |
| **[scutum-sdk](https://github.com/scutum-defense/scutum-sdk)** | TypeScript | Platform integration SDK | Apache-2.0 |
| **[scutum-cli](https://github.com/scutum-defense/scutum-cli)** | TypeScript | Platform CLI | Apache-2.0 |
| **[scutum-terraform-provider](https://github.com/scutum-defense/scutum-terraform-provider)** | Go | Terraform provider | Apache-2.0 |
| **[scutum-helm](https://github.com/scutum-defense/scutum-helm)** | Helm | Sovereign deployment charts | Apache-2.0 |
| **scutum-mvp** | TypeScript | Production command platform | Proprietary |
| **scutum-infra** | IaC | Infrastructure-as-code | Proprietary |
| **scutum-demo** | TypeScript | Investor demo artifact | Proprietary |

<br>

---

<div align="center">

Abu Dhabi, UAE &nbsp;&nbsp;·&nbsp;&nbsp; [scutum.defense](https://scutum.defense)

</div>
