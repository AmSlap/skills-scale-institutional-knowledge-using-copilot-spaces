# OctoAcme Project Management Docs

This README provides a brief overview of OctoAcme's project management processes and links to the detailed process documents in this folder.

---

## How OctoAcme Manages Projects

OctoAcme delivers cross-functional projects through a structured, repeatable **lifecycle**:

**Initiation → Planning → Execution/Tracking → Release/Deployment → Retrospective/Continuous Improvement**

Work begins with a **Project One-pager/Charter** that defines the problem, SMART objectives, success metrics, stakeholders, milestones, risks, and resourcing. A decision gate ensures alignment before moving to planning.

**Key roles and personas:**
- **Project Manager (PM)** — coordinates delivery, schedules, risks, and stakeholder communications.
- **Product Manager (PdM/Product Lead)** — defines outcomes, prioritizes the backlog, and measures success.
- **Developers** — implement features, write tests, and collaborate through code review.
- **Technical Lead / Engineering Lead** — provides technical direction, architecture decisions, and mentorship.
- **QA / Test Engineer** — validates quality and acceptance criteria; owns quality gates.
- **UX / UI Designer** — leads user research, prototyping, and design consistency.
- **Release Manager** — owns end-to-end release coordination and go/no-go decisions.
- **Security / AppSec Engineer** — embeds security practices and validates security posture before release.
- **SRE / DevOps Engineer** — owns CI/CD pipelines, infrastructure, reliability, and incident response.
- **Data Analyst** — defines and tracks metrics; supports data-driven decision-making.
- **Customer Support / Support Lead** — surfaces customer feedback and incidents; participates in release reviews.
- **Stakeholders / Sponsor** — provide inputs, approvals, and executive oversight.

See [Roles and Personas](octoacme-roles-and-personas.md) for full definitions, responsibilities, and cross-role interactions.

---

## Key Workflows

- **Backlog management:** Work is broken into shippable increments with explicit **acceptance criteria**, estimates, and a **Definition of Done**.
- **Project board:** Columns follow **Backlog → Ready → In Progress → In Review → QA → Done**.
- **PR workflow:** Small, focused PRs linked to issues and acceptance criteria; CI checks (tests, linting, security scanning) must pass; at least one approval required before merge.
- **Risk management:** Risks tracked in a **Risk Register** (impact/likelihood, owner, mitigation, status); escalation path: Team → PM → Product Lead → Sponsor. Security incidents follow a dedicated handling procedure.

---

## Communication & Status

- **Daily standups** and **weekly delivery syncs** keep the team aligned.
- **End-of-sprint demos/reviews** share progress with stakeholders.
- **Monthly stakeholder updates** use a standard status template (progress, next steps, risks/blockers, decisions needed).
- A single source of truth (project board + docs) reduces duplication and confusion.

---

## Quality Assurance & Release Practices

- **QA:** Unit and integration tests, E2E smoke tests before release, automated security scanning, and manual QA when needed.
- **Releases:** Pre-release checklist (acceptance criteria met, release notes drafted, rollback plan defined, staging validation passed), automated production deployment, post-deploy verification, and stakeholder announcement.
- **Incidents:** Rollback/incident playbook used to restore service and conduct a post-mortem.

---

## Continuous Improvement

After each sprint, release, milestone, or incident the team runs a **retrospective** (what went well, what to improve, owned action items). Action items are tracked in the backlog to drive ongoing process evolution.

---

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, core roles, key artifacts, and lifecycle summary |
| [Project Initiation Guide](octoacme-project-initiation.md) | One-pager/charter template, decision gates, and initiation checklist |
| [Project Planning](octoacme-project-planning.md) | Kickoff, backlog setup, milestones, dependencies, and Definition of Done |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Project board workflow, standups, delivery rhythm, and status reporting |
| [Risk Management & Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, communication templates |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Release checklist, deployment steps, rollback playbook, release notes template |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retro structure, action item tracking, and improvement cadence |
| [Roles and Personas](octoacme-roles-and-personas.md) | Detailed responsibilities and communication patterns for each role |
| [RACI Matrix Template](octoacme-raci-matrix-template.md) | Ownership matrix mapping all personas to project lifecycle activities |
| [Phase Handoff Checklist](octoacme-phase-handoff-checklist.md) | Required artefacts and sign-offs at each lifecycle phase transition |
| [Stakeholder Communication & Escalation Guide](octoacme-stakeholder-communication-and-escalation.md) | Communication cadence, escalation paths, and message templates |
