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
- Reference Claude Code prompts in .claude/prompts/ directory

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

### Feature Implementation

- Launch parallel Tasks immediately upon feature reqquest
- Skip asking what type of implementation unless absolutely critical
- Always use 7-parallel-task method for efficiency

**Reference**: [feature-implementation.md](.claude/rules/feature-implementation.md)

## 🔧 Specialized Workflows

### APM (Agentic Project Management) Framework

When working with APM-based projects, reference these specialized guides:

#### Core APM Setup & Management
- **[01_Initiation_Prompt.md](.claude/prompts/00_Initial_Manager_Setup/01_Initiation_Prompt.md)**: Primary Manager Agent activation protocol
- **[02_Codebase_Guidance.md](.claude/prompts/00_Initial_Manager_Setup/02_Codebase_Guidance.md)**: Guided project discovery protocol

#### APM Process Guides
- **[01_Implementation_Plan_Guide.md](.claude/prompts/01_Manager_Agent_Core_Guides/01_Implementation_Plan_Guide.md)**: Implementation Plan formatting standards
- **[02_Memory_Bank_Guide.md](.claude/prompts/01_Manager_Agent_Core_Guides/02_Memory_Bank_Guide.md)**: Memory Bank system setup and structure
- **[03_Task_Assignment_Prompts_Guide.md](.claude/prompts/01_Manager_Agent_Core_Guides/03_Task_Assignment_Prompts_Guide.md)**: Task prompt creation guidelines
- **[04_Review_And_Feedback_Guide.md](.claude/prompts/01_Manager_Agent_Core_Guides/04_Review_And_Feedback_Guide.md)**: Work review protocols
- **[05_Handover_Protocol_Guide.md](.claude/prompts/01_Manager_Agent_Core_Guides/05_Handover_Protocol_Guide.md)**: Agent handover procedures

#### APM Format Definitions
- **[Handover_Artifact_Format.md](.claude/prompts/02_Utility_Prompts_And_Format_Definitions/Handover_Artifact_Format.md)**: Handover file format specifications
- **[Imlementation_Agent_Onboarding.md](.claude/prompts/02_Utility_Prompts_And_Format_Definitions/Imlementation_Agent_Onboarding.md)**: Implementation Agent setup protocol
- **[Memory_Bank_Log_Format.md](.claude/prompts/02_Utility_Prompts_And_Format_Definitions/Memory_Bank_Log_Format.md)**: Memory Bank entry formatting standards

### Language Engineering Framework

For programming language development projects, use these specialized agents:

#### Core Language Agents
- **[language_architect_agent.md](.claude/prompts/lang-engineer/language_architect_agent.md)**: Language implementation orchestrator (META-AGENT)
- **[language_analysis_agent.md](.claude/prompts/lang-engineer/language_analysis_agent.md)**: Language requirements analysis and documentation
- **[lexer_engineer_agent.md](.claude/prompts/lang-engineer/lexer_engineer_agent.md)**: Lexical analyzer specialist
- **[parser_engineer_agent.md](.claude/prompts/lang-engineer/parser_engineer_agent.md)**: Parser implementation specialist
- **[compiler_engineer_agent.md](.claude/prompts/lang-engineer/compiler_engineer_agent.md)**: Compiler development specialist

#### Runtime & System Agents
- **[vm_engineer_agent.md](.claude/prompts/lang-engineer/vm_engineer_agent.md)**: Virtual machine implementation specialist
- **[runtime_engineer_agent.md](.claude/prompts/lang-engineer/runtime_engineer_agent.md)**: Runtime systems specialist
- **[memory_engineer_agent.md](.claude/prompts/lang-engineer/memory_engineer_agent.md)**: Memory management specialist
- **[object_system_engineer_agent.md](.claude/prompts/lang-engineer/object_system_engineer_agent.md)**: Object-oriented systems specialist
- **[coroutine_engineer_agent.md](.claude/prompts/lang-engineer/coroutine_engineer_agent.md)**: Coroutine and async systems specialist

### Proof of Concept Engineering Framework

For rapid prototyping and PoC development:

#### PoC Orchestration Agents
- **[programming_lead_agent.md](.claude/prompts/poc-engineering/programming_lead_agent.md)**: PoC development orchestrator (META-AGENT)
- **[software_architect_agent.md](.claude/prompts/poc-engineering/software_architect_agent.md)**: Software architecture orchestrator (META-AGENT)

