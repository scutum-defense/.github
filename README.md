<div align="center">

<!-- Replace with actual logo when available -->
<img src="https://via.placeholder.com/200x200.png?text=SCUTUM" alt="Scutum Defense" width="200" />

# Scutum Defense

**Sovereign Infrastructure Defense OS**

![GitHub Org](https://img.shields.io/badge/org-scutum--defense-1a1a2e?style=for-the-badge&logo=github)
![Repos](https://img.shields.io/badge/repositories-5-blue?style=for-the-badge)
![Security Policy](https://img.shields.io/badge/security-policy--enforced-critical?style=for-the-badge&logo=shield)
![Access](https://img.shields.io/badge/access-private-red?style=for-the-badge&logo=lock)

---

*Protecting critical national infrastructure through AI-driven situational awareness, human-authorized decision-making, and sovereign-grade auditability.*

</div>

---

## Mission

Scutum builds the operating system for sovereign infrastructure defense. We fuse multi-modal signals into a unified operating picture, generate ranked courses of action, require human authorization before execution, validate outcomes through digital twin simulation, and produce an auditable command trail -- all deployed within sovereign boundaries.

**Current Wedge:** Port and logistics continuity command.

---

## Engineering Principles

| Principle | Description |
|:--|:--|
| **Sovereign by default** | All data, compute, and audit trails remain within sovereign boundaries |
| **Human-in-the-loop** | No autonomous action without explicit operator authorization |
| **Auditability first** | Every decision, approval, and execution produces an immutable record |
| **Signal fusion** | Multi-modal inputs converge into a single operating picture |
| **Defense-grade reliability** | If realism and reliability conflict, choose reliability |

---

## Repository Map

| Repository | Purpose | Stack |
|:--|:--|:--|
| [`scutum-mvp`](https://github.com/scutum-defense/scutum-mvp) | Production MVP -- operator console, API, domain models | Next.js, Fastify, TypeScript, pnpm monorepo |
| [`scutum-demo`](https://github.com/scutum-defense/scutum-demo) | Investor demo -- interactive fundraising artifact | Next.js, TypeScript, playback engine |
| [`scutum-docs`](https://github.com/scutum-defense/scutum-docs) | Architecture, governance, ADRs, security baselines | Markdown, ADR format |
| [`scutum-infra`](https://github.com/scutum-defense/scutum-infra) | Infrastructure-as-code, environments, policy automation | IaC modules, CI/CD pipelines |
| [`.github`](https://github.com/scutum-defense/.github) | Org-wide standards, templates, workflows | GitHub Actions, issue templates |

---

## Org Standards

This `.github` repository defines organization-wide defaults that apply across all Scutum repositories:

- **Pull Request Templates** -- standardized PR format and review expectations
- **Issue Templates** -- feature requests, bug reports, security reviews, ADR requests
- **Security Policy** -- vulnerability reporting and responsible disclosure
- **CODEOWNERS** -- mandatory review gates on all critical paths
- **Workflow Hygiene** -- baseline CI checks enforced across the org

---

## Security & Access

| Policy | Status |
|:--|:--|
| All critical repos private | Enforced |
| Direct push to protected branches | Blocked |
| CODEOWNERS review | Mandatory |
| Secrets in code | Prohibited |
| README + CODEOWNERS per repo | Required |

---

<div align="center">

![Built with](https://img.shields.io/badge/built_with-TypeScript-3178C6?style=flat-square&logo=typescript)
![Platform](https://img.shields.io/badge/platform-sovereign_cloud-1a1a2e?style=flat-square)
![Status](https://img.shields.io/badge/status-active_development-brightgreen?style=flat-square)

**Scutum Defense** -- Sovereign Infrastructure Protection

</div>
