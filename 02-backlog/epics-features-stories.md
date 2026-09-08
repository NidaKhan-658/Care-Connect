# CareConnect Backlog: Epics, Features & User Stories

---

## EPIC 1: Appointment Management

### Feature 1.1: Appointment Scheduling
**US-101** | As a patient, I want to book an appointment online, so that I don't have to call the clinic.

<!-- Given I am logged into CareConnect
When I select a provider and an available time slot
Then the appointment is booked and I receive a confirmation -->
Story Points: 5

**US-102** | As a patient, I want to reschedule an appointment, so that I can adjust for conflicts.

<!-- Given I have an upcoming appointment
When I select "Reschedule" and choose a new time slot
Then the old slot is released and the new one is confirmed -->
Story Points: 3

**US-103** | As a patient, I want to cancel an appointment, so that the slot becomes available to others.

<!-- Given I have an upcoming appointment
When I select "Cancel" and confirm
Then the appointment is removed and the provider is notified -->
Story Points: 2

### Feature 1.2: Appointment Reminders
**US-104** | As a patient, I want to receive an SMS reminder 24 hours before my appointment, so that I don't forget.

<!-- Given I have an appointment scheduled
When it is 24 hours before the appointment time
Then I receive an SMS with date, time, and provider name -->

Story Points: 5

**US-105** | As a patient, I want to confirm or cancel via the reminder text, so that I don't need to open the app.

<!-- Given I received a reminder SMS
When I reply "CONFIRM" or "CANCEL"
Then my appointment status updates accordingly -->

Story Points: 3

### Feature 1.3: Provider Calendar View
**US-106** | As a care coordinator, I want to see all upcoming appointments in a calendar view, so that I can manage provider schedules.

<!-- Given I am logged in as a care coordinator
When I open the calendar view
Then I see all appointments for the week, filterable by provider -->

Story Points: 5

---

## EPIC 2: Medication Adherence Tracking

### Feature 2.1: Medication Schedule Setup
**US-201** | As a provider, I want to input a patient's medication schedule, so that reminders can be automated.

<!-- Given I am viewing a patient's profile
When I add a medication with dosage, frequency, and duration
Then the schedule is saved and reminders are auto-generated -->
Story Points: 5

### Feature 2.2: Medication Reminders & Logging
**US-202** | As a patient, I want to receive a reminder when it's time to take my medication, so that I don't miss a dose.

<!-- Given I have an active medication schedule
When the scheduled time arrives
Then I receive an SMS reminder with medication name and dosage -->
Story Points: 5

**US-203** | As a patient, I want to log that I took my medication by replying to the reminder, so that my adherence is tracked.

<!-- Given I received a medication reminder
When I reply "TAKEN"
Then my adherence log is updated with a timestamp -->
Story Points: 3

### Feature 2.3: Adherence Dashboard
**US-204** | As a care coordinator, I want to see which patients have missed doses, so that I can follow up proactively.

<!-- Given patients have active medication schedules
When I open the adherence dashboard
Then I see a list of patients with missed-dose flags, sorted by severity -->

Story Points: 8

---

## EPIC 3: Secure Provider Messaging

### Feature 3.1: Direct Messaging
**US-301** | As a patient, I want to send a secure message to my provider, so that I can ask non-urgent questions.

<!-- Given I am logged into CareConnect
When I select a provider and send a message
Then the message is delivered securely and encrypted -->

Story Points: 5

**US-302** | As a provider, I want to receive and reply to patient messages, so that I can address their concerns.

<!-- Given a patient has sent me a message
When I open my inbox
Then I see the message and can reply within the same thread -->

Story Points: 5

### Feature 3.2: Message Notifications
**US-303** | As a patient, I want to be notified when I receive a reply, so that I know to check the app.

<!-- Given a provider has replied to my message
When the reply is sent
Then I receive a push notification (not containing message content, per HIPAA) -->

Story Points: 3

---

## Backlog Summary
| Epic | Features | Stories | Total Points |
|---|---|---|---|
| Appointment Management | 3 | 6 | 23 |
| Medication Adherence Tracking | 3 | 4 | 21 |
| Secure Provider Messaging | 2 | 3 | 13 |
| **Total** | **8** | **13** | **57** |