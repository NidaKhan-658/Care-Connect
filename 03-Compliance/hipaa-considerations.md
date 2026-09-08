# HIPAA Considerations for CareConnect

## Protected Health Information (PHI) in Scope
- Patient names, appointment details, medication names/dosages, 
  and message content between patients and providers all qualify as PHI 
  and must be handled accordingly.

## Consent Management
- Patients must explicitly opt in to SMS reminders during onboarding, 
  since standard SMS is not inherently HIPAA-compliant
- Consent must be re-confirmed if the patient's phone number changes
- Patients can revoke consent at any time via account settings

## Data Encryption
- All PHI must be encrypted at rest (AES-256) and in transit (TLS 1.2+)
- Messaging feature must NOT include PHI content in push notification 
  previews (e.g., notification should say "You have a new message" 
  rather than showing the message content) — this is reflected in US-303

## Access Controls
- Role-based access: patients can only view their own records; 
  care coordinators can view records for their assigned patient panel only
- Providers must use multi-factor authentication to access patient messaging

## Audit Logging
- All access to PHI (views, edits, message sends) must be logged with 
  timestamp, user ID, and action taken
- Audit logs must be retained for a minimum of 6 years per HIPAA requirements

## Business Associate Agreements (BAAs)
- Any third-party vendor handling PHI (e.g., SMS gateway provider, 
  cloud hosting provider) must have a signed BAA in place before integration

## Breach Notification
- In the event of a suspected breach, the compliance team must be notified 
  within 24 hours per internal policy, ahead of the 60-day HHS notification 
  deadline required by law