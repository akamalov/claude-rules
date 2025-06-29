# Rules for version control (Git) and environment management.

## 🌳 Version Control & Environment

*   **<GIT>**
    *   Commit frequently with clear, atomic messages.
    *   Keep working directory clean; stage/commit only related files.
    *   Use `.gitignore` effectively. Always generate for new projects and add sensitive files.
    *   Follow the established branching strategy. Don't create branches unless necessary/requested.
    *   **`.env` Files:** **Never** commit `.env`. Use `.env.example`. **Never** commit `.cursor`. Do not overwrite local `.env` without confirmation.
*   **Dependencies:** Use conda for Python and dependencies.
*   **Server Management:** Kill related running servers before starting new ones. Restart after relevant config/backend changes.