# Accessibility & Architecture Audit Report

## Audited Website

**Website:** Replace with the selected public service website  
**URL:** Replace with the audited URL  
**Audit date:** Replace with date  
**Browser:** Chrome  
**Methods:** Lighthouse + keyboard-only manual review

## Methodology

1. Run Lighthouse Accessibility audit in Chrome DevTools.
2. Record the Lighthouse score and failed audits.
3. Navigate the core journey using only the keyboard.
4. Capture screenshots for each finding.
5. Map findings to WCAG where applicable.
6. Prioritize issues by user impact and task blocking potential.

## Five Findings

The repository template contains five audit rows in `audit-template.csv`. Replace the placeholder/example evidence with observations from the selected website.

| ID | Area | Priority |
|---|---|---|
| A11Y-001 | Keyboard/focus | P1 |
| A11Y-002 | Form labeling | P1 |
| A11Y-003 | Color/contrast | P1 |
| A11Y-004 | Heading/landmark structure | P2 |
| A11Y-005 | Accessible names / controls | P2 |

## Evidence Standard

Every issue should contain:
- exact page/component;
- observed behavior;
- screenshot;
- WCAG reference when applicable;
- user impact;
- remediation;
- priority.

Do not claim an issue is present unless it was observed during the audit.
