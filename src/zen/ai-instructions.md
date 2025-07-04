# AI Collaboration Guidelines

These are the universal collaboration rules for AI assistants working on this project.

## Project Understanding
- Always start by reading `PROJECT.md` in the root folder to understand project-specific context, purpose, tech stack, and architecture.
- Read `package.json` to understand available scripts and testing tools.
- If testing tools (e.g., Vitest) are missing, suggest setting them up.

## Core Development Workflow
1. Understand the project fully before writing code.
2. Follow the provided design fixtures exactly (Figma, Cosmos, or similar).
3. Do not improve or alter designs without asking first. Assume the design is the source of truth.
   - If you see opportunities for improvement, propose them as suggestions before implementation.
   - If tests conflict with designs, prioritize design and adjust tests accordingly.
4. Always write testable, simple, maintainable code.
5. After implementing a feature:
   - Write unit tests immediately.
   - Ensure all project tests pass—fix other parts of the code if necessary.
   - Refactor after tests pass, not before.
   - Confirm ≥80% test coverage.
   - If testing reveals code is too complex, simplify it.
6. No strict Test-Driven Development required—but testing is non-negotiable.

## Coding Philosophy
- Prioritize simplicity and readability over advanced patterns.
- No forced functional programming—use classes where appropriate.
- Keep files under 200 lines (except tests), splitting code if necessary.
- Balance between too many micro-files and large monolithic files.
- Borrow from simplicity-oriented practices that promote easy-to-maintain code.

## Persistent AI Behaviors
- Proactively update `CHANGELOG.md` after significant changes.
- No line limits for `CHANGELOG.md`—it serves as a complete historical record.
- Document key changes, bug fixes, architectural decisions, and progress in the changelog.
- If changelog updates lag, you may be prompted to update it.

## Manifest Notes (for Web Projects)
- Assume web development as the context (HTML, CSS, JavaScript/TypeScript, React, etc.).
- Chrome Manifest V3 compliance required for any browser extension projects.

## Additional Notes
- Ensure UI code and background logic are properly separated in multi-context applications (e.g., extensions).
- When debugging synchronization issues, prioritize correct communication between contexts (e.g., background and popup).