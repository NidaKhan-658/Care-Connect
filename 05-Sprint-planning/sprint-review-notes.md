# Sprint Review & Retrospective Notes

---

## Sprint 1 (Weeks 1-2)

### Committed Stories
| Story ID | Story | Points |
|---|---|---|
| US-101 | Book an appointment online | 5 |
| US-104 | Receive SMS reminder 24 hours before appointment | 5 |
| US-202 | Receive medication reminder | 5 |
| US-203 | Log medication as taken via reply | 3 |
| **Total** | | **18** |

### Sprint Review (Demo Summary)
- Demoed end-to-end appointment booking flow to stakeholders, including 
  confirmation screen
- Demoed SMS reminder trigger 24 hours before a test appointment
- Demoed medication reminder + "TAKEN" reply logging, shown live on the 
  compliance liaison's test phone
- Stakeholder feedback: compliance rep flagged that reminder SMS copy needed 
  to avoid stating specific medication names in the message preview on 
  lock screens — added as a fast-follow item for Sprint 2

### Retrospective
**What went well:**
- Team hit 18 of 20 estimated points — close to target for a first sprint
- SMS gateway vendor integration was smoother than expected after the 
  Sprint 0 spike

**What to improve:**
- Compliance review happened too late in the sprint (during the demo, 
  not before development started) — action: add a compliance checkpoint 
  to Definition of Ready going forward
- QA was bottlenecked in the last 2 days of the sprint — action: start 
  QA testing on completed stories mid-sprint instead of waiting until 
  the end

**Velocity for Sprint 2 planning:** 18 points (adjusted down slightly 
from the initial 20-point assumption)

---

## Sprint 2 (Weeks 3-4)

### Committed Stories
| Story ID | Story | Points |
|---|---|---|
| US-301 | Send secure message to provider | 5 |
| US-102 | Reschedule an appointment | 3 |
| US-105 | Confirm or cancel via reminder text reply | 3 |
| US-201 | Provider inputs medication schedule | 5 |
| **Total** | | **16** |

### Sprint Review (Demo Summary)
- Demoed secure messaging feature between a test patient and provider account, 
  including encryption confirmation from the engineering lead
- Demoed appointment rescheduling flow
- Demoed SMS reply-to-confirm/cancel functionality
- Demoed provider-side medication schedule input screen
- Stakeholder feedback: Product Owner requested the adherence dashboard 
  (US-204) be prioritized for Sprint 3, now that medication logging data 
  (US-203) exists to populate it

### Retrospective
**What went well:**
- Compliance checkpoint added to DoR (from Sprint 1 retro) caught a PHI 
  exposure risk in the messaging notification early, before it reached QA
- Team velocity stabilized at 16 points, giving a more reliable baseline 
  for Sprint 3 planning

**What to improve:**
- Two stories (US-201, US-105) had unclear acceptance criteria at sprint 
  start, causing rework — action: enforce the DoR checklist more strictly 
  during backlog refinement

**Velocity for Sprint 3 planning:** 16-18 points (stabilizing baseline)