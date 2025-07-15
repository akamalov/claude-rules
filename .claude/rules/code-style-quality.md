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

### Clear Code Principles

Write code as if the person maintaining it is a violent psychopath who knows where you live:

- **NO CLEVER TRICKS**: Clear, obvious code only
- **DESCRIPTIVE NAMING**: `processTextNodes()` not `ptn()` or `handleStuff()`
- **COMMENT THE WHY**: Only explain why, never what. Code shows what
- **SINGLE RESPONSIBILITY**: Each function does ONE thing
- **EXPLICIT ERROR HANDLING**: No silent failures
- **MEASURE THEN OPTIMIZE**: No premature optimization
- **SIMPLICITY FIRST**: Remove everything non-essential

### Honest Technical Assessment

ALWAYS provide honest assessment of technical decisions:

- If code has problems, explain the specific issues
- If an approach has limitations, quantify them
- If there are security risks, detail them clearly
- If performance will degrade, provide metrics
- If implementation is complex, justify why
- If you chose a suboptimal solution, explain the tradeoffs
- If you're uncertain, say so explicitly

Examples of honest assessment:
- "This will work for 1000 users but will break at 10,000 due to database bottleneck"
- "This fix addresses the symptom but not the root cause - we'll see this bug again"
- "This implementation is 3x more complex than needed because of legacy constraints"
- "I'm not certain this handles all edge cases - particularly around concurrent access"
- "This violates best practices but is necessary due to framework limitations"

### Context and Documentation

Preserve technical context. Never delete important information.

Keep these details:
- Code examples with line numbers
- Performance measurements and metrics
- Rationale for architectural decisions
- Explanations of non-obvious patterns
- Cross-references to related issues
- Technology-specific best practices

