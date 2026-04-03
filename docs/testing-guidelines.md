# Testing Guidelines for TODO App

This document outlines the testing guidelines for the TODO application, covering unit, integration, and end-to-end (E2E) tests.

## 1. Unit Testing
- Use **Jest** as the testing framework for both frontend and backend unit tests.
- Test individual functions, components, and modules in isolation.
- Follow the naming convention: `*.test.ts` for all unit test files.
- Place frontend unit tests under `frontend/src/__tests__/`.
- Place backend unit tests under `backend/__tests__/`.

## 2. Integration Testing
- Use **Jest** and **Supertest** for backend integration tests.
- Integration tests should test backend endpoints with real HTTP requests.
- Place integration tests under `backend/__tests__/` and use the `*.test.ts` naming convention.
- Ensure integration tests cover interactions between multiple modules or services.

## 3. End-to-End (E2E) Testing
- Use **Playwright** for E2E tests.
- E2E tests should simulate real user interactions and test the app as a whole.
- Place all Playwright tests under a dedicated `test/e2e/` directory at the root of the project.
- Configure Playwright to use only one browser (e.g., Chromium) for testing.
- E2E tests should cover critical user flows (e.g., adding, editing, deleting tasks).

## 4. General Guidelines
- Write clear, descriptive test cases and use meaningful assertions.
- Ensure tests are deterministic and do not depend on external state.
- Run all tests as part of the CI/CD pipeline.
- Keep tests up to date as features change.

---
Following these guidelines will help ensure the TODO app is robust, reliable, and maintainable.