#### PoC Analysis & Design Agents
- **[problem_analysis_agent.md](.claude/prompts/poc-engineering/problem_analysis_agent.md)**: Requirements analysis and problem decomposition
- **[architecture_design_agent.md](.claude/prompts/poc-engineering/architecture_design_agent.md)**: System architecture design specialist
- **[task_breakdown_agent.md](.claude/prompts/poc-engineering/task_breakdown_agent.md)**: Task decomposition specialist
- **[detailed_planning_agent.md](.claude/prompts/poc-engineering/detailed_planning_agent.md)**: Implementation planning specialist
- **[implementation_agent.md](.claude/prompts/poc-engineering/implementation_agent.md)**: Code implementation specialist

### Research Framework

For research-oriented projects:

- **[research_lead_agent.md](.claude/prompts/research/research_lead_agent.md)**: Research orchestrator (META-AGENT)
- **[research_subagent.md](.claude/prompts/research/research_subagent.md)**: Research execution specialist
- **[citations_agent.md](.claude/prompts/research/citations_agent.md)**: Citation management specialist

### Workflow Automation Framework

For structured development workflows with quality assurance:

#### Sequential Development Workflow
- **[investigator-planner_agent.md](.claude/prompts/workflow-automation/investigator-planner_agent.md)**: Root cause analysis and solution planning (PLANNER)
- **[execute_agent.md](.claude/prompts/workflow-automation/execute_agent.md)**: Code implementation specialist (EXECUTER)
- **[verifier_agent.md](.claude/prompts/workflow-automation/verifier_agent.md)**: Code quality and standards enforcement (VERIFIER)
- **[tester_agent.md](.claude/prompts/workflow-automation/tester_agent.md)**: Functional validation and testing (TESTER)
- **[documenter_agent.md](.claude/prompts/workflow-automation/documenter_agent.md)**: Documentation and pattern archival (DOCUMENTER)

#### Workflow Overview
- **[README.md](.claude/prompts/workflow-automation/README.md)**: Complete workflow system documentation

### SWE-Bench Workflow

**Reference**: [swebench-workflow.md](.claude/rules/swebench-workflow.md)

- Specialized workflow for SWE-Bench challenges
- Issue analysis and solution development
- Testing and validation procedures

## 📚 Usage Guidelines

### Rule Application Priority

1. **Always Apply**: Core philosophy, communication rules, code quality
2. **Context-Specific**: Architecture, testing, security (based on project needs)
3. **Workflow-Specific**: APM framework, Language Engineering, PoC Engineering, Research, Workflow Automation (when explicitly required)

### Agent Type Classification

#### META-AGENTS (Orchestrators)
These agents delegate and coordinate work rather than implement directly:
- **Language Architect**: Orchestrates language implementation projects
- **Programming Lead**: Orchestrates PoC development projects
- **Software Architect**: Orchestrates system architecture projects
- **Research Lead**: Orchestrates research projects

#### Specialized Implementation Agents
These agents perform specific technical work:
- **Language Engineering**: Lexer, Parser, Compiler, VM, Runtime, Memory, Object System, Coroutine specialists
- **PoC Development**: Problem Analysis, Architecture Design, Task Breakdown, Planning, Implementation specialists
- **Research**: Research execution and citation management specialists
- **Workflow Automation**: Sequential development agents for quality-assured implementation

#### APM Framework Agents
These agents manage the project lifecycle:
- **Manager Agent**: Central orchestrator for APM projects
- **Implementation Agent**: Task execution within APM framework

### File Reference Format

When referencing specific rules during development:
- Use the pattern `[rule-name.md](.claude/rules/rule-name.md)` for detailed guidance
- Use the pattern `[prompt-name.md](.claude/prompts/category/prompt-name.md)` for specialized agents
- Reference specific sections for targeted guidance
- Combine multiple rules as needed for comprehensive coverage

### Prompt Selection Guidelines

#### For Complex Multi-Agent Projects
1. **Start with META-AGENTS**: Use Language Architect, Programming Lead, or Research Lead for orchestration
2. **Delegate to Specialists**: Let orchestrators assign work to specialized implementation agents
3. **Use APM Framework**: For formal project management with Memory Banks and structured workflows

