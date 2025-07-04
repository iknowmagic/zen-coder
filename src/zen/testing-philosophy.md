# Testing Philosophy

## Testing Beliefs
- Testing is an integral part of the development process.
- Every feature must have corresponding unit tests.
- Focus on user-facing behaviors and core functionality.

## Coverage Goals
- Minimum 80% coverage for statements, functions, and lines.
- Higher coverage encouraged for critical modules.
- Branch coverage goals are flexible based on complexity.

## Recommended Tools
- Vitest for unit testing.
- Testing Library for UI components (e.g., @testing-library/react).
- jsdom for DOM simulation.
- Mocking utilities for APIs, storage, and network calls.

## Best Practices
1. Mock APIs and external services where necessary.
2. Keep tests isolated and deterministic—avoid shared state leakage.
3. Prefer testing behaviors and outcomes over internal implementation details.
4. Strive for clear, minimal test cases that are easy to understand.
5. Include edge case tests and error conditions.
6. Ensure tests run automatically on CI before merging any code.

## Test-Driven Development (Optional)
- Full TDD is not required.
- Focus on testability-first development rather than rigid TDD cycles.