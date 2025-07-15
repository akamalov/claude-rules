# Rules for version control (Git) and environment management.

## 🌳 Version Control & Environment

*   **<GIT>**
    *   Commit frequently with clear, atomic messages.
    *   Keep working directory clean; stage/commit only related files.
    *   Use `.gitignore` effectively. Always generate for new projects and add sensitive files.
    *   Follow the established branching strategy. Don't create branches unless necessary/requested.
    *   **`.env` Files:** **Never** commit `.env`. Use `.env.example`. **Never** commit `.claude`. Do not overwrite local `.env` without confirmation.
    *   Never commit the following files and directories in git repository push to GitHub (put them into .gitignore file):
    *  * `CLAUDE.md`
    *  * `GEMINI.md`
    *  * `.claude/`
    *  * `.gemini/`
    *  * `.cursor/`
    *  * `final_review_gate.py`
*   **Dependencies:** Use conda for Python and dependencies.
*   **Server Management:** Kill related running servers before starting new ones. Restart after relevant config/backend changes.

* Follow Conventional Commits v1.0.0:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

**Commit Types**:
- `feat`: New feature (MINOR version)
- `fix`: Bug fix (PATCH version)
- `refactor`: Code restructuring without behavior change
- `perf`: Performance improvement
- `docs`: Documentation only
- `test`: Test additions or corrections
- `build`: Build system or dependency changes
- `ci`: CI/CD configuration changes
- `chore`: Maintenance tasks
- `style`: Code formatting (whitespace, semicolons, etc)
