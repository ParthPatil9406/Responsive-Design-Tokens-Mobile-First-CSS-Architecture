# Architecture

## Responsibility Boundaries

| Layer | Responsibility |
|---|---|
| Client | Presentation, navigation, accessibility and API calls |
| Server | HTTP API, validation and business rules |
| Service | Reusable application/business operations |
| Data layer | Persistence abstraction |
| Tests | Accessibility, integration and end-to-end verification |
| Docs | Audit evidence and architecture decisions |

## First Feature

Recommended first slice: an accessible service-status or information request.

It should demonstrate:

1. Semantic and keyboard-accessible UI.
2. Client-side validation.
3. API request.
4. Server route and controller.
5. Service-layer processing.
6. Structured JSON response.
7. Accessible success/error feedback.

## Maintainability Rules

- Keep UI components independent from database logic.
- Keep business rules out of route definitions.
- Validate external input at the server boundary.
- Use semantic HTML before ARIA.
- Keep accessibility tests close to the feature.
