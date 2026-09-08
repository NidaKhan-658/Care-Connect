# MoSCoW Prioritization: CareConnect Backlog

## Must Have
These are essential for the MVP launch — without them, the feature doesn't solve the core problem.

| Story ID | Story | Reasoning |
|---|---|---|
| US-101 | Book an appointment online | Core scheduling function; without it, nothing else matters |
| US-104 | SMS appointment reminder | Directly targets the no-show problem stated in the charter |
| US-202 | Medication reminder | Directly targets the adherence problem stated in the charter |
| US-203 | Log medication as taken | Without logging, adherence can't be measured at all |
| US-301 | Send secure message to provider | Core communication channel; required for HIPAA-compliant messaging |

## Should Have
Important, but the product still functions without them at launch.

| Story ID | Story | Reasoning |
|---|---|---|
| US-102 | Reschedule appointment | High user value, but patients can cancel + rebook as a workaround initially |
| US-105 | Confirm/cancel via reminder reply | Improves UX significantly but isn't blocking — patients can still use the app |
| US-201 | Provider inputs medication schedule | Needed to enable reminders, but could launch with manual/CSV upload initially |
| US-302 | Provider replies to messages | Needed for two-way communication, but one-way alerts could ship first |

## Could Have
Nice to have, adds polish, but easily deferred to a later release.

| Story ID | Story | Reasoning |
|---|---|---|
| US-103 | Cancel appointment | Lower priority than booking; can be handled manually by staff short-term |
| US-303 | Push notification for message reply | Convenience feature; SMS/email fallback works in the meantime |

## Won't Have (this release)
Explicitly out of scope for this phase.

| Story ID | Story | Reasoning |
|---|---|---|
| US-106 | Provider calendar view | Valuable for coordinators, but not patient-facing; deferred to Phase 2 |
| US-204 | Adherence dashboard | Requires enough logged data (US-203) to be meaningful; sequenced after MVP |

## Prioritization Logic
Priority was assigned based on three factors:
1. **Direct link to charter KPIs** (no-show rate, adherence rate) — highest priority
2. **Dependency chains** — e.g., US-204 depends on US-203 data existing first
3. **HIPAA/compliance necessity** — anything required for secure messaging to be 
   legally viable was pulled into Must Have