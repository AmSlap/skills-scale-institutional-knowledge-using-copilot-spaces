# OctoAcme Phase Handoff Checklist

Use this checklist to confirm that all required artefacts exist and sign-offs are obtained before progressing to the next lifecycle phase. A phase cannot officially start until all items from the previous phase are checked off.

> **How to use**: Copy the relevant section into your project tracking tool (e.g., GitHub Issue, project board checklist). Assign each sign-off item to the named persona. Record the date and approver name next to each completed item.

Persona definitions: see [Roles and Personas](octoacme-roles-and-personas.md).
RACI context: see [RACI Matrix Template](octoacme-raci-matrix-template.md).

---

## Phase 1 → Phase 2: Initiation → Planning

**Trigger**: Project charter approved; team assembled.

### Required Artefacts
- [ ] Project Charter / One-pager published in the project repository
- [ ] SMART objectives and success metrics defined
- [ ] Stakeholder list documented (name, role, contact, engagement level)
- [ ] Initial risk register created with at least the top three risks identified
- [ ] High-level timeline and key milestones agreed

### Sign-offs Required
| Artefact | Sign-off Owner | Date | Notes |
|---|---|---|---|
| Project Charter | **Sponsor / Executive Stakeholder** | | |
| Success Metrics | **Product Manager** | | |
| Risk Register (initial) | **Project Manager** | | |
| Stakeholder List | **Project Manager** | | |

### Gate Question
> *"Do we have a clear, approved problem statement, a named team, and executive sponsorship to proceed into detailed planning?"*

---

## Phase 2 → Phase 3: Planning → Execution & Tracking

**Trigger**: All planning artefacts complete; kickoff meeting held.

### Required Artefacts
- [ ] Sprint/iteration backlog created with prioritised, estimated items
- [ ] Acceptance criteria written for all items in the first sprint
- [ ] Definition of Done (DoD) agreed and published
- [ ] Technical architecture documented (ADR or design doc)
- [ ] Test strategy and test plan drafted
- [ ] UX prototypes reviewed and approved by Product Manager
- [ ] Security threat model completed for new features
- [ ] CI/CD pipeline and environments provisioned and verified
- [ ] Analytics instrumentation plan agreed
- [ ] RACI matrix populated and reviewed in kickoff

### Sign-offs Required
| Artefact | Sign-off Owner | Date | Notes |
|---|---|---|---|
| Backlog & Acceptance Criteria | **Product Manager** | | |
| Definition of Done | **Technical Lead** | | |
| Technical Architecture | **Technical Lead** | | |
| Test Plan | **QA / Test Engineer** | | |
| UX Prototypes | **UX / UI Designer** | | |
| Threat Model | **Security / AppSec Engineer** | | |
| Environments Ready | **SRE / DevOps Engineer** | | |
| Kickoff Complete | **Project Manager** | | |

### Gate Question
> *"Does the team have everything needed to start building, testing, and tracking progress immediately?"*

---

## Phase 3 → Phase 4: Execution & Tracking → Release & Deployment

**Trigger**: All planned work complete or explicitly descoped; release criteria met.

### Required Artefacts
- [ ] All committed sprint items closed or formally descoped (with Product Manager approval)
- [ ] All P0/P1 defects resolved; P2 defects triaged and accepted or deferred
- [ ] QA test cycle complete; test summary report available
- [ ] Security review completed; no open critical or high findings without accepted risk
- [ ] Performance and load testing completed (if applicable)
- [ ] Release notes drafted and reviewed
- [ ] Rollback plan documented and tested
- [ ] Deployment runbook reviewed and up to date
- [ ] Go/no-go meeting facilitated; outcome recorded

### Sign-offs Required
| Artefact | Sign-off Owner | Date | Notes |
|---|---|---|---|
| Test Summary Report | **QA / Test Engineer** | | |
| Security Clearance | **Security / AppSec Engineer** | | |
| Release Notes | **Product Manager** | | |
| Rollback Plan | **SRE / DevOps Engineer** | | |
| Go/No-Go Decision | **Release Manager** | | |
| Stakeholder Notification Sent | **Project Manager** | | |

### Gate Question
> *"Is the product safe to release? Are all quality gates passed, rollback rehearsed, and stakeholders notified?"*

---

## Phase 4 → Phase 5: Release & Deployment → Retrospective & Close

**Trigger**: Deployment to production complete and stable; post-deployment verification passed.

### Required Artefacts
- [ ] Deployment completed and recorded (timestamp, version, environments)
- [ ] Post-deployment monitoring checks passed (SLOs within threshold for agreed period)
- [ ] Release announcement / customer communications sent
- [ ] Known issues log updated (any deferred defects or follow-up items captured)
- [ ] Support team briefed on new features and known issues
- [ ] Metrics baselines updated (Data Analyst confirms)

### Sign-offs Required
| Artefact | Sign-off Owner | Date | Notes |
|---|---|---|---|
| Post-Deployment Verification | **SRE / DevOps Engineer** | | |
| Release Communications | **Release Manager** | | |
| Support Team Briefing | **Customer Support / Support Lead** | | |
| Metrics Baseline Updated | **Data Analyst** | | |
| Phase Close Confirmation | **Project Manager** | | |

### Gate Question
> *"Is the release stable, communicated, and the team ready to shift focus to learning and improvement?"*

---

## Phase 5: Retrospective & Close

**Trigger**: Release confirmed stable; retrospective scheduled.

### Required Artefacts
- [ ] Retrospective meeting held (all key personas invited)
- [ ] Action items captured with named owner and due date
- [ ] Metrics review completed (outcomes vs. success metrics from initiation)
- [ ] Lessons learned document published in the project repository
- [ ] Process docs updated with any improvements identified
- [ ] Project formally closed in the tracking tool

### Sign-offs Required
| Artefact | Sign-off Owner | Date | Notes |
|---|---|---|---|
| Action Items (with owners) | **Project Manager** | | |
| Metrics Close Report | **Product Manager** | | |
| Lessons Learned Doc | **Project Manager** | | |
| Project Closed | **Sponsor / Executive Stakeholder** | | |

### Gate Question
> *"Have we captured what worked, what didn't, and who is responsible for the agreed improvements?"*

---

## Quick Reference: Who Signs Off What

| Phase Transition | Primary Sign-off | Secondary Sign-off |
|---|---|---|
| Initiation → Planning | Sponsor / Executive Stakeholder | Project Manager |
| Planning → Execution | Product Manager, Technical Lead | Project Manager |
| Execution → Release | Release Manager (go/no-go) | QA / Test Engineer, Security / AppSec |
| Release → Retro | SRE / DevOps (stability) | Release Manager |
| Retro / Close | Sponsor / Executive Stakeholder | Project Manager |
