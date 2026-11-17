# Communication Plan: RCHN Patient Intake and Scheduling System


**Consultant:** Arianna McGhee


**Role:** Project Manager, NovaTech Consulting


**Engagement:** RCHN


**Date:** November 16, 2026

---

## Communication Matrix

### Entry 1
**Stakeholder:** RCHN Executive Stakeholder
**Information Needed:** Triggered by the conclusion of each accounting period to review overall project health, financial burn rate against major budget milestones, and top-tier portfolio risks.
**Timing / Trigger:** Monthly project review meetings.
**Frequency:** Monthly
**Format:** Executive summary
**Owner:** Project Manager
**Method:** Push

### Entry 2
**Stakeholder:** Marcus Webb, RCHN Project Sponsor
**Information Needed:** Triggered by bi-weekly sprint reviews to evaluate completed milestone deliverables, approve major scope or workflow adjustments, and track budget allocation.
**Timing / Trigger:** Bi-weekly sponsor touchpoints.
**Frequency:** Bi-weekly
**Format:** Status email
**Owner:** Project Manager
**Method:** Push

### Entry 3
**Stakeholder:** RCHN Compliance Officer
**Information Needed:** Triggered whenever a new regulatory policy review or security workflow change is initiated, requiring verification of audit trails and risk status.
**Timing / Trigger:** As new regulatory or compliance reviews are triggered.
**Frequency:** As-needed
**Format:** Compliance checklist
**Owner:** Associate Consultant
**Method:** Pull

### Entry 4
**Stakeholder:** Clinic Intake Coordinators
**Information Needed:** Triggered at the start of each daily shift to receive immediate updates on front-line workflow adjustments, software patches, and patient scheduling instructions.
**Timing / Trigger:** Daily standups and shift changes.
**Frequency:** Daily
**Format:** Plain-language briefing
**Owner:** Scrum Master
**Method:** Push

### Entry 5
**Stakeholder:** NovaTech Delivery Team / Developers
**Information Needed:** Triggered by sprint transition milestones and daily blockers to align on technical specs, active user stories, and backlog progression.
**Timing / Trigger:** Sprint planning and daily scrum syncs.
**Frequency:** Daily / Sprint milestone
**Format:** Shared work view
**Owner:** Scrum Master
**Method:** Interactive

### Communication Method Justification
* **Entry 3:** I chose Pull for the RCHN Compliance Officer because their need for regulatory updates, audit trails, and risk status is event-driven and variable rather than constant. This means a Pull approach (via a self-service compliance checklist) is appropriate because it allows the compliance officer to access detailed tracking and documentation on-demand precisely when audits or security reviews are triggered, avoiding unnecessary noise during stable periods.
* **Entry 5:** I chose Interactive for the NovaTech Delivery Team / Developers because backlogs, technical specs, and daily blockers require continuous two-way collaboration and real-time problem-solving. This means an Interactive approach (via daily scrum syncs and shared work views) is appropriate because it enables developers to actively negotiate user stories, align on technical dependencies, and immediately resolve day-to-day delivery impediments.

---

## Escalation Path

* **Level 1 (Scrum Master):** Handles issues that can be resolved at the team level within **24 hours**. Triggered when day-to-day sprint blockers, minor resource scheduling overlaps, or technical dependencies arise between NovaTech developers and clinic intake coordinators that the immediate team can negotiate and clear.
* **Level 2 (Project Manager / Associate Consultant):** Handles issues that require client-side involvement or cross-functional coordination. Triggered when unresolved technical bottlenecks, scope creeps, or workflow discrepancies impact the schedule or require formal approval from RCHN stakeholders. **Expected response time:** Within **48 hours**.
* **Level 3 (Project Sponsor Marcus Webb & RCHN Executive Leadership):** Handles issues that require executive decision-making, budget reallocations, or major contractual sign-offs. Triggered when critical project risks materialize that exceed the Project Manager's authority, or when unresolved Level 2 disputes threaten key project milestones. **Expected response time:** Within **3 to 5 business days**.

### Escalation Scenario
If **Risk #4 (Integration delay due to legacy EMR data formatting incompatibilities)** from the Week 9 Risk Register materialized, the escalation would unfold as follows:
1. **Step 1:** The Scrum Master (Level 1) would lead daily sprint standups to attempt internal code-level data parsing workarounds and coordinate developers to map legacy patient intake fields within a **24-hour** window.
2. **Step 2:** If the legacy EMR API endpoints remain incompatible and block sprint progress beyond **48 hours**, the Project Manager (Level 2) would step in to coordinate directly with the RCHN Clinic Intake Coordinators and technical liaisons to secure alternative sample data feeds or formal requirement adjustments.
3. **Step 3:** The final escalation level would involve Project Sponsor Marcus Webb and RCHN Executive Leadership (Level 3) because prolonged legacy integration failure would threaten critical budget milestones and project delivery dates, requiring executive decisions on schedule adjustments or vendor scope changes.

---

## Connection to Prior Artifacts

* **Connection to Week 4 stakeholder register:** My communication plan entry for the **RCHN Executive Stakeholder** was shaped by their **high interest and high influence** classification because their decision authority requires a predictable, monthly Push delivery of executive summaries to ensure major budget milestones and portfolio risks are consistently reviewed without demanding manual data retrieval.
* **Connection to Week 8 project schedule:** The **integration and testing phase** from Week 8 drove my decision to **increase the frequency and shift to an Interactive format** for the **NovaTech Delivery Team / Developers** because the tight deadlines for resolving data parsing dependencies require daily scrum syncs and real-time shared work views to maintain development velocity.
* **Connection to Week 9 risk register:** My escalation path was shaped by **Risk #4 (Integration delay due to legacy EMR data formatting incompatibilities)** from the risk register because if this risk materializes, it creates immediate technical roadblocks that exceed team-level authority, triggering our structured 3-level escalation sequence from the Scrum Master up to Project Sponsor Marcus Webb.

---

## Gap Analysis

### Communication Gap
* **The gap I identified in my communication plan is** that we currently lack a formal, recurring communication trigger or designated stakeholder channel for frontline clinic staff and patient representatives to provide qualitative feedback on system usability during active sprint rollouts. 
* **This matters for the RCHN engagement because** while Clinic Intake Coordinators receive daily operational briefings, the day-to-day users (such as intake desk personnel interacting directly with patients) experience immediate friction points that may not surface during high-level Scrum syncs, potentially leading to user resistance or slow adoption of the new intake system. 
* **To fix this gap I would add/change** a bi-weekly "Usability & Feedback Check-In" format owned by the Scrum Master, pushed to frontline clinic staff, because it directly captures ground-level workflow friction before minor user frustrations compound into major adoption barriers.

### Silence as a Communication Decision
* **A situation where NovaTech silence could create a stakeholder problem is** during a multi-week backend data-migration sprint where no visible user-facing interface changes are occurring for the RCHN Project Sponsor, Marcus Webb, or executive stakeholders. 
* **Even though the project is on track,** Marcus Webb might assume that development has stalled, that technical risks are unmanaged, or that NovaTech lacks transparency regarding budget burn during these quiet engineering phases. 
* **My communication plan prevents this by** maintaining our predictable bi-weekly Push status email cadence and monthly executive summaries, which explicitly highlight backend engineering milestones, architecture progress, and risk mitigations even when no new front-end features are being released.

---

*NovaTech Consulting | IT 3310 | Governors State University | Fall 2026*
