# Structure and maintenance of project documentation and memory files.

## 🧠 Documentation & Memory Management

*   **Memory Files Structure:** A system of core and optional files in `docs/` and `tasks/` to maintain project context.
    *   **Core Files (Required):**
        1.  `docs/product_requirement_docs.md`: PRD/SOP (Why, goals, scope).
        2.  `docs/architecture.md`: System architecture (How, components, dependencies).
        3.  `docs/technical.md`: Dev env, stack, tech decisions, patterns.
        4.  `tasks/tasks_plan.md`: Detailed task backlog, progress, status, issues.
        5.  `tasks/active_context.md`: Current work focus, decisions, recent changes, next steps.
        6.  `.cursor/rules/error-documentation.mdc`: Reusable fixes/corrections, known issues log.
        7.  `.cursor/rules/lessons-learned.mdc`: Learning journal (patterns, preferences, intelligence).
    *   **Context Files (Optional):**
        *   `docs/literature/`: Research (.tex files).
        *   `tasks/rfc/`: RFCs for tasks (.tex files).
        *   Other `docs/` or `tasks/` files for organization (integrations, testing strategies, etc.).
*   **Documentation Updates:**
    *   **<DOC>** Update relevant docs (`README.md`, `docs/architecture.md`, `docs/technical.md`, `tasks/tasks_plan.md`, `docs/status.md`) if changes impact architecture, technical decisions, patterns, or task status.
    *   Update Memory Files when:
        *   Discovering new patterns.
        *   After implementing significant changes.
        *   User requests with "**update memory files**" (MUST review ALL Core Files).
        *   Context needs clarification.
        *   After significant part of Plan is verified.
    *   **Update Process:** Review Core Files -> Update `active_context.md` & `tasks_plan.md` -> Clarify next steps in `tasks_plan.md` -> Update `lessons-learned.mdc` & `error-documentation.mdc`.
    *   **Rule Updates:** Keep `.cursor/rules/*` files reviewed and updated.
*   **Project Intelligence (`lessons-learned.mdc`):**
    *   Capture critical paths, user preferences, project patterns, challenges, decision evolution, tool usage.
    *   Format is flexible; focus on valuable insights.
    *   **Learning Process:** Identify Pattern -> Validate with User -> Document in `lessons-learned.mdc`.
    *   **Usage:** Read `lessons-learned.mdc` -> Apply Learned Patterns -> Improve Future Work.
*   **Error Documentation (`error-documentation.mdc`):**
    *   If you find a reusable fix or correction, note it here to avoid repeating mistakes. Log known issues, context, and resolution.