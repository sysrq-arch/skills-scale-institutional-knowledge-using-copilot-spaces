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

### Interactions with Other Roles
- **Product Manager**: Clarify acceptance criteria and scope changes; surface technical constraints early.
- **Project Manager**: Provide effort estimates, flag risks, and report progress against milestones.
- **UX Designer**: Review mockups and prototypes; raise feasibility concerns before implementation begins.
- **DevOps Engineer**: Coordinate deployment readiness and environment requirements.
- **Technical Writer**: Review draft documentation for technical accuracy.
- **Security Engineer**: Respond to security findings and integrate recommended controls into code.

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

### Interactions with Other Roles
- **Project Manager**: Align on scope, timeline, and trade-offs; escalate blockers together.
- **UX Designer**: Co-define user research goals; review prototypes and validate against success metrics.
- **Technical Writer**: Provide feature context and user-facing copy for release notes and help content.
- **Security Engineer**: Review threat model impacts on product decisions; balance security requirements against delivery timelines.

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

### Interactions with Other Roles
- **Product Manager**: Align on priorities, scope, and decisions; co-own stakeholder communications.
- **Developers**: Communicate timelines and dependencies; unblock teams from process or resource constraints.
- **DevOps Engineer**: Plan deployment windows, coordinate release readiness, track infrastructure dependencies.
- **Technical Writer**: Ensure documentation milestones are included in the project plan and met before release.

---

## UX Designer

### Role Summary
UX Designers are responsible for user research, interaction design, and prototyping. They ensure that products are usable, accessible, and aligned with user needs throughout the project lifecycle.

### Responsibilities
- Conduct user research (interviews, usability tests, surveys) to inform design decisions
- Create wireframes, interaction designs, and high-fidelity prototypes
- Define and maintain design systems and accessibility standards
- Collaborate with Product Managers to translate requirements into user flows
- Provide developers with design specifications and assets
- Participate in design critiques and user-acceptance testing

### Goals
- Deliver intuitive, accessible, and delightful user experiences
- Reduce friction and support task completion for end users
- Maintain consistency across the product interface

### Typical Communication
- Design reviews and critique sessions with cross-functional team
- Annotated mockups and prototype links shared in project boards
- Usability test findings summaries

### Interactions with Other Roles
- **Product Manager**: Collaborate early on problem framing; validate designs against success metrics and user feedback.
- **Developers**: Provide detailed specifications and assets; review implemented UI against designs before release.
- **Project Manager**: Surface design milestones and flag dependency on early feedback cycles.
- **Technical Writer**: Coordinate on in-product copy, error messages, and onboarding flows to ensure consistent voice.

---

## DevOps Engineer

### Role Summary
DevOps Engineers maintain CI/CD pipelines, infrastructure, and deployment processes. They bridge development and operations to ensure reliable, scalable, and repeatable delivery.

### Responsibilities
- Design, build, and maintain CI/CD pipelines for automated testing and deployment
- Manage cloud infrastructure, environments (dev, staging, production), and configuration
- Monitor system health, set up alerting, and lead incident response for infrastructure issues
- Automate repetitive operational tasks to improve reliability and efficiency
- Collaborate with Security Engineers to implement infrastructure-level security controls
- Document deployment runbooks and operational procedures

### Goals
- Achieve fast, reliable, and low-risk deployments
- Maximize system uptime and observability
- Enable self-service infrastructure capabilities for the development team

### Typical Communication
- Deployment runbooks and operational playbooks in the docs/ directory
- Incident retrospectives and post-mortems
- Infrastructure change requests and release readiness sign-offs

### Interactions with Other Roles
- **Developers**: Define CI/CD pipeline requirements together; support developers with local environment parity and tooling.
- **Security Engineer**: Implement infrastructure security controls (secrets management, network policies, scanning); address findings from infrastructure audits.
- **Project Manager**: Provide deployment window recommendations and flag infrastructure risks in the risk register.
- **Product Manager**: Communicate release readiness constraints and capacity impacts on delivery timelines.

---

## Technical Writer

### Role Summary
Technical Writers document APIs, user-facing features, internal processes, and onboarding material. They ensure all audiences — end users, developers, and stakeholders — can find and understand the information they need.

### Responsibilities
- Write and maintain end-user documentation, release notes, and help content
- Document internal APIs, developer guides, and integration instructions
- Create and improve onboarding guides for new team members
- Collaborate with subject matter experts to review drafts for accuracy
- Maintain the docs/ directory structure and documentation style guide
- Support cross-team communication by standardizing templates and processes

### Goals
- Reduce time-to-productivity for new team members and users
- Improve discoverability and accuracy of technical and process documentation
- Maintain a consistent voice and structure across all documentation

### Typical Communication
- Pull requests for documentation updates reviewed by subject-matter experts
- Documentation review sessions before release milestones
- Style guide and documentation standards shared with the team

### Interactions with Other Roles
- **Developers**: Request technical reviews of API and feature documentation; align on code examples and integration steps.
- **Product Manager**: Obtain feature context for user-facing content and release notes.
- **UX Designer**: Coordinate in-product copy and microcopy to ensure a consistent tone and terminology.
- **Project Manager**: Confirm documentation tasks are tracked and scheduled before release gates.

---

## Security Engineer

### Role Summary
Security Engineers identify and mitigate security risks across the software lifecycle. They integrate security practices into design, development, and operations to protect the product and its users.

### Responsibilities
- Conduct threat modeling and security risk assessments for new features and infrastructure changes
- Perform security reviews of code, architecture, and third-party dependencies
- Define and maintain security standards, policies, and remediation guidance
- Collaborate with DevOps Engineers to implement security controls in CI/CD pipelines and infrastructure
- Triage and prioritize vulnerabilities; track remediation to closure
- Support incident response for security events

### Goals
- Shift security left by integrating it early in the development lifecycle
- Minimize the risk of security incidents and data exposure
- Build a culture of security awareness and shared responsibility

### Typical Communication
- Threat model documents and security review findings shared with affected teams
- Vulnerability reports and remediation tracking in the risk register
- Security standards and guidelines in the docs/ directory

### Interactions with Other Roles
- **Developers**: Provide actionable remediation guidance; review security-sensitive code changes.
- **DevOps Engineer**: Define infrastructure security requirements (secret rotation, network segmentation, scanning); validate controls are in place before production deployments.
- **Product Manager**: Communicate security risks that affect feature scope or release readiness.
- **Project Manager**: Escalate security findings that affect project timelines; ensure security milestones are included in release plans.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Refer to [Onboarding & Handoff Guide](octoacme-onboarding-and-handoff.md) for checklists that apply to each role.

