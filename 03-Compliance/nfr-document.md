# Non-Functional Requirements (NFRs)

## Performance
- App screens must load within 2 seconds on 4G connection
- SMS reminders must be sent within 1 minute of the scheduled trigger time
- System must support 10,000 concurrent users without degraded performance

## Accessibility
- All screens must meet WCAG 2.1 AA compliance
- Font sizes must be adjustable up to 200% without breaking layout
  (important given Persona 1: Margaret, low tech literacy, may need larger text)
- Color contrast ratio must meet minimum 4.5:1 for all text elements
- App must be fully navigable via screen reader (VoiceOver/TalkBack)

## Security
- All data in transit must use TLS 1.2 or higher
- All data at rest must be encrypted using AES-256
- Session timeout after 15 minutes of inactivity
- Multi-factor authentication required for provider accounts

## Reliability & Availability
- System uptime target: 99.9% (excluding scheduled maintenance windows)
- Automated backups every 24 hours, retained for 30 days
- Failover plan in place for SMS gateway provider outage

## Scalability
- Architecture must support horizontal scaling to accommodate 
  hospital-wide rollout beyond initial pilot group

## Compatibility
- Must function on iOS 15+ and Android 11+
- Must be responsive on mobile web for patients without the app installed