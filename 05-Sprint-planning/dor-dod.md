# Definition of Ready & Definition of Done

## Definition of Ready (DoR)
A user story is considered "Ready" to be pulled into a sprint when:

- [ ] The story follows the "As a... I want... so that..." format
- [ ] Acceptance criteria are written in Given/When/Then format
- [ ] Story has been estimated by the team (story points assigned)
- [ ] Story is small enough to be completed within a single sprint
- [ ] Dependencies on other stories/teams have been identified
- [ ] UI/UX mockups exist (if the story involves a user-facing screen)
- [ ] Compliance/security implications have been flagged (if the story 
      touches PHI, per HIPAA considerations doc)
- [ ] Product Owner has reviewed and approved the story

## Definition of Done (DoD)
A user story is considered "Done" when:

- [ ] Code is written and merged to the main branch
- [ ] Unit tests are written and passing (minimum 80% coverage for new code)
- [ ] Code has been peer-reviewed and approved
- [ ] QA has tested the story against all acceptance criteria
- [ ] Story has been tested on both iOS and Android (if applicable)
- [ ] Accessibility check passed (WCAG 2.1 AA, per NFR doc)
- [ ] No critical or high-severity bugs remain open
- [ ] Feature has been demoed to and accepted by the Product Owner
- [ ] Documentation updated (if the change affects user-facing behavior 
      or API contracts)
- [ ] Deployed to staging environment successfully

## Why This Matters
Without a shared DoR/DoD, teams argue about whether something is "actually done" 
or whether a story was ready to be picked up in the first place. Having this 
documented upfront — especially the compliance and accessibility checks — 
prevents HIPAA or accessibility issues from being discovered late, when 
they're expensive to fix.