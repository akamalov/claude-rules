# Claude Code Development Rules

This directory contains a comprehensive set of development rules and guidelines converted from Cursor IDE format (.mdc) to Claude Code format (.md).

## 📁 Directory Structure

```
output/
├── CLAUDE.md                                          # Main rules file (reference all others)
├── README.md                                          # This file
├── core-philosophy.md                                 # Core development principles
├── communication-rules.md                             # AI communication guidelines
├── implementation-workflow.md                         # ACT/Code mode procedures
├── planning-workflow.md                               # PLAN/Architect mode procedures  
├── code-style-quality.md                             # Code quality standards
├── testing.md                                        # Testing procedures
├── debugging-workflow.md                             # Debugging protocols
├── security.md                                       # Security guidelines
├── architecture-understanding.md                     # Architecture adherence
├── system-patterns.md                                # System design patterns
├── directory-structure.md                            # Project organization
├── documentation-memory.md                           # Documentation standards
├── version-control.md                                # Git and environment management
├── improvements-suggestions.md                       # Optimization guidelines
├── swebench-workflow.md                              # SWE-Bench specialized workflow
├── apm_impl_plan_critical_elements_reminder.md       # APM implementation checklist
├── apm_memory_system_format_source.md                # APM memory system guide
├── apm_plan_format_source.md                         # APM plan formatting
├── apm_task_prompt_plan_guidance_incorporation_reminder.md # APM task guidance
├── apm_discovery_synthesis_reminder.md               # APM discovery procedures
└── apm_memory_naming_validation_reminder.md          # APM memory validation
```

## 🚀 How to Use These Rules

### Option 1: Single CLAUDE.md File (Recommended)
Copy the `CLAUDE.md` file to your project root. This file references all other rules and provides comprehensive guidance.

### Option 2: Organized .claude Directory
Create a `.claude` directory structure in your project:

```bash
mkdir -p .claude/rules
cp *.md .claude/rules/
mv .claude/rules/CLAUDE.md .claude/
mv .claude/rules/README.md .claude/
```

### Option 3: Selective Rules
Choose only the rules relevant to your project and copy them to your project's `.claude/rules/` directory, then update CLAUDE.md to reference only the selected rules.

## 📋 Rule Categories

### 🎯 Core Rules (Always Apply)
- `core-philosophy.md` - Fundamental development principles
- `communication-rules.md` - AI interaction guidelines
- `code-style-quality.md` - Code quality standards

### 🔧 Workflow Rules (Context-Specific)
- `implementation-workflow.md` - Step-by-step implementation procedures
- `planning-workflow.md` - Project planning and architecture
- `debugging-workflow.md` - Problem-solving protocols

### 🏗️ Architecture Rules (Project-Specific)
- `architecture-understanding.md` - System design adherence
- `system-patterns.md` - Design pattern application
- `directory-structure.md` - Project organization

### 🔒 Quality Assurance Rules
- `testing.md` - Comprehensive testing procedures
- `security.md` - Security best practices
- `version-control.md` - Git and environment management

### 📝 Documentation Rules
- `documentation-memory.md` - Documentation standards
- `improvements-suggestions.md` - Optimization guidelines

### 🤖 Specialized Workflows
- `swebench-workflow.md` - SWE-Bench challenge procedures
- `apm_*.md` - Agentic Project Management framework rules

## 🎯 Usage Examples

### For a New Project
1. Copy `CLAUDE.md` to your project root
2. Copy relevant rule files to `.claude/rules/`
3. Customize `CLAUDE.md` to reference your specific needs

### For an Existing Project
1. Review current development practices
2. Choose applicable rules from the collection
3. Integrate selected rules into existing CLAUDE.md or create new one

### For Specialized Workflows
- **APM Projects**: Include all `apm_*.md` files
- **SWE-Bench**: Include `swebench-workflow.md`
- **Security-Critical**: Emphasize `security.md` rules

## 🔄 Customization Guidelines

### Adapting Rules to Your Project
1. **Technology Stack**: Modify technology-specific references
2. **Team Size**: Adjust collaboration guidelines
3. **Project Complexity**: Scale workflow procedures accordingly
4. **Industry Requirements**: Add domain-specific security or compliance rules

### Adding Project-Specific Rules
Create additional `.md` files for:
- Technology-specific patterns (e.g., `react.md`, `python.md`)
- Domain-specific logic (e.g., `finance.md`, `healthcare.md`)
- Team conventions (e.g., `code-review.md`, `deployment.md`)

## 📊 Rule Priority System

### High Priority (Always Apply)
- Core philosophy and principles
- Communication guidelines
- Code quality standards

### Medium Priority (Apply When Relevant)
- Architecture and system design
- Testing and debugging procedures
- Security guidelines

### Low Priority (Apply When Explicitly Needed)
- Specialized workflows (APM, SWE-Bench)
- Advanced optimization techniques
- Framework-specific patterns

## 🛠️ Integration Tips

### With Claude Code
1. Place `CLAUDE.md` in project root or `.claude/` directory
2. Reference specific rules in code comments when needed
3. Use rule names in prompts for targeted guidance

### With Development Workflow
1. Review applicable rules before starting new features
2. Reference rules during code reviews
3. Update rules based on project learnings

### With Team Collaboration
1. Share rule files with team members
2. Establish consensus on rule priorities
3. Document team-specific customizations

## 🔗 External References

- [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code)
- [Original Cursor IDE Rules](../) - Source .mdc files
- Project-specific documentation and requirements

## 📈 Continuous Improvement

- Regularly review and update rules based on project experience
- Collect feedback from development team
- Adapt rules to evolving best practices and technologies
- Maintain version history of rule changes

---

*These rules provide a comprehensive foundation for consistent, high-quality development with Claude Code across diverse project types and requirements.*