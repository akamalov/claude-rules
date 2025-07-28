# Testing & Security Rules

## ✅ Comprehensive Testing Framework

### Testing Methodology
- **TDD Focus**: Outline tests → write failing tests → implement code → refactor
- **Bug Fix Protocol**: Write test reproducing bug BEFORE fixing it
- **Test-First Workflow**: Write tests first, then code, run tests, update until passing

### Testing Requirements
- **<DEPENDENCY BASED TESTING>**: Create unit tests for new functionality
- **<NO BREAKAGE ASSERTION>**: Run tests yourself, verify they pass
- **Test Location**: Separate test files from implementation code
- **Comprehensive Coverage**: Unit, integration, and E2E tests
- **Tests Must Pass**: ALL tests MUST pass before committing
- **Manual Verification**: Supplement automated tests with manual checks (especially UI)

### Test Planning
- **<TEST PLAN>**: Define comprehensive test scenarios covering edge cases
- Specify validation methods and monitoring approaches
- Consider and prevent regressions
- Document testing approach in memory files

### Test Data Policy
- **No Mock Data (Except Tests)**: Use mocks ONLY in test environments
- Dev/Prod use real/realistic data
- Never add stubbing/fake data patterns to dev/prod code

## 🔒 Security Framework

### Security Audit Process
- Act as expert security researcher auditing codebase
- Focus on high-priority vulnerabilities
- **Structured 3-Phase Approach**:

#### Phase 1: Analysis
- Review codebase systematically
- Focus on critical areas: auth, data handling, APIs, env vars
- Document concerns with file locations/line numbers
- Prioritize by impact and risk

#### Phase 2: Planning
- For each vulnerability: explain risk, provide evidence
- Document attack vectors and remediation steps
- Explain security implications of fixes

#### Phase 3: Implementation
- Proceed ONLY after analysis and planning
- Make minimal necessary changes
- Document changes (before/after)
- Verify changes don't introduce new vulnerabilities
- Do not create test files under project root directory. Use "tests/" directory to create and test scripts and files

### Security Principles
- **Server-Side Authority**: Keep sensitive logic strictly server-side
- **Input Sanitization**: ALWAYS sanitize/validate user input server-side
- **Dependency Awareness**: Monitor security implications of dependencies
- **Credentials**: NEVER hardcode secrets - use environment variables
- **XSS Prevention**: Sanitize all user inputs, never use innerHTML with user content

### Key Security Focus Areas
- Exposed credentials/environment variables
- Insufficient input validation
- Authentication bypasses
- Insecure Direct Object References (IDOR)
- Missing rate limiting
- Inadequate error handling/logging
- Unsafe data exposure

### Security Review Guidelines
- **DO NOT**: Make cosmetic/performance changes during security review
- **DO NOT**: Modify unrelated code or skip analysis phases
- **MUST EXPLAIN**: After modification, explain:
  1. Vulnerability addressed
  2. Why original code was unsafe
  3. How new code prevents the issue
  4. Additional security measures to consider

### Security Workflow Integration
- Perform security analysis once code is working
- Integrate security considerations into all development phases
- Document security decisions and rationale
