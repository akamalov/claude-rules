# CLAUDE Agents Workflow System 
 
## 
�
�
 Overview 
 
The CLAUDE Agents System is a structured workflow for implementing 
features and fixing problems in the NAME APP frontend project. It uses 
6 specialized agents that work sequentially to ensure high-quality 
code, proper documentation, and safe version control. PLANNER needs to 
specify which phases can done simultaneoulsy! 
 
## 
�
�
 The Agents 
 
### 1. PLANNER - The Strategist - **Role**: Investigates problems and designs solutions - **Analyzes**: Root causes, not symptoms - **Creates**: Detailed phases for other agents - **Command**: `/planner "describe your problem or idea"` 
 
### 2. EXECUTER - The Builder - **Role**: Implements the solution - **Follows**: Phase 1 instructions from PLANNER - **Uses**: Established patterns from docs/ - **Output**: Clean, working code 
 
### 3. VERIFIER - The Guardian - **Role**: Ensures code quality - **Checks**: CLAUDE.md compliance - **Runs**: Validation commands - **Output**: Pass/fail report 
 
### 4. TESTER - The Validator - **Role**: Tests functionality - **Validates**: User flows and edge cases - **Tests**: Different user roles - **Output**: Test results 
 
### 5. DOCUMENTER - The Historian - **Role**: Updates documentation - **Updates**: CLAUDE.md with new patterns - **Maintains**: PROJECT_DOCUMENTATION.md - **Output**: Updated docs 
 
### 6. UPDATER - The Deployer 
- **Role**: Handles version control - **Creates**: Detailed commit messages - **Pushes**: To development branch only - **Output**: Commit confirmation 
 
## 
�
�
 How It Works 
 
### Step 1: Identify Problem 
User reports an issue or proposes a feature: 
```bash 
/planner "Users getting 'Session expired' error on dashboard" 
``` 
 
### Step 2: PLANNER Investigation 
PLANNER analyzes: - Current code implementation - Documentation in docs/ - Recent reports/ - Database schema - CLAUDE.md patterns 
 
Output: 5 phases with specific instructions for each agent 
 
### Step 3: Sequential Execution 
Each agent reads their phase and executes: 
```bash 
/executer   # Implements fix based on Phase 1 
/verifier   # Validates code quality from Phase 2 
/tester     # Tests functionality from Phase 3 
/documenter # Updates documentation from Phase 4 
/updater    # Commits changes from Phase 5 
``` 
 
### Step 4: Safe Deployment - Changes committed to `development` branch - User prompted about PR to `main` - No automatic merges to production 
 
## 
�
�
 Key Principles 
 
### 1. Root Cause Focus - Don't fix symptoms, fix the actual problem - No workarounds or quick patches 
- Follow established patterns 
 
### 2. Documentation First - Check docs/ before implementing - Update docs/ after implementing - Keep CLAUDE.md current 
 
### 3. Quality Gates - Each agent must complete successfully - Validation must pass (including violation checks) - Tests must pass - Docs must be updated - No console.log without __DEV__ - No 'any' types or catch(error: any) - No hardcoded text (must use i18n) - All error handlers must use logger 
 
### 4. Safety First - Never push directly to main - Always work on development branch - Manual approval for production 
 
## 
�
�
 Example Workflow 
 
### Problem: "Session expired errors" 
 
**PLANNER Output:** 
``` 
Root Cause: Services using auth.getUser() which fails on expired 
sessions 
Solution: Implement centralized auth checking 
 
Phase 1 - EXECUTER: - Update services to use ensureAuthenticated() - Pattern: utils/supabaseAuth.ts 
 
Phase 2 - VERIFIER: - Check TypeScript compliance - Verify import order 
 
Phase 3 - TESTER: - Test auth flows - Test expired session handling 
 
Phase 4 - DOCUMENTER: - Add pattern to CLAUDE.md - Update auth documentation 
 
Phase 5 - UPDATER: - Commit as fix(auth): implement centralized auth checking 
``` 
 
**Result**: Problem solved systematically with documentation 
 
## 
�
�
 Best Practices 
 
### For Users 
1. Describe problems clearly 
2. Include error messages 
3. Wait for each agent to complete 
4. Review changes before deployment 
 
### For Development 
1. Always start with PLANNER 
2. Never skip agents 
3. Fix failures before proceeding 
4. Document everything 
 
## 
�
�
 Common Mistakes 
 
1. **Skipping PLANNER**: Going straight to implementation 
2. **Ignoring VERIFIER**: Pushing code that doesn't pass validation 
3. **Skipping DOCUMENTER**: Not updating documentation 
4. **Direct to main**: Pushing without review 
 
## 
�
�
 Success Metrics 
 - 
✅
 All validations passing - 
✅
 No TypeScript errors - 
✅
 Tests passing - 
✅
 Documentation updated - 
✅
 Clean commit history - 
✅
 Safe deployment process 
 
## 
�
�
 Tools Used 
 
- **Supabase MCP**: Database operations - **TypeScript**: Type checking - **ESLint**: Code quality - **Git**: Version control - **npm scripts**: Automation 
 
## 
�
�
 Continuous Improvement 
 
The system learns from each problem: 
1. New patterns → CLAUDE.md 
2. New solutions → docs/ 
3. New anti-patterns → Documentation 
4. Better workflows → Agent updates 
 --- 
 
## Quick Start 
 
1. Install Claude.ai desktop app 
2. Enable Claude Code features 
3. Open project in Claude 
4. Use `/planner "your problem"` to start 
5. Follow agent sequence 
6. Deploy safely 
 
Remember: **Quality over speed. Fix it right the first time.** 
 
