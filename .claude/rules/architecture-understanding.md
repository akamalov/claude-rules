# Rules for understanding and adhering to project architecture defined in docs/architecture.md.

## 🏗️ Architecture Understanding

*   Based on `docs/architecture.md`:
    *   Load and parse the complete Mermaid diagram.
    *   Extract and understand module boundaries, relationships, data flow, interfaces, and dependencies.
    *   Validate any proposed changes against these architectural constraints.
    *   Ensure new code maintains the defined separation of concerns.
*   **Error Handling:**
    *   If `docs/architecture.md` not found: STOP and notify.
    *   If diagram parse fails: REQUEST clarification.
    *   If architectural violation detected: WARN user and propose compliant alternatives.