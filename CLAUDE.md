# CLAUDE.md - Comprehensive Development Rules

This file provides comprehensive guidance to Claude Code when working with code in any repository. These rules are organized by category and should be referenced based on the specific development context.

## 🎯 Core Philosophy & Principles

- **Simplicity**: Prioritize simple, clear, and maintainable solutions
- **Iterate**: Prefer iterating on existing code rather than building from scratch  
- **Focus**: Concentrate on the specific task assigned
- **Quality**: Strive for clean, organized, well-tested, and secure codebase
- **Consistency**: Maintain consistent coding style throughout the project

## 💻 Development Workflow

**Reference**: [01-development-workflow.md](.claude/rules/01-development-workflow.md)

### MODE Selection & Systematic Process
- **PLAN MODE**: Architecture, planning, requirements analysis
- **ACT MODE**: Implementation, coding, testing
- Systematic development protocol with analysis, implementation, and validation phases

### Key Workflow Elements
- Requirements understanding and code analysis
- Incremental rollouts with simulation validation
- Architecture adherence and quality standards
- Checkpointing and progress recording

## 🧪 Testing & Security

**Reference**: [02-testing-security.md](.claude/rules/02-testing-security.md)

### Testing Framework
- **TDD Focus**: Test-driven development with comprehensive coverage
- **Bug Fix Protocol**: Write reproducing tests before fixes
- **No Breakage Assertion**: All tests must pass before committing
- Test planning with edge case coverage

### Security Framework
- **3-Phase Security Audit**: Analysis → Planning → Implementation
- **Security Principles**: Server-side authority, input sanitization, credential protection
- **Key Focus Areas**: Authentication, input validation, exposed credentials, IDOR

## 🗣️ Communication & Documentation

**Reference**: [03-communication-documentation.md](.claude/rules/03-communication-documentation.md)

### Communication Standards
- **Clarity First**: Clear, specific communication with context
- **Split Responses**: Multiple responses when needed for clarity
- **Confirmation Protocol**: Check-ins for complex tasks
- **Incremental Steps**: Break down complex tasks

### Memory Files Structure
#### Core Files (Required)
1. **`docs/product_requirement_docs.md`**: PRD/SOP (Why, goals, scope)
2. **`docs/architecture.md`**: System architecture (How, components, dependencies)  
3. **`docs/technical.md`**: Dev environment, stack, tech decisions, patterns
4. **`tasks/tasks_plan.md`**: Detailed task backlog, progress, status, issues
5. **`tasks/active_context.md`**: Current work focus, decisions, recent changes
6. **`.claude/rules/05-error-documentation.md`**: Reusable fixes, known issues log
7. **`.claude/rules/06-lessons-learned.md`**: Learning journal (patterns, preferences)

## ✨ Code Quality & Standards

**Reference**: [04-code-quality-standards.md](.claude/rules/04-code-quality-standards.md)

### Core Quality Principles
- **Clean Code**: Readable, maintainable, self-documenting code
- **DRY Principle**: Eliminate code duplication through abstraction
- **KISS Principle**: Choose simplest solutions that meet requirements
- **Modularity**: Atomic functions, single responsibility, clear interfaces

### Code Organization Standards
- **File Management**: Target < 200-300 lines per file
- **Directory Structure**: Logical organization with clear naming
- **Import Strategy**: Prefer specific function imports
- **Dependency Management**: Minimize and clearly define dependencies

### Quality Assurance Process
- **Pre-Commit Checks**: Formatting, linting, testing, security scans
- **Code Reviews**: DRY/KISS compliance, performance, readability, security
- **Continuous Improvement**: Regular refactoring and pattern analysis

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

1. **Always Apply**: 
   - Core philosophy and principles
   - [01-development-workflow.md](.claude/rules/01-development-workflow.md) - Development process and standards
   - [04-code-quality-standards.md](.claude/rules/04-code-quality-standards.md) - Code quality and organization
   - [03-communication-documentation.md](.claude/rules/03-communication-documentation.md) - Communication and documentation standards

2. **Context-Specific**: 
   - [02-testing-security.md](.claude/rules/02-testing-security.md) - Applied based on project security requirements and testing needs

3. **Workflow-Specific**: 
   - APM framework, Language Engineering, PoC Engineering, Research, Workflow Automation (when explicitly required by project type)

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
- Use the pattern `[##-rule-name.md](.claude/rules/##-rule-name.md)` for core development rules
- Use the pattern `[prompt-name.md](.claude/prompts/category/prompt-name.md)` for specialized agents
- Reference specific sections within rules for targeted guidance
- Combine multiple rules as needed for comprehensive coverage

#### Core Rule References
- **Development Process**: [01-development-workflow.md](.claude/rules/01-development-workflow.md)
- **Testing & Security**: [02-testing-security.md](.claude/rules/02-testing-security.md)  
- **Communication & Docs**: [03-communication-documentation.md](.claude/rules/03-communication-documentation.md)
- **Code Quality**: [04-code-quality-standards.md](.claude/rules/04-code-quality-standards.md)

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
│   ├── 01-development-workflow.md
│   ├── 02-testing-security.md
│   ├── 03-communication-documentation.md
│   ├── 04-code-quality-standards.md
│   ├── 05-error-documentation.md
│   └── 06-lessons-learned.md
├── context/
│   ├── architecture.md
│   └── domain.md
└── CLAUDE.md (this file)
```

## 🔄 Rule Management & Continuous Improvement

### How to Use This Index

1. **Start Here**: Use this CLAUDE.md as your central reference index
2. **Follow Links**: Click rule references to access detailed guidelines  
3. **Apply Systematically**: Use the Rule Application Priority as your guide
4. **Context-Aware**: Select specialized workflows based on project type
5. **Document Learning**: Update 05-error-documentation.md and 06-lessons-learned.md as you work

### Updating Rules

- **Core Rules**: Modify files in `.claude/rules/` for fundamental changes
- **Specialized Workflows**: Update prompts in `.claude/prompts/` for agent-specific guidance
- **Index Updates**: Update this CLAUDE.md when adding new rule files or major restructuring
- **Version Control**: Always commit rule changes to maintain consistency across sessions

### Rule Validation

- Ensure all referenced files exist and are accessible
- Validate that rule links point to correct locations
- Test specialized workflows before documenting them
- Keep rule content aligned with actual development practices

### Continuous Improvement Process

- **Regular Review**: Periodically review rules for relevance and accuracy
- **Experience Integration**: Update rules based on project learnings and challenges
- **Pattern Recognition**: Document recurring patterns in 06-lessons-learned.md
- **Error Prevention**: Log common issues in 05-error-documentation.md
- **Team Alignment**: Ensure rules reflect team consensus and best practices

---

*This comprehensive rule index ensures consistent, high-quality development practices across all projects while maintaining flexibility for specific requirements and contexts. The structured approach with core rules and specialized workflows provides both foundational guidance and advanced capabilities for complex projects.*
