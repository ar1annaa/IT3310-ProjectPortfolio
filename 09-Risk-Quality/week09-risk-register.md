# Risk Register: RCHN Patient Intake and Scheduling System

**Consultant:** Arianna McGhee  
**Role:** Associate Consultant, Project Manager, NovaTech Consulting  
**Engagement:** RCHN  
**Date:** October 30, 2026  

---

## Risk Entries

Risk 1: If appointment data discrepancies identified during migration are not fully reconciled before go-live, then the RCHN project will experience immediate double-booking errors and patient scheduling conflicts across multiple clinics, undermining data integrity.

Risk 2: If the two lagging clinic locations fail to complete mandatory staff training prior to deployment, then front desk staff will struggle with the new intake and scheduling workflows, leading to severe operational bottlenecks and disrupted patient care.

Risk 3: If local high-speed internet bandwidth and network stability checks are not verified across all six clinic locations prior to cutover, then the cloud-based intake and scheduling platform will suffer from latency spikes, dropped sessions, or connection timeouts during peak morning intake hours, disrupting patient check-ins.

Risk 4: If required-field validation rules fail to be strictly enforced across all patient records during high-volume intake hours, then the central database will accumulate unstandardized and missing data inconsistencies.

Risk 5: If we decide to do a phased rollout and don't fix all issues in the 1st pilot clinic, then we will spend time correcting that clinic's errors and using the pilot launch as a time to remediate issues in the 5 remaining clinics.

---

## Bring Forward

Week 5 assumptions: We are assuming that all six RCHN clinic locations currently have reliable high-speed internet access capable of supporting a cloud-based intake and scheduling platform. If this is wrong, then the technical implementation schedule and hardware budget will need to change to account for local infrastructure upgrades before deployment. Additionally, we are assuming that clinic management will release front desk staff for mandatory training without disrupting daily patient care operations. If this is wrong, then our training schedule and resource plan will need to change to include phased or after-hours training sessions.

Week 7 backlog item: As a clinic intake coordinator, I want intake forms to enforce strict required-field validation across all patient records, so that we eliminate missing data inconsistencies and ensure every submission is standardized before it reaches the central database.

Week 8 schedule item: Milestone: All six clinic intake workflows configured and tested, End of Sprint 3 (Week 5): All clinic managers have signed off on the standardized intake workflow configuration and User Acceptance Testing (UAT) results show zero critical defects across all six locations.

---

## Assumption Connection

Risk 2 connects to my Week 5 assumption that clinic management would release front desk staff for mandatory training without disrupting daily patient care operations. This became a risk because the uncertainty around whether clinics can maintain daily patient volumes while pulling staff off the floor creates a high probability that training completion will lag behind schedule, which could directly affect Smart Objective 2, requiring front desk staff and clinic managers across all six RCHN clinics to successfully complete mandatory system training verified by 90% or higher user satisfaction ratings on feedback surveys prior to deployment authorization. 

Risk 3 connects to my Week 5 assumption that all six RCHN clinic locations currently have reliable high-speed internet access capable of supporting a cloud-based intake and scheduling platform. This became a risk because the uncertainty regarding local IT infrastructure and bandwidth limits across older facilities creates the threat of latency spikes, dropped sessions, or connection timeouts during peak intake hours, directly affecting our go-live readiness and operational reliability objectives, risking severe check-in bottlenecks and compromising data integrity during the initial system cutover.

---

## Probability, Impact, and Scoring

| # | Risk Description (Summary) | Probability | Impact | Score | Priority |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1** | Unresolved migration data discrepancies | High (3) | High (3) | **9** | Higher Priority |
| **2** | Incomplete staff training at lagging clinics | High (3) | Medium (2) | **6** | Higher Priority |
| **3** | Local clinic internet infrastructure gaps | Medium (2) | High (3) | **6** | Higher Priority |
| **4** | Required-field validation inconsistencies | Low (1) | Medium (2) | **2** | Lower Priority |
| **5** | Phased pilot rollout error remediation overlap | Medium (2) | High (3) | **6** | Higher Priority |

