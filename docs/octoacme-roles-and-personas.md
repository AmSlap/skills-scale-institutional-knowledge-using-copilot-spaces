# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA / Test Engineer

### Role Summary
QA / Test Engineers own quality assurance across the project lifecycle. They design and execute test strategies, surface defects, and act as the quality gate before releases reach production.

### Responsibilities
- Define and maintain test plans, test cases, and acceptance criteria coverage
- Execute manual and automated tests (functional, regression, integration, performance)
- Track, triage, and verify defects in the issue tracker
- Own the definition and enforcement of quality gates for each release
- Contribute to the Definition of Done alongside Developers and the Project Manager

### Goals
- Prevent defect leakage to production
- Reduce regression risk through broad automated test coverage
- Provide fast, actionable feedback to Developers

### Typical Communication
- Daily standups and sprint reviews alongside Developers
- Defect reports and test summary documents shared with Project Manager and Product Manager
- Pre-release sign-off communicated to Release Manager and Project Manager

### Interactions with Existing Roles
- **Developers**: pairs on testability, reviews code for edge cases, validates fixes immediately.
- **Product Managers**: aligns test cases to acceptance criteria; escalates ambiguous requirements.
- **Project Managers**: surfaces quality risks and test-blocking blockers; contributes to risk register.
- **Stakeholders**: presents quality metrics and test outcomes in sprint reviews.

---

## UX / UI Designer

### Role Summary
UX / UI Designers ensure that solutions are user-centred by conducting research, creating wireframes and prototypes, and maintaining design consistency across the product.

### Responsibilities
- Lead user research, personas, journey mapping, and usability testing
- Produce wireframes, high-fidelity mockups, and interactive prototypes
- Define and maintain the design system and UI components
- Collaborate with Product Managers to translate user needs into actionable requirements
- Participate in sprint reviews to validate that implemented UIs match design intent

### Goals
- Deliver intuitive, accessible, and consistent user experiences
- Reduce rework caused by late-stage usability feedback
- Bridge user research and engineering through clear design specifications

### Typical Communication
- Design reviews and prototype walkthroughs with Developers and Product Managers
- Usability test findings shared with Product Managers and Project Managers
- Handoff documentation and design specs in shared design tools (e.g., Figma)

### Interactions with Existing Roles
- **Developers**: provides design specs and component guidance; reviews implemented screens together.
- **Product Managers**: co-defines user stories and acceptance criteria; aligns on priorities.
- **Project Managers**: flags design-blocking dependencies or scope changes that affect timelines.
- **Stakeholders**: presents prototypes and usability findings to gather early feedback.

---

## Technical Lead / Engineering Lead

### Role Summary
The Technical Lead provides technical direction and oversight for the engineering team. They make architectural decisions, remove technical blockers, and ensure code quality and maintainability.

### Responsibilities
- Define and document technical architecture and key design decisions
- Review and approve significant code changes and pull requests
- Identify and mitigate technical risks and technical debt
- Guide and mentor Developers on best practices and standards
- Coordinate with the Release Manager on deployment readiness and hotfix strategy

### Goals
- Maintain a coherent, scalable, and secure technical architecture
- Unblock developers and reduce re-work through early technical guidance
- Ensure engineering output meets quality and performance standards

### Typical Communication
- Architecture decision records (ADRs) and design documents
- Code review feedback and technical spike write-ups
- Regular syncs with Project Manager and Product Manager on technical feasibility and trade-offs

### Interactions with Existing Roles
- **Developers**: provides day-to-day technical mentorship, review, and unblocking.
- **Product Managers**: translates technical constraints and trade-offs into product-level implications.
- **Project Managers**: flags technical risks, estimates, and resource needs.
- **Stakeholders**: presents technical architecture and security posture in design reviews.

---

## Release Manager

### Role Summary
The Release Manager owns the end-to-end release process, coordinating planning, execution, and communications across all teams to ensure safe, repeatable deployments.

