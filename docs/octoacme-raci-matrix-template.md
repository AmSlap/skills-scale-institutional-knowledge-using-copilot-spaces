# OctoAcme RACI Matrix Template

Use this template to assign ownership for key activities across the project lifecycle. Fill in the matrix for each project or workstream. Adjust personas as needed to reflect your team structure.

**Key:**
| Symbol | Meaning |
|--------|---------|
| **R** | **Responsible** — does the work |
| **A** | **Accountable** — owns the outcome; one per row |
| **C** | **Consulted** — provides input before or during the work |
| **I** | **Informed** — receives updates after decisions are made |

Persona definitions: see [Roles and Personas](octoacme-roles-and-personas.md).

---

## Project Lifecycle RACI

| Activity | Project Manager | Product Manager | Technical Lead | Developers | QA / Test Engineer | UX / UI Designer | Release Manager | Security / AppSec | SRE / DevOps | Data Analyst | Customer Support | Sponsor / Exec |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **INITIATION** | | | | | | | | | | | | |
| Draft project charter / one-pager | **A** | C | C | | | | | | | | | I |
| Define success metrics and KPIs | C | **A** | C | | | | | | | R | | I |
| Identify stakeholders and sponsors | **A** | C | | | | | | | | | | C |
| Conduct initial risk assessment | **A** | C | C | C | | | | C | C | | | I |
| Obtain charter approval (gate) | C | C | | | | | | | | | | **A** |
| **PLANNING** | | | | | | | | | | | | |
| Define scope and acceptance criteria | C | **A** | C | C | C | C | | C | | | | I |
| Create project plan and milestones | **A** | C | C | | | | | | | | | I |
| Design UX / UI prototypes | C | C | C | C | | **A** | | | | | | I |
| Produce technical architecture | C | C | **A** | R | | | | C | C | | | I |
| Security threat modelling | C | C | C | C | | | | **A** | C | | | I |
| Set up CI/CD and environments | C | | C | C | | | C | | **A** | | | |
| Define test strategy and test plan | C | C | C | C | **A** | | | C | | | | |
| Define analytics instrumentation plan | C | **A** | C | C | | | | | | R | | |
| Kickoff meeting facilitation | **A** | C | C | C | C | C | C | C | C | C | C | I |
| **EXECUTION & TRACKING** | | | | | | | | | | | | |
| Feature development | I | C | C | **A** | | C | | | | | | |
| Code review and merge | I | | **A** | R | | | | C | | | | |
| Test execution and defect reporting | I | C | | C | **A** | | | | | | | |
| Defect triage and resolution | C | C | C | **A** | C | | | C | | | C | |
| Sprint status reporting | **A** | C | C | | | | | | | | | I |
| Risk register maintenance | **A** | C | C | C | C | | | C | C | | C | I |
| Stakeholder status updates | **A** | C | | | | | | | | | | I |
| Usability / UAT review | C | C | | C | C | **A** | | | | | C | I |
| Analytics tracking validation | C | C | C | R | C | | | | | **A** | | |
| **RELEASE & DEPLOYMENT** | | | | | | | | | | | | |
| Release readiness review (go/no-go) | C | C | C | C | C | | **A** | C | C | | C | I |
| Security sign-off | C | | C | | C | | C | **A** | | | | I |
| QA sign-off | C | C | C | C | **A** | | C | | | | | |
| Deployment execution | I | | C | C | | | **A** | | R | | | |
| Release communications | C | C | | | | | **A** | | | | C | I |
| Post-deployment verification | C | | C | C | C | | **A** | | R | C | C | I |
| **RETROSPECTIVE & CLOSE** | | | | | | | | | | | | |
| Retrospective facilitation | **A** | C | C | C | C | C | C | C | C | C | C | I |
| Action item tracking | **A** | C | | | | | | | | | | I |
| Metrics review and close report | C | **A** | | | | | | | | R | | I |
| Knowledge base / doc updates | C | C | C | R | R | R | C | C | C | C | **A** | |

---

## How to Use This Template

1. **Copy this table** into your project's planning document or project board wiki.
2. **Replace persona columns** with the names of actual team members where helpful.
3. **Review every row**: there must be exactly one **A** per activity. If you find two, resolve the conflict before work begins.
4. **Share and agree**: walk through the RACI in the project kickoff meeting so every stakeholder understands their role.
5. **Update as the team evolves**: revisit during sprint planning if ownership changes.

---

## Tips

- If a cell is blank, that persona has no defined involvement. That is intentional — avoid over-communicating or over-consulting.
- When in doubt about R vs C, ask: *"Does this person produce a work product or make a decision?"* (R) vs *"Does this person give input but not own the output?"* (C).
- Keep the RACI aligned with the [Phase Handoff Checklist](octoacme-phase-handoff-checklist.md) to ensure sign-off owners match accountability in this matrix.
