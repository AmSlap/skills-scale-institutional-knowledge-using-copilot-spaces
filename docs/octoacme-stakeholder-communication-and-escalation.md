# OctoAcme Stakeholder Communication Cadence & Risk Escalation Guide

This document makes communication ownership and escalation paths explicit so every persona knows what to send, to whom, and how often — and what to do when something goes wrong.

Persona definitions: see [Roles and Personas](octoacme-roles-and-personas.md).
Phase ownership: see [Phase Handoff Checklist](octoacme-phase-handoff-checklist.md).

---

## Stakeholder Communication Cadence Checklist

Use this as a running checklist throughout the project. Check off each cadence item when the communication is sent or the meeting is held.

### Weekly Cadence

| Communication | Owner | Audience | Format | Checklist |
|---|---|---|---|:---:|
| Weekly status update (scope, schedule, risk RAG) | Project Manager | Sponsor, Stakeholders, Product Manager | Written report or project board update | ☐ |
| Product / backlog sync | Product Manager | Project Manager, Technical Lead | Meeting or async message | ☐ |
| Engineering sync | Technical Lead | Developers, SRE / DevOps | Meeting or async | ☐ |
| Support digest (top issues and trends) | Customer Support / Support Lead | Product Manager, Project Manager | Written digest | ☐ |
| QA / defect summary | QA / Test Engineer | Project Manager, Product Manager, Technical Lead | Defect dashboard or written summary | ☐ |
| Metrics snapshot | Data Analyst | Product Manager, Project Manager | Dashboard link or written snapshot | ☐ |

### Sprint / Iteration Cadence

| Communication | Owner | Audience | Format | Checklist |
|---|---|---|---|:---:|
| Sprint planning | Project Manager (facilitates) | Full delivery team | Meeting | ☐ |
| Daily standup | Project Manager (facilitates) | Developers, QA / Test Engineer, UX / UI Designer, Technical Lead | Meeting (15 min max) | ☐ |
| Sprint demo / review | Product Manager (facilitates) | Stakeholders, Sponsor (optional), full team | Meeting + recording | ☐ |
| Retrospective | Project Manager (facilitates) | Full delivery team | Meeting | ☐ |
| Sprint action items distributed | Project Manager | Named owners | Written (issue tracker or doc) | ☐ |

### Monthly / Milestone Cadence

| Communication | Owner | Audience | Format | Checklist |
|---|---|---|---|:---:|
| Executive / stakeholder briefing | Project Manager | Sponsor, senior stakeholders | Slide deck or executive summary | ☐ |
| Roadmap update | Product Manager | Stakeholders, Technical Lead, Project Manager | Roadmap doc or slide | ☐ |
| Security posture report | Security / AppSec Engineer | Project Manager, Sponsor (if required) | Written report | ☐ |
| SLO / reliability report | SRE / DevOps Engineer | Project Manager, Technical Lead | Dashboard or written report | ☐ |
| Analytics / outcomes review | Data Analyst | Product Manager, Project Manager | Metrics report or slide | ☐ |

### Release-Specific Communications

| Communication | Owner | Audience | Timing | Checklist |
|---|---|---|---|:---:|
| Release readiness summary (go/no-go inputs) | Release Manager | Project Manager, QA, Security, SRE/DevOps | T−2 business days | ☐ |
| Go/no-go decision communicated | Release Manager | All stakeholders | Day of release window | ☐ |
| Pre-release notification | Release Manager | Customers / end-users (via Support Lead) | T−1 business day | ☐ |
| Post-release status | Release Manager | All stakeholders | Within 2 hours of deployment | ☐ |
| Customer release notes | Product Manager | Customers (via Support Lead) | At or before deployment | ☐ |

---

## Risk Escalation Quick Reference

Use this matrix to determine how quickly to escalate a risk or issue and who to loop in.

### Escalation Severity Levels

| Level | Description | Response Time | Examples |
|---|---|---|---|
| **P0 — Critical** | Production is down or a release is blocked; business impact is immediate | Immediate (< 1 hour) | Site outage, data loss incident, critical security vulnerability in production |
| **P1 — High** | Significant risk to release timeline, quality, or key deliverable; customer impact likely | Same business day (< 4 hours) | P1 defect blocking release, security finding with no accepted risk, key dependency missed |
| **P2 — Medium** | Risk is real but manageable with mitigation; schedule impact is possible | Next business day | Scope creep request, unresolved technical debt, third-party integration delay |
| **P3 — Low** | Monitor; unlikely to affect schedule or quality without mitigation | Weekly review | Minor blockers, team availability concerns, documentation gaps |

---

### Escalation Path by Risk Type