### Responsibilities
- Maintain the release calendar and coordinate release windows with all stakeholders
- Confirm all release criteria (quality gates, sign-offs, rollback plans) are met before deployment
- Manage deployment pipelines and coordinate with SRE / DevOps on environment readiness
- Communicate release status and post-deployment results to the team and stakeholders
- Own rollback decisions and incident coordination during and immediately after releases

### Goals
- Deliver releases on schedule with minimal production incidents
- Ensure consistent, documented, and auditable release practices
- Reduce mean-time-to-recovery (MTTR) when releases cause issues

### Typical Communication
- Release readiness emails and go/no-go meeting facilitation
- Post-release reports and incident summaries
- Coordination with QA, SRE/DevOps, and Project Manager via release tracking boards

### Interactions with Existing Roles
- **Developers**: receives build artefacts and confirms code freeze adherence.
- **Product Managers**: aligns release scope with approved features and release notes.
- **Project Managers**: keeps release milestones visible in the project plan; escalates blockers.
- **Stakeholders**: issues advance release notifications and post-release status updates.

---

## Security / AppSec Engineer

### Role Summary
Security / AppSec Engineers embed security practices throughout the project lifecycle, from threat modelling in planning to vulnerability assessments before release.

### Responsibilities
- Conduct threat modelling and security design reviews for new features
- Perform or coordinate static analysis (SAST), dependency scanning, and penetration testing
- Triage and track security findings to resolution in collaboration with Developers
- Define and enforce security standards and secure-coding guidelines
- Advise on compliance, privacy, and regulatory requirements

### Goals
- Prevent the introduction of security vulnerabilities into production
- Reduce time-to-remediation for identified security issues
- Foster a shift-left security culture across engineering

### Typical Communication
- Security review reports and threat model documents shared with Technical Lead and Project Manager
- Vulnerability findings triaged in the issue tracker with severity and owner assigned
- Pre-release security sign-off communicated to Release Manager

### Interactions with Existing Roles
- **Developers**: provides secure-coding guidance, reviews code for security flaws, assists with remediation.
- **Product Managers**: surfaces security trade-offs that affect prioritisation or release timelines.
- **Project Managers**: adds security tasks to the risk register and tracks remediation progress.
- **Stakeholders**: reports on security posture and compliance status in appropriate forums.

---

## SRE / DevOps Engineer

### Role Summary
SRE / DevOps Engineers own the reliability, scalability, and operability of the systems delivered by the project. They build and maintain CI/CD pipelines, infrastructure-as-code, and observability tooling.

### Responsibilities
- Design, implement, and maintain CI/CD pipelines and deployment automation
- Define and monitor Service Level Objectives (SLOs) and alert on Service Level Indicators (SLIs)
- Manage cloud infrastructure, environments, and secrets securely
- Lead incident response, post-mortems, and reliability improvements
- Collaborate with Developers and Release Manager on deployment strategies (canary, blue/green, etc.)

### Goals
- Maximise system reliability and minimise toil through automation
- Enable fast, safe deployments with instant rollback capability
- Provide high-signal observability to all teams

### Typical Communication
- Runbooks and infrastructure documentation in the project repository
- On-call alerts, incident bridges, and post-mortem reports
- Environment status updates to Project Manager and Release Manager during release windows

### Interactions with Existing Roles
- **Developers**: partners on CI/CD configuration, containerisation, and local dev environment setup.
- **Product Managers**: provides reliability data that informs prioritisation of infrastructure work.
- **Project Managers**: surfaces environment or infrastructure risks; reports SLO health.
- **Stakeholders**: presents reliability metrics and incident trends in operational reviews.

---

## Data Analyst

### Role Summary
Data Analysts define, collect, and interpret project and product metrics to inform decisions at every stage of the project lifecycle.

