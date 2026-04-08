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
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)

</div>

<br>

We build software that helps nations protect critical infrastructure. Scutum fuses multi-modal sensor data into a unified operating picture, generates ranked courses of action, requires human authorization before execution, validates outcomes through digital twin simulation, and produces cryptographically auditable command trails — all deployed within sovereign boundaries.

```
  SENSE               FUSE                DECIDE              AUTHORIZE           VALIDATE            AUDIT
  ┌─────────┐        ┌─────────┐        ┌─────────┐        ┌─────────┐        ┌─────────┐        ┌─────────┐
  │ Video   │──┐     │         │        │ Ranked  │        │ Human   │        │ Digital │        │ Hash-   │
  │ Thermal │──┤     │ Signal  │───────>│ Course  │───────>│ Operator│───────>│  Twin   │───────>│ Chained │
  │ RF      │──┼────>│ Fusion  │        │   of    │        │ Approval│        │  Gate   │        │ Audit   │
  │ OT/SCADA│──┤     │ Engine  │        │ Action  │        │         │        │         │        │ Trail   │
  │ AIS     │──┤     │         │        │         │        │         │        │         │        │         │
  │ ADS-B   │──┘     └─────────┘        └─────────┘        └─────────┘        └─────────┘        └─────────┘
```

<br>

## Open Source

We publish the building blocks of sovereign infrastructure defense under Apache 2.0.

<table>
<tr><td colspan="3"><h3>Detection & Security</h3></td></tr>
<tr>
<td width="33%">