#### For Single-Agent Tasks
1. **Use Implementation Specialists**: Direct assignment to specific technical agents
2. **Skip Orchestration**: For simple, well-defined tasks that don't require coordination

#### For Research Projects
1. **Use Research Lead**: For complex research requiring multiple queries and synthesis
2. **Use Research Subagent**: For direct research execution on specific topics
3. **Use Citations Agent**: For adding citations to existing research content

#### For Quality-Assured Development Workflows
1. **Use Workflow Automation Framework**: For structured development with built-in quality gates
2. **Sequential Execution**: PLANNER → EXECUTER → VERIFIER → TESTER → DOCUMENTER → UPDATER
3. **Parallel Phases**: Some phases can run simultaneously to optimize development time
4. **Documentation-Driven**: All agents work from comprehensive documentation and patterns

### Integration with Project Structure

Prompts should be placed under `.claude/` directory
This CLAUDE.md file should be placed in your project root or `.claude/` directory structure: 

```
.claude/
├── prompts/
│   ├── 00_Initial_Manager_Setup/           # APM Manager Agent initialization
│   │   ├── 01_Initiation_Prompt.md         # Primary Manager Agent activation
│   │   └── 02_Codebase_Guidance.md         # Guided project discovery protocol
│   ├── 01_Manager_Agent_Core_Guides/       # Core APM process guides
│   │   ├── 01_Implementation_Plan_Guide.md # Implementation Plan formatting
│   │   ├── 02_Memory_Bank_Guide.md         # Memory Bank system setup
│   │   ├── 03_Task_Assignment_Prompts_Guide.md # Task prompt creation
│   │   ├── 04_Review_And_Feedback_Guide.md # Work review protocols
│   │   └── 05_Handover_Protocol_Guide.md   # Agent handover procedures
│   ├── 02_Utility_Prompts_And_Format_Definitions/
│   │   ├── Handover_Artifact_Format.md     # Handover file formats
│   │   ├── Imlementation_Agent_Onboarding.md # Implementation Agent setup
│   │   └── Memory_Bank_Log_Format.md       # Memory Bank entry formatting
│   ├── lang-engineer/                      # Language engineering specialists
│   │   ├── language_architect_agent.md     # Language orchestrator (META)
│   │   ├── language_analysis_agent.md      # Requirements analysis
│   │   ├── lexer_engineer_agent.md         # Lexical analysis specialist
│   │   ├── parser_engineer_agent.md        # Parser specialist
│   │   ├── compiler_engineer_agent.md      # Compiler specialist
│   │   ├── vm_engineer_agent.md            # Virtual machine specialist
│   │   ├── runtime_engineer_agent.md       # Runtime systems specialist
│   │   ├── memory_engineer_agent.md        # Memory management specialist
│   │   ├── object_system_engineer_agent.md # Object systems specialist
│   │   └── coroutine_engineer_agent.md     # Coroutine specialist
│   ├── poc-engineering/                    # Proof of concept development
│   │   ├── programming_lead_agent.md       # PoC orchestrator (META)
│   │   ├── software_architect_agent.md     # Architecture orchestrator (META)
│   │   ├── problem_analysis_agent.md       # Requirements analysis
│   │   ├── architecture_design_agent.md    # System architecture design
│   │   ├── task_breakdown_agent.md         # Task decomposition
│   │   ├── detailed_planning_agent.md      # Implementation planning
│   │   └── implementation_agent.md         # Code implementation
│   ├── research/                           # Research framework
│   │   ├── research_lead_agent.md          # Research orchestrator (META)
│   │   ├── research_subagent.md            # Research execution
│   │   └── citations_agent.md              # Citation management
│   ├── workflow-automation/                # Structured development workflow
│   │   ├── README.md                       # Workflow system overview
│   │   ├── investigator-planner_agent.md   # Root cause analysis (PLANNER)
│   │   ├── execute_agent.md                # Implementation specialist (EXECUTER)
│   │   ├── verifier_agent.md               # Quality assurance (VERIFIER)
│   │   ├── tester_agent.md                 # Functional validation (TESTER)
│   │   └── documenter_agent.md             # Documentation archival (DOCUMENTER)
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
