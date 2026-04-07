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

### Sovereign Infrastructure Defense Operating System

<br>

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-202020?style=for-the-badge&logo=fastify&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

<br>

[![Repos](https://img.shields.io/badge/repositories-9-0a0d12?style=flat-square&labelColor=243242)](#repository-map)
[![Security](https://img.shields.io/badge/security-policy_enforced-0a0d12?style=flat-square&labelColor=243242)](#security--governance)
[![Status](https://img.shields.io/badge/status-Sprint_0-0a0d12?style=flat-square&labelColor=243242)](#current-milestone)
[![Deployment](https://img.shields.io/badge/deployment-sovereign_single--tenant-0a0d12?style=flat-square&labelColor=243242)](#)

---

**Protecting critical national infrastructure through AI-driven situational awareness,<br>human-authorized decision-making, and sovereign-grade auditability.**

</div>

<br>

## What Scutum Does

Scutum builds the command layer for nations that need to **detect threats** across critical infrastructure, **decide how to respond** with AI-ranked courses of action, and **defend assets** through human-authorized, digitally-validated execution — all within sovereign boundaries.

```
 SENSE                FUSE                 DECIDE               AUTHORIZE            VALIDATE             AUDIT
 ┌──────────┐        ┌──────────┐        ┌──────────┐        ┌──────────┐        ┌──────────┐        ┌──────────┐
 │  Video   │───┐    │          │        │  Ranked  │        │  Human   │        │  Digital │        │ Immutable│
 │  Thermal │───┤    │  Signal  │───────>│  Course  │───────>│  Operator│───────>│   Twin   │───────>│ Command  │
 │  RF      │───┼───>│  Fusion  │        │  of      │        │  Approval│        │  Gate    │        │  Trail   │
 │  OT/SCADA│───┤    │  Engine  │        │  Action  │        │          │        │          │        │          │
 │  AIS     │───┤    │          │        │          │        │          │        │          │        │          │
 │  ADS-B   │───┘    └──────────┘        └──────────┘        └──────────┘        └──────────┘        └──────────┘
                     One operating                           No autonomous        Safe vs unsafe       Every decision
                     picture                                 execution            path comparison      is traceable
```

<br>

## Core Principles

<table>
<tr>
<td width="33%" valign="top">

### Sovereign by Default
All data, compute, and audit trails remain within national boundaries. Single-tenant deployment. No shared infrastructure. No data leaves sovereign control.

</td>
<td width="33%" valign="top">

### Human-in-the-Loop
No autonomous action without explicit operator authorization. AI recommends, humans decide. Every approval requires identity, rationale, and timestamp.

</td>
<td width="33%" valign="top">

### Auditable by Design
Every signal, decision, approval, and execution produces an immutable, policy-labeled record. Trust is proven through transparency, not assertion.

</td>
</tr>
</table>

<br>

## Repository Map

<table>
<tr>
<td colspan="3"><strong>Product Engineering</strong></td>
</tr>
<tr>
<td width="30%">

**[scutum-mvp](https://github.com/scutum-defense/scutum-mvp)**<br>
![CI](https://github.com/scutum-defense/scutum-mvp/actions/workflows/ci.yml/badge.svg)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/-Next.js-000?style=flat-square&logo=nextdotjs)

</td>
<td width="50%">

Production wedge MVP monorepo. Operator command center, Fastify API with JWT/RBAC, domain ontology, AI COA engine, digital twin simulator, PostgreSQL persistence, real-time SSE event bus.

</td>
<td width="20%" align="center">

`85 files`<br>
`pnpm monorepo`

</td>
</tr>
<tr>
<td>

**[scutum-demo](https://github.com/scutum-defense/scutum-demo)**<br>
![CI](https://github.com/scutum-defense/scutum-demo/actions/workflows/ci.yml/badge.svg)
![Next.js](https://img.shields.io/badge/-Next.js-000?style=flat-square&logo=nextdotjs)

</td>
<td>

Investor demo with deterministic 6-scene narrative. Port-airspace incident scenario, ranked COA, twin validation, audit trail. Separate from production to prevent demo shortcuts in real architecture.

</td>
<td align="center">

`41 files`<br>
`5 scenes`

</td>
</tr>
<tr>
<td colspan="3"><strong>Platform & Integration</strong></td>
</tr>
<tr>
<td>

**[scutum-sdk](https://github.com/scutum-defense/scutum-sdk)**<br>
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Apache 2.0](https://img.shields.io/badge/-Apache_2.0-D22128?style=flat-square)

</td>
<td>

Official TypeScript SDK for platform integration. Type-safe API client, SSE event streaming, authentication helpers, and domain types for incidents, recommendations, and audit records.

</td>
<td align="center">

`13 files`<br>
`API client`

</td>
</tr>
<tr>
<td>

**[scutum-schemas](https://github.com/scutum-defense/scutum-schemas)**<br>
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Apache 2.0](https://img.shields.io/badge/-Apache_2.0-D22128?style=flat-square)

</td>
<td>

Canonical schema registry. Versioned event models, entity types, workflow state machines, and geospatial primitives. Single source of truth for all platform contracts using `scutum.<category>.<name>.v1` convention.

</td>
<td align="center">

`19 files`<br>
`schema registry`

</td>
</tr>
<tr>
<td colspan="3"><strong>Public & Brand</strong></td>
</tr>
<tr>
<td>

**[scutum-website](https://github.com/scutum-defense/scutum-website)**<br>
![Next.js](https://img.shields.io/badge/-Next.js-000?style=flat-square&logo=nextdotjs)
![Tailwind](https://img.shields.io/badge/-Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

</td>
<td>

Public marketing website. Sovereign dark aesthetic, solutions pages for port security, energy infrastructure, and national defense command. Careers and contact.

</td>
<td align="center">

`13 files`<br>
`5 pages`

</td>
</tr>
<tr>
<td>

**[scutum-brand](https://github.com/scutum-defense/scutum-brand)**<br>
![Assets](https://img.shields.io/badge/-Brand_Assets-b99a66?style=flat-square)

</td>
<td>

Brand guidelines, color system (Sovereign Dark + Command Gold palette), typography scale, logo specifications, and templates for presentations, documents, and social media.

</td>
<td align="center">

`12 files`<br>
`brand kit`

</td>
</tr>
<tr>
<td colspan="3"><strong>Operations & Governance</strong></td>
</tr>
<tr>
<td>

**[scutum-docs](https://github.com/scutum-defense/scutum-docs)**<br>
![ADRs](https://img.shields.io/badge/-ADR_tracked-0e8a16?style=flat-square)

</td>
<td>

Architecture Decision Records, ontology documentation, operator workflow definitions, security baselines, deployment patterns, pilot integration notes, governance model, and operational runbooks.

</td>
<td align="center">

`12 files`<br>
`10 categories`

</td>
</tr>
<tr>
<td>

**[scutum-infra](https://github.com/scutum-defense/scutum-infra)**<br>
![Terraform](https://img.shields.io/badge/-IaC-844FBA?style=flat-square&logo=terraform&logoColor=white)

</td>
<td>

Infrastructure-as-code for 4 environments (dev, staging, pilot-port, pilot-energy). Reusable modules for network, identity, storage, observability, and secrets management. Policy-as-code enforcement.

</td>
<td align="center">

`15 files`<br>
`4 environments`

</td>
</tr>
</table>

<br>

## Architecture

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                              SCUTUM COMMAND PLATFORM                                │
│                                                                                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐               │
│  │  Operator   │  │  Decision   │  │  Digital    │  │  Audit &    │   Command      │
│  │  Console    │  │  Workspace  │  │  Twin       │  │  Sovereignty│   Center       │
│  │  (Next.js)  │  │  (COA Panel)│  │  (Validation│  │  (Trail)    │   Web App      │
│  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘               │
│         │                │                │                │                        │
│  ───────┴────────────────┴────────────────┴────────────────┴──────── SSE Bus ──── │
│                                                                                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐               │
│  │  Signal     │  │  AI COA     │  │  Approval   │  │  Audit      │   Fastify      │
│  │  Ingestion  │  │  Engine     │  │  Service    │  │  Logger     │   API           │
│  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘               │
│         │                │                │                │                        │
│  ───────┴────────────────┴────────────────┴────────────────┴──────── Domain ───── │
│                                                                                     │
│  ┌──────────────────────────────────────────────────────────────────────────────┐   │
│  │  @scutum/domain    @scutum/schemas    @scutum/scenario    @scutum/db        │   │
│  │  Ontology v0.1     Event contracts    Seed data           PostgreSQL + ORM   │   │
│  └──────────────────────────────────────────────────────────────────────────────┘   │
│                                                                                     │
│  ┌──────────────────────────────────────────────────────────────────────────────┐   │
│  │  PostgreSQL 16   ·   Redis 7   ·   Docker Compose   ·   Sovereign Infra     │   │
│  └──────────────────────────────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

<br>

## Current Milestone

<table>
<tr>
<td width="25%" align="center">

**Sprint 0**<br>
`April 2026`<br>
![Active](https://img.shields.io/badge/-ACTIVE-brightgreen?style=flat-square)

</td>
<td>

**Objective:** First product repo live with working end-to-end skeleton.

- Monorepo scaffold with operator console, API, and domain ontology
- Seeded scenario: suspicious drone + perimeter incursion at port cluster
- One vertical slice: detect → correlate → recommend → approve → validate → audit
- Release train, CODEOWNERS, CI/CD, and branch protection established
- Design partner identified and integration pack prepared

</td>
</tr>
</table>

**Roadmap**

```
  Apr 2026          May-Jul 2026        Aug-Oct 2026        Nov 2026-Jan 2027    Feb-Apr 2027
  ─────────         ────────────        ────────────        ─────────────────    ────────────
  Sprint 0          Phase 1             Phase 2             Phase 3              Phase 4
  Scaffold &        Foundation &        Integrated          Partner Beta &       Production
  Architecture      First Pilot         Alpha               Multi-sector         MVP
                    Integration                             Expansion
  ▓▓▓▓▓▓▓▓▓▓        ░░░░░░░░░░          ░░░░░░░░░░          ░░░░░░░░░░           ░░░░░░░░░░
```

<br>

## Technology

| Layer | Technology | Purpose |
|:--|:--|:--|
| **Frontend** | Next.js 15, React 19, Tailwind CSS, Mapbox GL | Operator command center and strategic asset map |
| **Backend** | Fastify 5, Node.js 22, TypeScript 5.9 | API server with JWT auth, RBAC, and SSE streaming |
| **Database** | PostgreSQL 16, Drizzle ORM | Mission data persistence and audit storage |
| **Cache / PubSub** | Redis 7 | Real-time event distribution and session cache |
| **AI** | COA Engine, Twin Simulator | Ranked recommendations and outcome validation |
| **Schemas** | TypeScript interfaces, versioned contracts | Platform-wide type safety and schema governance |
| **Infra** | Docker Compose, IaC modules | Environment management and sovereign deployment |
| **CI/CD** | GitHub Actions, pnpm workspaces | Automated build, typecheck, test, and deploy gates |
| **Package Mgmt** | pnpm 10 monorepo | Workspace dependency management and build orchestration |

<br>

## Security & Governance

| Control | Status | Scope |
|:--|:--|:--|
| Private repositories only | ![Enforced](https://img.shields.io/badge/-enforced-brightgreen?style=flat-square) | All repos |
| No direct push to `main` | ![Enforced](https://img.shields.io/badge/-enforced-brightgreen?style=flat-square) | All repos |
| Pull request required | ![Enforced](https://img.shields.io/badge/-enforced-brightgreen?style=flat-square) | All repos |
| CODEOWNERS review gate | ![Enforced](https://img.shields.io/badge/-enforced-brightgreen?style=flat-square) | All repos |
| No secrets in code | ![Enforced](https://img.shields.io/badge/-enforced-brightgreen?style=flat-square) | All repos |
| Domain-based ownership | ![Enforced](https://img.shields.io/badge/-enforced-brightgreen?style=flat-square) | scutum-mvp |
| CI status checks required | ![Enforced](https://img.shields.io/badge/-enforced-brightgreen?style=flat-square) | mvp, demo |
| Architecture Decision Records | ![Active](https://img.shields.io/badge/-active-blue?style=flat-square) | scutum-docs |
| Signed commits | ![Planned](https://img.shields.io/badge/-planned-yellow?style=flat-square) | scutum-infra |

<br>

## Team Structure

```
                              ┌──────────────────┐
                              │   Engineering    │
                              │   Leadership     │
                              └────────┬─────────┘
                                       │
          ┌────────────────────────────┼────────────────────────────┐
          │                            │                            │
  ┌───────┴───────┐          ┌────────┴────────┐          ┌───────┴───────┐
  │   Product     │          │   Platform      │          │   Operations  │
  │   Engineering │          │   & Security    │          │   & Delivery  │
  └───────┬───────┘          └────────┬────────┘          └───────┬───────┘
          │                            │                            │
  ┌───────┼───────┐          ┌────────┼────────┐          ┌───────┼───────┐
  │       │       │          │        │        │          │       │       │
  Data  Mission  AI       Platform  SRE     Crypto     Field  Release  Demo
  Plat  Apps    Decision  Security  Release Assurance  Eng    Mgmt    Strike
  form                                                                Team
```

**16 engineering teams** organized by domain, with architecture council and product leads as cross-cutting governance functions.

<br>

## The Wedge

Scutum is not building a broad platform on day one. We are building **one narrow, production-ready wedge**:

> **Port and Logistics Continuity Command**
>
> One incident family (drone + perimeter incursion). One operator workflow (detect → decide → defend).
> One deployment model (sovereign single-tenant). One design partner. One vertical slice that proves the thesis.

This wedge becomes the spine of the broader platform. The architecture, ontology, and workflow engine are designed to extend into energy, maritime, airspace, and national-scale federation — but only after the wedge is production-proven.

<br>

---

<div align="center">

<br>

```
  One platform. One ontology. One release train.
  Every decision auditable. Every action human-authorized.
  Sovereign by design. Defense-grade by default.
```

<br>

![Scutum Defense](https://img.shields.io/badge/Scutum_Defense-Sovereign_Infrastructure_Defense-0a0d12?style=for-the-badge&labelColor=243242)

<br>

</div>