| Risk Category | First Contact | Escalation 1 | Escalation 2 | Comms Owner |
|---|---|---|---|---|
| **Technical / Architecture** | Technical Lead | Project Manager | Sponsor (if timeline at risk) | Project Manager |
| **Quality / Defect** | QA / Test Engineer | Technical Lead | Project Manager → Release Manager | Project Manager |
| **Security Vulnerability** | Security / AppSec Engineer | Technical Lead + Project Manager | Sponsor (P0/P1 only) | Security / AppSec + Project Manager |
| **Release / Deployment** | Release Manager | SRE / DevOps Engineer + Project Manager | Sponsor (P0 only) | Release Manager |
| **Infrastructure / Reliability** | SRE / DevOps Engineer | Technical Lead | Project Manager → Sponsor | Project Manager |
| **Scope / Requirements** | Product Manager | Project Manager | Sponsor (budget/timeline impact) | Project Manager |
| **Resource / Staffing** | Project Manager | Sponsor | — | Project Manager |
| **Customer / Support** | Customer Support / Support Lead | Product Manager | Project Manager | Project Manager |
| **Compliance / Regulatory** | Security / AppSec Engineer | Project Manager | Sponsor + Legal | Project Manager |
| **Third-Party / Vendor** | Project Manager | Technical Lead (if technical) | Sponsor (if contractual) | Project Manager |

---

### Escalation Checklist (Use for Every P0/P1)

When a P0 or P1 risk or incident occurs, work through this checklist:

- [ ] **Identify**: Confirm severity level (P0 or P1) and risk type using the table above
- [ ] **Notify First Contact**: Alert the named first contact within the required response time
- [ ] **Open an incident or risk item**: Create a tracked item (GitHub Issue or risk register entry) with:
  - Description of the risk/incident
  - Business impact and affected systems/personas
  - Current severity and justification
  - Owner assigned
  - Next action and expected resolution time
- [ ] **Loop in Escalation 1**: Brief Escalation 1 contact within the required window
- [ ] **Update stakeholders**: Project Manager sends a brief update to relevant stakeholders (see Communication Cadence above)
- [ ] **Escalate to Sponsor** if the risk meets the Escalation 2 criteria (see table above)
- [ ] **Resolve or accept risk**: Document the resolution or risk acceptance decision and owner in the risk register
- [ ] **Post-incident review** (P0 only): Schedule a blameless post-mortem within 5 business days; share findings with the team

---

## Communication Templates

### Weekly Status Update (Project Manager → Stakeholders)

```
## Project Status — [Project Name] — Week of [Date]

**Overall RAG Status**: 🟢 Green / 🟡 Amber / 🔴 Red

**Summary**
[2–3 sentence summary of progress this week]

**Highlights**
- [Key accomplishment 1]
- [Key accomplishment 2]

**Risks / Issues**
| Risk/Issue | Severity | Owner | Mitigation | Status |
|---|---|---|---|---|
| | | | | |

**Next Week**
- [Planned activity 1]
- [Planned activity 2]

**Decisions Needed**
- [Decision or approval required, by whom, by when]
```

---

### Go / No-Go Release Communication (Release Manager → All Stakeholders)

```
## Go/No-Go Decision — [Release Name / Version] — [Date]

**Decision**: ✅ GO / ❌ NO-GO

**Release Window**: [Date & Time (UTC)]
**Environments**: [Staging / Production]

**Quality Gate Summary**
| Gate | Status | Owner | Notes |
|---|---|---|---|
| QA Sign-off | ✅ / ❌ | QA / Test Engineer | |
| Security Sign-off | ✅ / ❌ | Security / AppSec | |
| Rollback Tested | ✅ / ❌ | SRE / DevOps | |

**Known Issues Accepted**
- [Issue description, severity, rationale for acceptance]

**Rollback Trigger**: [Condition that will trigger rollback]
**Rollback Owner**: [SRE / DevOps Engineer name]

**Next Communication**: Post-release status within 2 hours of deployment.
```

---

### Risk Escalation Brief (Project Manager → Sponsor)

```
## Risk Escalation Brief — [Project Name] — [Date]

**Severity**: P0 / P1
**Risk Type**: [Technical / Quality / Security / Scope / etc.]

**Summary**
[1–2 sentences: what is the risk and what is the business impact?]

**Current Status**
[What has been done so far to address it?]

**Decision / Support Needed**
[What specifically does the Sponsor need to decide, approve, or unblock?]

**Options**
1. [Option A] — Impact: [x] — Owner: [y]
2. [Option B] — Impact: [x] — Owner: [y]

**Recommended Action**: [Recommendation and rationale]
**Response Needed By**: [Date / Time]
```
