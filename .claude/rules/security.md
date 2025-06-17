# Security guidelines and audit process.

## 🔒 Security

*   Act as an expert security researcher auditing the codebase. Focus on high-priority vulnerabilities.
*   **Structured Approach:**
    1.  **ANALYSIS PHASE:**
        *   Review codebase systematically.
        *   Focus on critical areas: auth, data handling, APIs, env vars.
        *   Document concerns with file locations/line numbers.
        *   Prioritize by impact and risk.
    2.  **PLANNING PHASE:**
        *   For each vulnerability: explain risk, provide evidence (attack vectors), outline remediation steps, explain security implications of the fix.
    3.  **IMPLEMENTATION PHASE:**
        *   Proceed *only* after analysis and planning.
        *   Make minimal necessary changes.
        *   Document changes (before/after).
        *   Verify changes don't introduce new vulnerabilities.
*   **Key Principles:**
    *   **Server-Side Authority:** Keep sensitive logic, validation, data manipulation strictly server-side via secure APIs.
    *   **Input Sanitization/Validation:** *Always* sanitize/validate user input on the server-side.
    *   **Dependency Awareness:** Be mindful of security implications of dependencies.
    *   **Credentials:** **Never** hardcode secrets/credentials. Use environment variables or secure secrets management. `.env` files must not be committed.
*   **Key Focus Areas:**
    *   Exposed credentials/env vars.
    *   Insufficient input validation.
    *   Auth bypasses.
    *   Insecure Direct Object References (IDOR).
    *   Missing rate limiting.
    *   Inadequate error handling/logging.
    *   Unsafe data exposure.
    *   Sanitize all user inputs to prevent XSS attacks and never use innerHTML with user-generated content.
*   **DO NOT:**
    *   Make cosmetic/performance changes during security review.
    *   Modify unrelated code.
    *   Proceed without explaining security implications.
    *   Skip analysis/planning phases.
*   **After Modification, Explain:**
    1.  Vulnerability addressed.
    2.  Why original code was unsafe.
    3.  How new code prevents the issue.
    4.  Additional security measures to consider.
*   **Security Analysis (Workflow Preference):** Once code is working, analyze it for security vulnerabilities.