### Responsibilities
- Define success metrics and KPIs in collaboration with Product Managers
- Instrument analytics and ensure tracking coverage for new features
- Analyse data to surface insights, trends, and anomalies for the team
- Prepare dashboards and reports for stakeholder reviews and retrospectives
- Support A/B test design, statistical analysis, and interpretation of results

### Goals
- Ensure every major decision is grounded in data rather than assumptions
- Reduce time from data question to actionable insight
- Maintain a trustworthy, well-documented data environment

### Typical Communication
- Weekly metrics reports and executive dashboards shared with Project Manager and Product Manager
- A/B test read-outs and retrospective data summaries
- Data model documentation and tracking specifications in the project repository

### Interactions with Existing Roles
- **Developers**: collaborates on event instrumentation, data pipelines, and analytics tooling.
- **Product Managers**: provides data to validate hypotheses, prioritise backlog, and measure OKRs.
- **Project Managers**: supplies objective progress indicators and helps measure project health.
- **Stakeholders**: presents outcome metrics in business reviews to demonstrate value delivered.

---

## Customer Support / Support Lead

### Role Summary
Customer Support / Support Leads represent the voice of the customer within the project team. They collect, triage, and escalate user feedback and incidents to ensure customer experience is considered in every decision.

### Responsibilities
- Collect and categorise user feedback, bug reports, and support tickets
- Identify patterns and recurring issues and escalate them to the appropriate team
- Participate in release reviews to flag known customer-impacting issues
- Contribute to user acceptance testing (UAT) using real-world customer scenarios
- Maintain a knowledge base and FAQs in sync with product changes

### Goals
- Reduce customer-impacting defects that reach production
- Close the feedback loop between customers and the delivery team
- Minimise support ticket volume through proactive documentation and quality

### Typical Communication
- Weekly support digest and trend reports shared with Project Manager and Product Manager
- Escalation tickets with severity and customer impact details
- Participation in release go/no-go discussions to confirm known issues are acceptable

### Interactions with Existing Roles
- **Developers**: shares reproduction steps and customer context for defect triaging.
- **Product Managers**: surfaces high-impact customer pain points to inform prioritisation.
- **Project Managers**: flags customer-impacting risks and participates in risk register reviews.
- **Stakeholders**: contributes customer satisfaction data to executive and business reviews.

---

## Sponsor / Executive Stakeholder

### Role Summary
Sponsors and Executive Stakeholders provide strategic direction, secure funding and resources, and act as the final decision-making authority for high-impact trade-offs and escalations.

### Responsibilities
- Champion the project at the executive level and secure necessary budget and headcount
- Approve project charter, major scope changes, and milestone gates
- Remove organisational blockers that are beyond the Project Manager's authority
- Participate in executive-level status reviews and provide strategic guidance
- Sign off on go/no-go decisions for major releases

### Goals
- Ensure the project delivers measurable business value aligned with strategic objectives
- Maintain executive visibility and confidence in project health
- Resolve cross-functional conflicts and resource contention quickly

### Typical Communication
- Monthly or milestone-based executive briefings from Project Manager
- Exception reports and escalation briefs when risks exceed defined thresholds
- Approval emails or decision log entries for gate decisions

### Interactions with Existing Roles
- **Developers**: minimal day-to-day interaction; engages during all-hands or major demos.
- **Product Managers**: aligns product strategy and OKRs with business objectives; approves roadmap changes.
- **Project Managers**: primary contact for status reporting, escalation, and gate approvals.
- **Stakeholders**: peer-level engagement with other business unit leaders and external partners.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Reference the [RACI Matrix Template](octoacme-raci-matrix-template.md) to map these personas to ownership for each phase.
- Use the [Phase Handoff Checklist](octoacme-phase-handoff-checklist.md) to see which personas sign off at each lifecycle transition.
- Consult the [Stakeholder Communication & Escalation Guide](octoacme-stakeholder-communication-and-escalation.md) for cadence and escalation paths per persona.

