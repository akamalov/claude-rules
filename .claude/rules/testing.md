# Rules and procedures for testing code.

## ✅ Testing

**<TESTING>** (Always write tests after implementation)

*   **TDD Focus:**
    *   *New Features:* Outline tests -> write failing tests -> implement code -> refactor.
    *   *Bug Fixes:* Write a test reproducing the bug *before* fixing it.
*   **<DEPENDENCY BASED TESTING>** Create unit tests for new functionality. Run tests affected by the changes (**<ANALYZE CODE>** from `implementation-workflow.md`) to confirm existing behavior.
*   **<NO BREAKAGE ASSERTION>** Run tests *yourself* after proposing a change and verify they pass. Be certain code won't be broken.
*   **Test Location:** Write test logic in separate files from implementation code.
*   **<TEST PLAN>**
    *   Define comprehensive, exhaustive test scenarios covering edge cases based on requirements.
    *   Specify validation methods.
    *   Suggest monitoring approaches.
    *   Consider and prevent regressions.
*   **Comprehensive Tests:** Write thorough unit, integration, and/or E2E tests.
*   **Tests Must Pass:** All tests MUST pass before committing or completing a task. Notify human immediately if tests fail and can't be easily fixed.
*   **No Mock Data (Except Tests):** Use mocks *only* in test environments. Dev/Prod use real/realistic data. Never add stubbing/fake data patterns to dev/prod code.
*   **Manual Verification:** Supplement automated tests with manual checks (especially UI).
*   **Test First (Workflow Preference):** Write tests first, then code, run tests, update code until tests pass. (Applies particularly to new features).
*   **Document Testing:** Document in memory files as specified by `documentation-memory.md`.
