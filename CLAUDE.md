# CLAUDE.md - Comprehensive Development Rules

This file provides comprehensive guidance to Claude Code when working with code in any repository. These rules are organized by category and should be referenced based on the specific development context.

## 🎯 Core Philosophy & Principles

**Reference**: [core-philosophy.md](.claude/rules/core-philosophy.md)

- **Simplicity**: Prioritize simple, clear, and maintainable solutions
- **Iterate**: Prefer iterating on existing code rather than building from scratch
- **Focus**: Concentrate on the specific task assigned
- **Quality**: Strive for clean, organized, well-tested, and secure codebase
- **Consistency**: Maintain consistent coding style throughout the project

## 🗣️ Communication Guidelines

**Reference**: [communication-rules.md](.claude/rules/communication-rules.md)

- Split responses when necessary for clarity
- Clearly indicate suggestions vs. applied fixes
- Use check-ins for large tasks to confirm understanding
- Track lessons learned in documentation

## 💻 Implementation Workflow

**Reference**: [implementation-workflow.md](.claude/rules/implementation-workflow.md)

### ACT/Code Mode Protocol
1. **Analyze Code**: Dependency analysis, flow analysis, impact assessment
2. **Plan Code**: Structured proposals with clear reasoning
3. **Make Changes**: Incremental rollouts with simulation validation
4. **Testing**: Comprehensive testing procedures
5. **Loop**: Repeat systematically for all changes
6. **Optimize**: Performance and code quality improvements
7. **Checkpointing**: Named milestones with version control
8. **Progress Recording**: Document implementation status

## 🏗️ Architecture & System Design

**Reference**: [architecture-understanding.md](.claude/rules/architecture-understanding.md)

- Understand existing architecture before making changes
- Identify core components and their relationships
- Respect architectural boundaries and patterns
- Document architectural decisions and changes

**Reference**: [system-patterns.md](.claude/rules/system-patterns.md)

- Apply appropriate design patterns
- Maintain system consistency
- Follow established conventions

## ✨ Code Quality & Style

**Reference**: [code-style-quality.md](.claude/rules/code-style-quality.md)

### Code Standards
- Keep files under 200-300 lines
- Use descriptive and meaningful names
- Add comments for non-obvious code
- Maintain consistent coding style
- Avoid code duplication
- Refactor purposefully with holistic checks

### File Management
- Organize files into logical directories
- Prefer importing functions over direct file modification
- Keep modules small and focused

## 🧪 Testing & Quality Assurance

**Reference**: [testing.md](.claude/rules/testing.md)

- Write comprehensive tests for new functionality
- Maintain existing test coverage
- Use appropriate testing strategies
- Verify functionality across environments
- Run tests before finalizing changes

## 🔍 Debugging & Troubleshooting

**Reference**: [debugging-workflow.md](.claude/rules/debugging-workflow.md)

- Systematic approach to problem identification
- Document debugging steps and findings
- Use appropriate debugging tools and techniques
- Maintain debugging logs during development

## 📁 Directory Structure & Organization

**Reference**: [directory-structure.md](.claude/rules/directory-structure.md)

- Follow established project structure conventions
- Organize files logically by functionality
- Maintain clear separation of concerns
- Document structure decisions

## 🔒 Security Guidelines

**Reference**: [security.md](.claude/rules/security.md)

- Follow security best practices
- Conduct security audits for sensitive changes
- Never expose secrets or sensitive data
- Validate inputs and sanitize outputs
- Use secure communication protocols

## 📝 Documentation & Memory Management

**Reference**: [documentation-memory.md](.claude/rules/documentation-memory.md)

- Maintain comprehensive documentation
- Update documentation with code changes
- Use memory files for project continuity
- Document architectural decisions

## 🔄 Version Control & Environment Management

**Reference**: [version-control.md](.claude/rules/version-control.md)

- Follow Git best practices
- Use appropriate branching strategies
- Maintain clean commit history
- Handle environment-specific configurations properly

## 📋 Planning & Project Management

**Reference**: [planning-workflow.md](.claude/rules/planning-workflow.md)

