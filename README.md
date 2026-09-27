# Accessibility & Architecture Audit

A full-stack project foundation created from an accessibility and architecture audit of a public-facing service website.

## Project Goals
- Audit a real public-facing website with Lighthouse.
- Perform a keyboard-only navigation review.
- Document five accessibility/architecture issues with evidence and remediation priority.
- Establish a maintainable monorepo-style full-stack structure.
- Prepare the first end-to-end vertical feature slice.

## Repository Structure

```text
accessibility-architecture-audit/
├── client/          # Frontend UI, pages, components and API client
├── server/          # Backend API, controllers, services and middleware
├── docs/            # Audit, keyboard test and architecture documentation
└── tests/           # Cross-application and accessibility tests
```

## Architecture Boundaries

```text
Browser
   │
   ▼
┌──────────────────┐
│      Client      │
│ UI / Pages / API │
└────────┬─────────┘
         │ HTTP / JSON
         ▼
┌──────────────────┐
│      Server      │
│ Routes / Service │
└────────┬─────────┘
         │
         ▼
     Data Layer
```

### Client
Responsible for UI, routing, semantic HTML, keyboard accessibility and API communication.

### Server
Responsible for HTTP routes, validation, business logic and data access boundaries.

### Docs
Contains the audit report, keyboard test, architecture notes and screenshot evidence.

### Tests
Contains accessibility, integration and future end-to-end tests.

## Local Setup

```bash
npm install
npm run dev
npm test
```

The current repository is intentionally a setup-ready skeleton. Add the chosen frontend/backend framework in the first implementation slice.

## First Vertical Feature Slice

The first feature should cross every application boundary:

```text
Accessible UI
   ↓
API Request
   ↓
Server Route
   ↓
Controller
   ↓
Service
   ↓
Data Layer
   ↓
API Response
   ↓
Accessible UI State
```

## Audit Evidence

- `docs/audit-report.md`
- `docs/keyboard-test.md`
- `docs/architecture.md`
- `docs/audit-template.csv`
- `docs/screenshots/`

> Replace placeholder audit evidence with screenshots and measurements from the actual audited website before submission.

## Official References

- https://developer.chrome.com/docs/devtools/lighthouse/
- https://www.w3.org/WAI/fundamentals/accessibility-principles/
- https://www.w3.org/WAI/WCAG21/Understanding/keyboard-accessible
- https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes
- https://docs.npmjs.com/cli/v8/using-npm/workspaces/