**[scutum-detect](https://github.com/scutum-defense/scutum-detect)**

Declarative threat detection rules engine. Threshold, sequence, and correlation matchers with MITRE ATT&CK mapping.

</td>
<td width="33%">

**[scutum-detection-packs](https://github.com/scutum-defense/scutum-detection-packs)**

15 curated detection rules across 6 sectors: port, energy, airspace, maritime, OT, cyber-physical. Response playbooks and false positive guidance.

</td>
<td width="33%">

**[scutum-policy-engine](https://github.com/scutum-defense/scutum-policy-engine)**

Policy-as-code evaluation. Operational, safety, and sovereignty constraints with deny/require_approval/warn/allow verdicts.

</td>
</tr>
<tr>
<td>

**[scutum-safe-logging](https://github.com/scutum-defense/scutum-safe-logging)**

Structured safe logging with SafeArg/UnsafeArg. Prevents sensitive data leakage with automatic field detection and redaction guards.

</td>
<td>

**[scutum-audit-chain](https://github.com/scutum-defense/scutum-audit-chain)**

Tamper-evident SHA-256 hash-chained audit trails. Cryptographic verification and tamper detection for command records.

</td>
<td>

**[scutum-eslint-config](https://github.com/scutum-defense/scutum-eslint-config)**

Shared ESLint configuration for defense-grade TypeScript. Bans console.log, eval, enforces complexity limits and strict types.

</td>
</tr>
<tr><td colspan="3"><h3>Simulation & Geospatial</h3></td></tr>
<tr>
<td>

**[scutum-twin](https://github.com/scutum-defense/scutum-twin)**

Digital twin simulation. Validate proposed actions against infrastructure models before execution. Outcomes: safe, unsafe, uncertain, degraded.

</td>
<td>

**[scutum-geo](https://github.com/scutum-defense/scutum-geo)**

Geospatial primitives. Zone classification, corridor deviation, threat corridor projection, haversine, point-in-polygon.

</td>
<td>

</td>
</tr>
<tr><td colspan="3"><h3>Platform & Integration</h3></td></tr>
<tr>
<td>

**[scutum-event-kit](https://github.com/scutum-defense/scutum-event-kit)**

Type-safe event bus with middleware pipeline, typed subscriptions, and the Scutum event protocol (12 event types).

</td>
<td>

**[scutum-schemas](https://github.com/scutum-defense/scutum-schemas)**

Canonical schema registry. 15 versioned schemas across events, entities, workflows, and geospatial primitives.

</td>
<td>

**[scutum-codegen](https://github.com/scutum-defense/scutum-codegen)**

Contract-first code generation. TypeScript interfaces + clients and Python Pydantic models from schema definitions.

</td>
</tr>
<tr><td colspan="3"><h3>SDKs & Developer Tools</h3></td></tr>
<tr>
<td>

**[scutum-sdk](https://github.com/scutum-defense/scutum-sdk)**

TypeScript SDK. Type-safe API client, SSE event streaming, authentication, and domain types.

</td>
<td>

**[scutum-python-sdk](https://github.com/scutum-defense/scutum-python-sdk)**

Python SDK. Sync and async clients with Pydantic v2 validation, mypy strict, tested across Python 3.10–3.12.

</td>
<td>

**[scutum-cli](https://github.com/scutum-defense/scutum-cli)**

Command-line interface. Platform health, incident inspection, audit trail queries, validation.

</td>
</tr>
<tr><td colspan="3"><h3>Deployment & Infrastructure</h3></td></tr>
<tr>
<td>

**[scutum-terraform-provider](https://github.com/scutum-defense/scutum-terraform-provider)**

Terraform provider for zones, corridors, detection rules, policies — infrastructure-as-code for the platform.

</td>
<td>

**[scutum-helm](https://github.com/scutum-defense/scutum-helm)**

Kubernetes Helm charts for sovereign single-tenant deployment. Network policies, security contexts, sovereignty config.

</td>
<td>

**[scutum-starter-app](https://github.com/scutum-defense/scutum-starter-app)**

React starter template. Pre-built hooks and components for building applications on the Scutum platform.

</td>
</tr>
<tr><td colspan="3"><h3>Engineering Standards</h3></td></tr>
<tr>
<td>

**[scutum-engineering-guide](https://github.com/scutum-defense/scutum-engineering-guide)**

Style guides for TypeScript, API design, security, testing, and defense-specific patterns (human-in-loop, audit chain, policy gate, twin validation).

</td>
<td></td>
<td></td>
</tr>
</table>

<br>

## Architecture

```
┌────────────────────────────────────────────────────────────────────────────────┐
│                          SCUTUM COMMAND PLATFORM                              │
│                                                                                │
│    Operator Surfaces                                                           │
│    ┌────────────┐  ┌────────────┐  ┌────────────┐  ┌────────────┐            │
│    │  Command   │  │  Decision  │  │  Twin      │  │  Audit &   │            │
│    │  Console   │  │  Workspace │  │  Validation│  │  Sovereignty│            │
│    └─────┬──────┘  └─────┬──────┘  └─────┬──────┘  └─────┬──────┘            │
│          └───────────────┴───────────────┴───────────────┘                     │
│                            Event Bus (event-kit)                               │
│          ┌───────────────┬───────────────┬───────────────┐                     │
│    ┌─────┴─────┐   ┌─────┴─────┐   ┌─────┴─────┐   ┌─────┴─────┐           │
│    │  Signal   │   │  AI COA   │   │  Approval  │   │  Audit    │           │
│    │  Ingestion│   │  Engine   │   │  Service   │   │  Logger   │           │
│    └───────────┘   └───────────┘   └───────────┘   └───────────┘           │
│                                                                                │
│    Core Libraries                                                              │
│    ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐        │
│    │ detect │ │ policy │ │ audit  │ │  twin  │ │  geo   │ │  safe  │        │
│    │  +packs│ │ engine │ │ chain  │ │        │ │        │ │ logging│        │
│    └────────┘ └────────┘ └────────┘ └────────┘ └────────┘ └────────┘        │
│                                                                                │
│    ┌───────────────────────────────────────────────────────────────────┐       │
│    │  event-kit · schemas · codegen · eslint-config · engineering-guide│       │
│    └───────────────────────────────────────────────────────────────────┘       │
│                                                                                │
│    SDKs & Integration                                                          │
│    ┌───────────────────────────────────────────────────────────────────┐       │
│    │  sdk (TS) · python-sdk · cli · terraform-provider · starter-app  │       │
│    └───────────────────────────────────────────────────────────────────┘       │
│                                                                                │
│    Infrastructure                                                              │
│    ┌───────────────────────────────────────────────────────────────────┐       │
│    │  PostgreSQL · Redis · Docker · Helm · Sovereign Single-Tenant    │       │
│    └───────────────────────────────────────────────────────────────────┘       │
└────────────────────────────────────────────────────────────────────────────────┘
```

<br>

## Principles

| | |
|:--|:--|
| **Sovereign by default** | All data, compute, and audit trails remain within national boundaries. Single-tenant. No shared infrastructure. |
| **Human-in-the-loop** | No autonomous action without explicit operator authorization. AI recommends, humans decide. |
| **Auditable by design** | Every decision produces a hash-chained, policy-labeled, tamper-evident record. |
| **Safe by construction** | No OT write without twin validation. Policy engine enforces safety at every boundary. |
| **One platform** | One ontology, one release train. Extend through schemas and detection packs, not forks. |
| **Open core** | Defense primitives are open source. Product platform is proprietary. |

<br>

## Engineering Standards

Every repository ships with CI/CD, security scanning (CodeQL + TruffleHog), automated dependency updates (Renovate), CODEOWNERS, semantic versioning, and changelogs. See the [engineering guide](https://github.com/scutum-defense/scutum-engineering-guide) for our TypeScript, API design, security, testing, and defense pattern standards.

<br>

---

<div align="center">

Abu Dhabi, UAE &nbsp;&nbsp;·&nbsp;&nbsp; [scutum.defense](https://scutum.defense)

</div>
