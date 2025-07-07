# Guidelines for code style, quality, and maintainability.

## ✨ Code Style & Quality

*   **Clean Code:** Keep the codebase clean and organized.
*   **Readability/Maintainability:**
    *   Refactor working code to improve readability and maintainability.
    *   Use descriptive and meaningful names for variables, functions, classes, files.
    *   Add comments to explain non-obvious code. (Balance with writing self-documenting code where possible).
*   **File Size:** Avoid files over 200-300 lines. Refactor.
*   **No Scripts in Files:** Avoid writing one-off scripts directly in project files if possible.
*   **Logging:** Add logs during implementation/debugging. Remove them once the code is working and stable.
*   **Consistency:** Maintain a consistent coding style throughout the project (see `core-philosophy.md`).
*   **Avoid Duplication:** Check for existing similar code/functionality before writing new code. Refactor to reduce duplication (see `core-philosophy.md`).
*   **Refactoring:** (Also see `implementation-workflow.md` -> `<REFACTORING>` section if exists, otherwise keep here)
    *   Purposeful Refactoring: Refactor to improve clarity, reduce duplication, simplify complexity, or adhere to architectural goals.
    *   Holistic Check: When refactoring, look for duplicate code, similar components/files, and opportunities for consolidation across the affected area.
    *   Edit, Don't Copy: Modify existing files directly. Do not duplicate files and rename them (e.g., `component-v2.tsx`).
    *   Verify Integrations: After refactoring, ensure all callers, dependencies, and integration points function correctly. Run relevant tests. 
    *   Stay within defined project, and not execute programs outside. When executing commands use full path, never relative. Do not assume you're in the project directory. Use full path.