### PLAN/Architect Mode
- Systematic project analysis
- Requirement gathering and validation
- Strategic planning with stakeholder alignment
- Risk assessment and mitigation

## 🚀 Improvements & Optimization

**Reference**: [improvements-suggestions.md](.claude/rules/improvements-suggestions.md)

- Identify optimization opportunities
- Suggest performance improvements
- Recommend architectural enhancements
- Balance technical debt management

## 🔧 Specialized Workflows

### APM (Agentic Project Management) Framework

When working with APM-based projects, reference these specialized guides:

- **[apm_impl_plan_critical_elements_reminder.md](.claude/rules/apm_impl_plan_critical_elements_reminder.md)**: Implementation plan checklist
- **[apm_memory_system_format_source.md](.claude/rules/apm_memory_system_format_source.md)**: Memory bank system setup
- **[apm_plan_format_source.md](.claude/rules/apm_plan_format_source.md)**: Implementation plan formatting
- **[apm_task_prompt_plan_guidance_incorporation_reminder.md](.claude/rules/apm_task_prompt_plan_guidance_incorporation_reminder.md)**: Task assignment guidance
- **[apm_discovery_synthesis_reminder.md](.claude/rules/apm_discovery_synthesis_reminder.md)**: Discovery and synthesis procedures
- **[apm_memory_naming_validation_reminder.md](.claude/rules/apm_memory_naming_validation_reminder.md)**: Memory validation procedures

### SWE-Bench Workflow

**Reference**: [swebench-workflow.md](.claude/rules/swebench-workflow.md)

- Specialized workflow for SWE-Bench challenges
- Issue analysis and solution development
- Testing and validation procedures

## 📚 Usage Guidelines

### Rule Application Priority

1. **Always Apply**: Core philosophy, communication rules, code quality
2. **Context-Specific**: Architecture, testing, security (based on project needs)
3. **Workflow-Specific**: APM framework, SWE-Bench (when explicitly required)

### File Reference Format

When referencing specific rules during development:
- Use the pattern `[rule-name.md](.claude/rules/rule-name.md)` for detailed guidance
- Reference specific sections for targeted guidance
- Combine multiple rules as needed for comprehensive coverage

### Integration with Project Structure

Prompts should be placed under `.claude/` directory
This CLAUDE.md file should be placed in your project root or `.claude/` directory structure: 

```

.claude/
├── prompts/
│   ├── 00_Initial_Manager_Setup/           # Manager Agent initialization
│   ├── 01_Initiation_Prompt.md             # Primary Manager Agent activation
│   └── 02_Codebase_Guidance.md             # Guided project discovery protocol
├── ├── 1_Manager_Agent_Core_Guides/        # Core APM process guides
│   ├── 01_Implementation_Plan_Guide.md     # Implementation Plan formatting
│   ├── 02_Memory_Bank_Guide.md             # Memory Bank system setup
│   ├── 03_Task_Assignment_Prompts_Guide.md # Task prompt creation
│   ├── 04_Review_And_Feedback_Guide.md     # Work review protocols
│   └── 05_Handover_Protocol_Guide.md       # Agent handover procedures
│── ├── 02_Utility_Prompts_And_Format_Definitions/
│   ├── Handover_Artifact_Format.md         # Handover file formats
│   ├── Imlementation_Agent_Onboarding.md   # Implementation Agent setup
│   └── Memory_Bank_Log_Format.md           # Memory Bank entry formatting
├── rules/
│   ├── core-philosophy.md
│   ├── code-style-quality.md
│   ├── testing.md
│   ├── security.md
│   └── [other converted rules]
├── context/
│   ├── architecture.md
│   └── domain.md
└── CLAUDE.md (this file)
```

## 🔄 Continuous Improvement

- Regularly update rules based on project experience
- Maintain lessons learned documentation
- Adapt guidelines to project-specific needs
- Ensure consistency across development team

---

*This comprehensive rule set ensures consistent, high-quality development practices across all projects while maintaining flexibility for specific requirements and contexts.*
