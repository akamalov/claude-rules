# Communication & Documentation Rules

## 🗣️ Communication Standards

### Core Communication Principles
- **Clarity First**: Be clear, specific, and provide context
- **Split Responses**: Use multiple responses if one isn't sufficient
- **Clear Intent**: Distinguish between "Suggestion:" vs "Applying fix:"
- **Confirmation Protocol**: Use check-ins for large tasks to confirm understanding

### Interaction Guidelines
- **AI Check-in**: Before major suggestions, confirm understanding:
  "Confirming understanding: I've reviewed [source]. The goal is [goal], adhering to [constraint]. Proceeding with [step]."
- **Reference Context**: Reference previous interactions when relevant
- **Incremental Steps**: Use incremental approach for complex tasks
- **Critical Review**: Encourage human oversight for complex logic, architecture, security

### Communication Workflow
- **Context Reference**: Always reference relevant documentation and patterns
- **Assumption Clarification**: State all assumptions, choices, decisions, trade-offs
- **Multi-Attempt Reasoning**: Question assumptions, think of better solutions
- **Web Research**: Use web search when needed for research

## 🧠 Documentation & Memory Management

### Memory Files Structure
A systematic approach to maintaining project context through structured documentation.

#### Core Files (Required)
1. **`docs/product_requirement_docs.md`**: PRD/SOP (Why, goals, scope)
2. **`docs/architecture.md`**: System architecture (How, components, dependencies)
3. **`docs/technical.md`**: Dev environment, stack, tech decisions, patterns
4. **`tasks/tasks_plan.md`**: Detailed task backlog, progress, status, issues
5. **`tasks/active_context.md`**: Current work focus, decisions, recent changes
6. **`.claude/rules/error-documentation.md`**: Reusable fixes, known issues log
7. **`.claude/rules/lessons-learned.md`**: Learning journal (patterns, preferences)

#### Context Files (Optional)
- **`docs/literature/`**: Research files (.tex files)
- **`tasks/rfc/`**: RFCs for tasks (.tex files)
- Additional `docs/` or `tasks/` files for specific organizational needs

### Documentation Update Protocol

#### When to Update
- **<DOC>**: Update when changes impact architecture, technical decisions, patterns
- When discovering new patterns or implementing significant changes
- User requests with "**update memory files**" (MUST review ALL Core Files)
- When context needs clarification or after Plan verification

#### Update Process
1. Review Core Files
2. Update `active_context.md` & `tasks_plan.md`
3. Clarify next steps in `tasks_plan.md`
4. Update `lessons-learned.md` & `error-documentation.md`
5. Keep `.claude/rules/*` files reviewed and updated

### Project Intelligence Management

#### Lessons Learned (`lessons-learned.md`)
- **Capture**: Critical paths, user preferences, project patterns, challenges
- **Format**: Flexible format focused on valuable insights
- **Process**: Identify Pattern → Validate with User → Document
- **Usage**: Read lessons → Apply learned patterns → Improve future work
- **Integration**: Create phase documentation in docs/documentation/software-documentation.md

#### Error Documentation (`error-documentation.md`)
- **Purpose**: Log reusable fixes to avoid repeating mistakes
- **Content**: Known issues, context, and resolution
- **Usage**: Reference before implementing similar solutions

### Documentation Standards
- **Version Control**: Always maintain documentation in version control
- **Consistency**: Follow established documentation patterns
- **Completeness**: Ensure all critical decisions are documented
- **Accessibility**: Write documentation for future developers
- **Updates**: Keep documentation current with code changes

### Special Documentation Requirements
- **Database Schema**: Document complete schema in docs/planning/[project-name]-planning.md
- **Technology Stack**: Record stack, modules, and versions in [project-name]-technology-stack.md
- **Progress Tracking**: Maintain implementation status in separate tracking files
- **Milestone Updates**: Update milestone documentation after major features