For Risk 1 (Unresolved migration data discrepancies), I rated probability as High because appointment data discrepancies have already been identified during migration in the project briefing. I rated impact as High because corrupt or inaccurate patient data directly threatens patient safety, clinical workflows, and core data accuracy standards. For Risk 5 (Phased pilot rollout error remediation overlap), I rated probability as Medium because pilot testing inherently uncovers unforeseen technical and operational defects that require active correction. I rated impact as High because failing to fully resolve pilot clinic errors before cascading changes to the remaining five facilities risks compounding defects across the entire RCHN network.

---

## Response Strategies

Risk 1 Strategy (Mitigate): The team will execute a 100% data scrubbing and reconciliation pass on all migrated appointment records. Trigger: Discovery of duplicate or mismatched patient appointment IDs during pre-migration testing.

Risk 2 Strategy (Mitigate): The team will establish flexible, phased, or after-hours training sessions and provide targeted coaching to the two lagging clinic facilities. Trigger: Failure of a clinic's staff to meet the mandatory training completion threshold 7 days prior to launch.

Risk 3 Strategy (Mitigate): The team will perform a pre-deployment network bandwidth and ping-latency audit across all six clinics and provision redundant cellular failover hotspots. Trigger: A network stress test or staging simulation revealing connection timeout rates exceeding 2% or packet loss during peak simulated user loads.

Risk 4 Strategy (Avoid): The development team will hardcode strict required-field validation logic into the intake form architecture so submissions cannot bypass missing fields. Trigger: Identification of optional field bypasses during front-end form testing.

Risk 5 Strategy (Mitigate): The project team will establish a dedicated 48-hour stabilization and hotfix sprint immediately following the pilot launch at Clinic X to resolve all uncovered errors before releasing configuration packages to the remaining five clinics. Trigger: Identification of more than three critical or high-severity workflow defects during the pilot clinic run.

---

## Owner Assignments

Risk 1 Owner: Developer, because this role is responsible for executing database scripts and resolving backend data integration and migration anomalies.

Risk 2 Owner: Product Manager, because this role oversees user acceptance, stakeholder alignment, and training curriculum readiness across all clinic locations.

Risk 3 Owner: Project Manager, because managing overarching technical infrastructure requirements, third-party vendor coordination, and deployment resource allocations across multiple facilities falls directly under project governance.

Risk 4 Owner: Developer, because this role directly builds and enforces the user interface validation rules and schema constraints.

Risk 5 Owner: Project Manager, because overseeing overall deployment scheduling, milestone gating, and cross-clinic transition sequencing falls directly under project governance.

---

## Risk Reflection and GitHub Update

### Highest Priority Risk and Project Impact
My highest-priority threat is Risk 1 (Unresolved migration data discrepancies) with a course score of 9 (High). It deserves the most attention because it directly threatens system reliability and clinical trust. If it occurred, it could affect quality and go-live readiness by causing widespread scheduling errors and unverified patient records; schedule by forcing emergency remediation sprints that violate our zero-float timeline; and stakeholder confidence by shaking the trust of executive sponsor Marcus Webb and clinical staff during the initial rollout.

### Risk vs. Issue Distinction
After reviewing my five risks, I verified that Risks 1, 2, and 4 function as active issues because executive sponsor Marcus Webb explicitly confirmed in the briefing that appointment data discrepancies, incomplete staff training at two clinic locations, and incomplete acceptance testing are current problems happening today. In contrast, Risk 3 (local clinic internet infrastructure bandwidth and latency degradation during peak morning intake hours) and Risk 5 (phased pilot rollout error remediation overlap) function as true future uncertainties, because they describe conditional future events—such as potential network timeout rates and pilot clinic stabilization outcomes—that we are projecting and planning for rather than experiencing as active outages today. 

This distinction matters because an issue requires immediate, direct operational intervention and escalation to resolve current roadblocks, whereas a risk requires proactive mitigation strategies, contingency planning, and trigger monitoring to prevent potential future failures before they disrupt go-live readiness.

---
*NovaTech Consulting | IT 3310 | Governors State University | Fall 2026*
