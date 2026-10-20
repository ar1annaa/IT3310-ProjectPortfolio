# Product Backlog: RCHN Patient Intake and Scheduling System


**Consultant:** Arianna McGhee


**Role:** Associate Consultant, NovaTech Consulting


**Engagement:** Regional Care Health Network (RCHN)


**Date:** October 14, 2026


---


## Product Backlog


### Story 1


**User Story:** As a Clinic Intake Coordinator, I want to complete intake using a consistent workflow, so that I can reduce re-entry and uncertainty during intake.


**Acceptance Criteria:** Given an intake coordinator is logged into the system, when they open a new patient intake form, then all required standard fields and validation checks will be displayed uniformly across all six clinics to prevent missing data.


**Story Points:** 5 points


**MoSCoW Priority:** Must Have


---


### Story 2


**User Story:** As a Clinic Manager, I want to view appointment status across all six clinics, so that I can identify and resolve scheduling bottlenecks.


**Acceptance Criteria:** Given a clinic manager accesses the scheduling dashboard, when they filter by appointment status across all six clinic locations, then they will see real-time updates to identify booking bottlenecks and wait-time delays.


**Story Points:** 8 points


**MoSCoW Priority:** Won't Have This Time


---


### Story 3


**User Story:** As a Clinic Patient, I want to securely update my intake and insurance information online prior to my appointment, so that I don't have to fill out paper clipboards in the waiting room and can check in faster upon arrival.


**Acceptance Criteria:** Given a pre-filled digital patient form is successfully submitted, when the front-desk staff opens the patient's arrival queue, then the system marks pre-check-in as complete, bypassing manual paper data entry.


**Story Points:** 8 points


**MoSCoW Priority:** Should Have


---


### Story 4


**User Story:** As a clinic patient, I want to receive automated appointment reminders via SMS and email prior to my visit, so that I don't forget my scheduled time and can confirm or reschedule in advance to avoid no-shows.


**Acceptance Criteria:** Given an appointment is successfully scheduled in the system, when the appointment date is 24 hours away, then the system automatically triggers an SMS and email reminder containing the date, time, clinic location, and a direct confirmation/reschedule link.


**Story Points:** 8 points


**MoSCoW Priority:** Should Have


---


### Story 5


**User Story:** As a clinic intake coordinator, I want intake forms to enforce strict required-field validation across all patient records, so that we eliminate missing data inconsistencies and ensure every submission is standardized before it reaches the central database.


**Acceptance Criteria:** Given an intake coordinator is filling out a patient intake form across any of the six clinic locations, when they attempt to save a form with blank or improperly formatted required fields, then the system triggers an inline validation error and blocks submission until all standardized criteria are met.


**Story Points:** 3 points


**MoSCoW Priority:** Must Have


---


## Prioritization Rationale


### Must Have Justification


For our Must-Have priority, I selected RCHN-104 (Flag missing intake information, 3 pts), backed by our clinic intake coordinator user story. This item is essential for the current planning horizon because it directly supports our agreed RCHN delivery condition that we must have accurate, up-to-date information across all six clinic locations before full rollout. However, choosing this as a Must-Have doesn't automatically mean it has to be crammed into Sprint 1. 


We have to tackle this ticket in a deliberate, step-by-step structure—we need the core intake field skeleton completely established first before we can layer on automated validation and flagging conditions. Establishing this foundation ensures our intake staff aren't dealing with fragmented legacy data, giving us the reliable data quality required for sustainable multi-clinic operations.


---


### Won't Have Rationale


For our Won't Have priority, I selected RCHN-107 (Report cross-clinic wait times, 13 pts) and deliberately excluded it from the current planning horizon. We are not prioritizing cross-clinic wait time reporting and analytics right now because our immediate focus must be on establishing the core operational foundation—specifically locking down patient identity verification, contact updates, and standardized intake data (RCHN-101) first. 


We cannot accurately report across all six locations or analyze system-wide bottlenecks until we ensure that all incoming data across our clinic network is reliable and standardized. This item could be reconsidered in a future planning horizon once the core transactional intake fields are fully implemented, verified, and operational across all clinic locations.


---


## Backlog Reflection


### Persona Connection


Looking back, my Week 3 persona (Marie, IT Support Staff) focused heavily on reducing daily support tickets and troubleshooting calls related to system fragmentation and appointment confirmation errors. While that persona targeted IT support, we can connect our backlog story RCHN-103 (Show appointment availability) directly to those findings about scheduling friction and unconfirmed appointment saves. 


The core research showed that staff and patients constantly struggled with fragmented scheduling views and not knowing if bookings went through properly, generating a massive administrative headache. By making clear schedule visibility and availability a core backlog item, we address that exact user need—eliminating the guesswork and manual booking double-checks that caused those daily support requests in the first place.


---


### Scope Connection


Looking at my [Project Plan Foundation](https://github.com/ar1annaa/IT3310-ProjectPortfolio/blob/main/05-Project-Plan-Foundation/week05-project-plan.md), I explicitly established Phase One scope boundaries by including the intake workflow standardization while formally keeping custom executive dashboards out of scope. That Week 5 scope decision directly informed our backlog story connected to the clinic intake coordinator—specifically RCHN-103 | Show appointment availability (and the patient portal updates in RCHN-103/RCHN-105)—focusing development strictly on intake and scheduling integrity rather than analytics or reminders for now. 


The backlog item adds crucial technical and functional detail for the developers by specifying how availability must be presented: it requires real-time slot rendering, conflict prevention logic, and secure database synchronization so patients can independently select open times without creating double-booking errors across our six clinic locations. This gives developers precise boundaries knowing they need to build robust front-end calendar availability components while ignoring complex backend executive reporting features that fall outside Phase One.


---


*NovaTech Consulting | IT 3310 | Governors State University | Fall 2026*
