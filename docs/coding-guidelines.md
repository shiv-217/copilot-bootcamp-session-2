# Coding Guidelines for TODO App

## 1. General Principles
- Use clear, descriptive names for variables, functions, and components.
- Write modular, reusable code—prefer small, focused functions and components.
- Keep code DRY (Don’t Repeat Yourself) and avoid duplication.
- Use comments to explain complex logic, but prefer self-explanatory code.

## 2. Frontend (React + Material UI)
- Use functional components and React hooks.
- Organize components by feature or domain.
- Use Material UI components for all UI elements to ensure consistency.
- Style components using Material UI’s theming and styling solutions.
- Ensure all UI is accessible (keyboard navigation, ARIA labels, color contrast).
- Handle user feedback with Material UI Snackbar/Alert components.
- Keep state management simple; use React context or local state unless complexity requires more.

## 3. Backend (Node.js + Express)
- Organize code by feature (routes, controllers, services).
- Validate all incoming data (e.g., using middleware).
- Handle errors gracefully and return meaningful HTTP status codes.
- Keep business logic out of route handlers—use separate service modules.
- Use async/await for asynchronous code and handle promise rejections.

## 4. Testing
- Write unit tests for all functions, components, and modules using Jest.
- Use Supertest for backend integration tests.
- Use Playwright for end-to-end (E2E) tests simulating real user flows.
- Place tests in the appropriate directories and follow naming conventions (`*.test.js`, `*.spec.js`).
- Ensure tests are deterministic and run as part of CI/CD.

## 5. Code Style & Quality
- Use a linter (e.g., ESLint) and formatter (e.g., Prettier) to enforce consistent style.
- Prefer const and let over var.
- Use modern JavaScript/ES6+ features.
- Avoid magic numbers and hardcoded values—use constants.
- Review and refactor code regularly for readability and maintainability.

## 6. Documentation
- Document all public functions, components, and modules.
- Update documentation as features and APIs change.
