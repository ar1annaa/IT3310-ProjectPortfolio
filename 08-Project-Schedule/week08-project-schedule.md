# Project Schedule: RCHN Patient Intake and Scheduling System
**Consultant:** Arianna McGhee


**Role:** Associate Consultant, Project Manager, NovaTech Consulting

**Engagement:** RCHN


**Date:** October 27, 2026

---

## Work Breakdown Structure

### Grouping 1: Project Initiation and Setup
- Initial stakeholder requirements gathering and scope baseline approval across all six clinic locations
- Project governance and communication channel establishment
- Resource allocation and team role assignments for the multi-clinic deployment

### Grouping 2: Project Planning and Backlog Preparation
- Standardize required intake fields architecture and validation rules
- Draft patient identity and record confirmation workflow wireframes and scheduling interface specifications
- Define missing intake information flagging logic and warning notification specifications

### Grouping 3: System Development and Configuration
- Core patient database schema and secure contact information update module
- Front-end appointment calendar availability and scheduling conflict warning engine
- Automated SMS and email appointment reminder notification triggers

### Grouping 4: Clinic Deployment and Project Closure
- Execute User Acceptance Testing (UAT) and resolve and review critical defects with clinic managers/stakeholders across all six locations
- Conduct staff training program and distribute user documentation across all six clinic locations
- Final simultaneous go-live deployment across all six RCHN clinics and formal project closure sign-off

### WBS Rationale
My WBS directly represents the scope established in Week 5 by focusing exclusively on foundational delivery areas: project setup, planning and backlog preparation, system development across our six clinic locations, and final deployment. Making sure that every week's work and progress is intentional helps me understand direction, alignment, and rationalizes the strict boundaries needed to protect our core schedule across all six RCHN clinics. One notable scope item from Week 5 that was intentionally excluded from this WBS is the executive reporting dashboard for clinic leadership. This item was intentionally left out because developing custom executive analytics would significantly increase project complexity, consume valuable technical resources, and risk delaying our core schedule. Given that our primary project goals center entirely on standardizing intake and streamlining appointment scheduling across all six RCHN clinics, executive analytics are not an immediate priority for Phase One and have been appropriately excluded to keep the project on time and within budget.

---

## Task Dependencies

- Standardize required intake fields architecture and validation rules → Core patient database schema and secure contact information update module, Finish-to-Start
- Core patient database schema and secure contact information update module → Front-end appointment calendar availability and scheduling conflict warning engine, Start-to-Start
- Deploy and start running the new RCHN cloud-based scheduling and intake platform → Decommission legacy scheduling software across all six clinic locations, Start-to-Finish

### Dependency Logic
If the predecessor activity, "standardizing the required intake fields architecture and validation rules," slipped by two weeks, it would directly block the start of the core patient database schema and secure contact information update module. Because database developers cannot build or finalize tables without these defined field rules, downstream technical execution would halt. This two-week slip would directly push back front-end calendar UI development, system integration, and UAT across all six clinic locations. Because the RCHN project mandates a simultaneous multi-clinic go-live rather than a staggered rollout, there is zero schedule float available to absorb this delay, meaning the final deployment milestone would face a direct two-week delay. To reduce this impact, the team could attempt fast-tracking by starting preliminary database mock-ups using estimated field rules, though this carries a high risk of technical rework from not having every requirement outlined.

---

## Activity Schedule

| ID | Activity | Duration (working days) | Predecessors | Start week |
|---|---|---:|---|---:|
| A | Standardize intake fields and validation rules | 5 | None | 1 |
| B | Build core intake database schema and information validation | 10 | A | 2 |
| C | Develop calendar scheduling interface | 10 | A,B | 4 |
| D | Prepare and execute multi-clinic UAT and user training | 10 | C | 6 |

### Scheduling Assumptions
Durations were based off my experience where two weeks has usually been the standard sprint time, giving us enough space for meetings to get clarification and make sure we understand our objectives while still leaving plenty of actual work time for the team. Predecessors were chosen because of logical technical flow, where foundational requirements like standardizing intake fields have to be completely finished before dependent tasks like building the database schema can start because they rely on each other. One uncertainty that could change this schedule is that I don't know the exact headcount or size of the team, so I don't know if a two-week window will actually be enough time for everyone to work efficiently.

---

## Milestones

- All six clinic intake workflows configured and tested, End of Sprint 3 (Week 5): All clinic managers have signed off on the standardized intake workflow configuration and User Acceptance Testing (UAT) results show zero critical defects across all six locations.
- Staff training completed and go-live deployment authorized, End of Sprint 4 (Week 6): Staff across all six RCHN clinics have completed mandatory system training with 90% or higher user satisfaction on feedback surveys, and leadership has given final sign-off for simultaneous go-live deployment.

### Critical Path Analysis
For the practice network, Path A → B → D totals 9 days ($3 + 4 + 2$) and Path A → C → D totals 11 days ($3 + 6 + 2$). The critical path is A → C → D with a total project duration of 11 days, because it represents the longest path through the network. If any activity on this path slips by two days, the entire project duration will increase by two days to 13 days due to zero float. This calculation differs from my RCHN schedule, which uses RCHN's deployment tasks measured in weeks rather than an abstract network with arbitrary letter IDs.

---

## Schedule Reflection

### Scope Connection
My WBS Phase 3 (System Development and Configuration) directly goes hand in hand with the scope established in Week 5 by focusing on the core technical building blocks needed for our multi-clinic rollout, specifically the core database schema, the calendar scheduling interface, and automated reminder triggers. These lower-level work packages support this portion of the project by ensuring that all development efforts remain strictly aligned with replacing the legacy scheduling and intake software across all six RCHN locations without slipping into out-of-scope features like mobile apps or executive dashboards.

### Objective Connection
Milestone 2 (Staff training completed and go-live deployment authorized) directly supports our Week 5 SMART Objective 2, which requires front desk staff and clinic managers across all six RCHN clinics to successfully complete mandatory system training verified by 90% or higher user satisfaction ratings on feedback surveys. Because the connection between training completion and formal go-live authorization is already established through our operational transition plan, the primary additional confirmation needed before final sign-off is ensuring that clinic management has officially cleared staff coverage so that training sessions do not disrupt daily patient care operations.

---
*NovaTech Consulting | IT 3310 | Governors State University | Fall 2026*
