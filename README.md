# Claude Code Development Rules & Multi-Agent Framework

This repository contains a comprehensive collection of development rules, guidelines, and 26 specialized agent prompts designed for Claude Code. These resources provide consistent, high-quality development practices across diverse project types and requirements, featuring four distinct multi-agent frameworks for different development scenarios.

## 📁 Repository Structure

```
claude-rules/
├── README.md                                                # This file
├── CLAUDE.md                                                # Main rules file (references all others)
└── .claude/
    ├── prompts/                                             # Claude Code prompt templates (26 agents)
    │   ├── 00_Initial_Manager_Setup/                        # Manager Agent initialization (2 files)
    │   │   ├── 01_Initiation_Prompt.md                      # Primary Manager Agent activation
    │   │   └── 02_Codebase_Guidance.md                      # Guided project discovery protocol
    │   ├── 01_Manager_Agent_Core_Guides/                    # Core APM process guides (5 files)
    │   │   ├── 01_Implementation_Plan_Guide.md              # Implementation Plan formatting
    │   │   ├── 02_Memory_Bank_Guide.md                      # Memory Bank system setup
    │   │   ├── 03_Task_Assignment_Prompts_Guide.md          # Task prompt creation
    │   │   ├── 04_Review_And_Feedback_Guide.md              # Work review protocols
    │   │   └── 05_Handover_Protocol_Guide.md                # Agent handover procedures
    │   ├── 02_Utility_Prompts_And_Format_Definitions/       # Utility prompts and formats (3 files)
    │   │   ├── Handover_Artifact_Format.md                  # Handover file formats
    │   │   ├── Imlementation_Agent_Onboarding.md            # Implementation Agent setup
    │   │   └── Memory_Bank_Log_Format.md                    # Memory Bank entry formatting
    │   ├── lang-engineer/                                   # Language Engineering Framework (10 agents)
    │   │   ├── language_architect_agent.md                  # Language orchestrator (META-AGENT)
    │   │   ├── language_analysis_agent.md                   # Requirements analysis
    │   │   ├── lexer_engineer_agent.md                      # Lexical analysis specialist
    │   │   ├── parser_engineer_agent.md                     # Parser specialist
    │   │   ├── compiler_engineer_agent.md                   # Compiler specialist
    │   │   ├── vm_engineer_agent.md                         # Virtual machine specialist
    │   │   ├── runtime_engineer_agent.md                    # Runtime systems specialist
    │   │   ├── memory_engineer_agent.md                     # Memory management specialist
    │   │   ├── object_system_engineer_agent.md              # Object systems specialist
    │   │   └── coroutine_engineer_agent.md                  # Coroutine specialist
    │   ├── poc-engineering/                                 # PoC Engineering Framework (7 agents)
    │   │   ├── programming_lead_agent.md                    # PoC orchestrator (META-AGENT)
    │   │   ├── software_architect_agent.md                  # Architecture orchestrator (META-AGENT)
    │   │   ├── problem_analysis_agent.md                    # Requirements analysis
    │   │   ├── architecture_design_agent.md                 # System architecture design
    │   │   ├── task_breakdown_agent.md                      # Task decomposition
    │   │   ├── detailed_planning_agent.md                   # Implementation planning
    │   │   └── implementation_agent.md                      # Code implementation
    │   ├── research/                                        # Research Framework (3 agents)
    │   │   ├── research_lead_agent.md                       # Research orchestrator (META-AGENT)
    │   │   ├── research_subagent.md                         # Research execution
    │   │   └── citations_agent.md                           # Citation management
    │   └── workflow-automation/                             # Workflow Automation Framework (6 agents)
    │       ├── README.md                                    # Workflow system overview
    │       ├── investigator-planner_agent.md                # Root cause analysis (PLANNER)
    │       ├── execute_agent.md                             # Implementation specialist (EXECUTER)
    │       ├── verifier_agent.md                            # Quality assurance (VERIFIER)
    │       ├── tester_agent.md                              # Functional validation (TESTER)
    │       └── documenter_agent.md                          # Documentation archival (DOCUMENTER)
    └── rules/                                               # Development rules (21 files)
        ├── core-philosophy.md                               # Core development principles
        ├── communication-rules.md                           # AI communication guidelines
        ├── implementation-workflow.md                       # ACT/Code mode procedures
        ├── planning-workflow.md                             # PLAN/Architect mode procedures
        ├── code-style-quality.md                            # Code quality standards
        ├── testing.md                                       # Testing procedures
        ├── debugging-workflow.md                            # Debugging protocols
        ├── security.md                                      # Security guidelines
        ├── architecture-understanding.md                    # Architecture adherence
        ├── system-patterns.md                               # System design patterns
        ├── directory-structure.md                           # Project organization
        ├── documentation-memory.md                          # Documentation standards
        ├── version-control.md                               # Git and environment management
        ├── improvements-suggestions.md                      # Optimization guidelines
        ├── swebench-workflow.md                             # SWE-Bench specialized workflow
        └── apm_*.md                                         # APM framework rules (6 files)
```

## 🚀 How to Use These Rules

### Option 1: Complete Integration (Recommended)
Copy the entire `.claude` directory to your project root:

```bash
cp -r .claude /path/to/your/project/
```

### Option 2: Single File Integration
Copy only the main rules file:

```bash
cp CLAUDE.md /path/to/your/project/
```

### Option 3: Selective Rules
Choose specific rules for your project:

```bash
mkdir -p /path/to/your/project/.claude/rules
cp .claude/rules/core-philosophy.md /path/to/your/project/.claude/rules/
cp .claude/rules/code-style-quality.md /path/to/your/project/.claude/rules/
# Copy other relevant rules...
```

## 🤖 Multi-Agent Frameworks

### 🔧 Language Engineering Framework (10 Agents)
**Purpose**: Build programming languages, compilers, and runtime systems
- **Language Architect Agent** (META-AGENT) - Orchestrates language development projects
- **Language Analysis Agent** - Requirements analysis and documentation
- **Lexer Engineer Agent** - Lexical analyzer specialist
- **Parser Engineer Agent** - Parser implementation specialist
- **Compiler Engineer Agent** - Compiler development specialist
- **VM Engineer Agent** - Virtual machine implementation specialist
- **Runtime Engineer Agent** - Runtime systems specialist
- **Memory Engineer Agent** - Memory management specialist
- **Object System Engineer Agent** - Object-oriented systems specialist
- **Coroutine Engineer Agent** - Coroutine and async systems specialist

### 🚀 PoC Engineering Framework (7 Agents)
**Purpose**: Rapid prototyping and proof-of-concept development
- **Programming Lead Agent** (META-AGENT) - PoC development orchestrator
- **Software Architect Agent** (META-AGENT) - Software architecture orchestrator
- **Problem Analysis Agent** - Requirements analysis and problem decomposition
- **Architecture Design Agent** - System architecture design specialist
- **Task Breakdown Agent** - Task decomposition specialist
- **Detailed Planning Agent** - Implementation planning specialist
- **Implementation Agent** - Code implementation specialist

### 🔍 Research Framework (3 Agents)
**Purpose**: Research-oriented projects and documentation
- **Research Lead Agent** (META-AGENT) - Research orchestrator
- **Research Subagent** - Research execution specialist
- **Citations Agent** - Citation management specialist

### ⚙️ Workflow Automation Framework (6 Agents)
**Purpose**: Structured development workflows with quality assurance
- **Investigator-Planner Agent** (PLANNER) - Root cause analysis and solution planning
- **Execute Agent** (EXECUTER) - Code implementation specialist
- **Verifier Agent** (VERIFIER) - Code quality and standards enforcement
- **Tester Agent** (TESTER) - Functional validation and testing
- **Documenter Agent** (DOCUMENTER) - Documentation and pattern archival

### 📝 APM Framework (Classic)
**Purpose**: Agentic Project Management with Memory Banks
- **Manager Agent** - Central project orchestrator
- **Implementation Agent** - Task execution within APM framework
- **Memory Bank System** - Project continuity and knowledge management

## 📋 Rule Categories

### 🎯 Core Rules (Always Apply)
- **`core-philosophy.md`** - Fundamental development principles
- **`communication-rules.md`** - AI interaction guidelines  
- **`code-style-quality.md`** - Code quality standards

### 🔧 Workflow Rules (Context-Specific)
- **`implementation-workflow.md`** - Step-by-step implementation procedures
- **`planning-workflow.md`** - Project planning and architecture
- **`debugging-workflow.md`** - Problem-solving protocols

### 🏗️ Architecture Rules (Project-Specific)
- **`architecture-understanding.md`** - System design adherence
- **`system-patterns.md`** - Design pattern application
- **`directory-structure.md`** - Project organization

### 🔒 Quality Assurance Rules
- **`testing.md`** - Comprehensive testing procedures
- **`security.md`** - Security best practices
- **`version-control.md`** - Git and environment management

### 📝 Documentation Rules
- **`documentation-memory.md`** - Documentation standards
- **`improvements-suggestions.md`** - Optimization guidelines

### 🤖 Specialized Workflows
- **`swebench-workflow.md`** - SWE-Bench challenge procedures
- **`apm_*.md`** - Agentic Project Management framework (6 specialized files)

## 🎯 Usage Examples

### For a New Project
```bash
# Copy the complete rule set and all agent frameworks
cp -r .claude /path/to/new/project/
cp CLAUDE.md /path/to/new/project/

# Or just the main file for simple projects
cp CLAUDE.md /path/to/new/project/
```

### For an Existing Project
```bash
# Review your current practices, then integrate relevant rules
mkdir -p /path/to/existing/project/.claude
cp CLAUDE.md /path/to/existing/project/
cp -r .claude/rules /path/to/existing/project/.claude/
cp -r .claude/prompts /path/to/existing/project/.claude/
```

### For Specialized Frameworks

#### Language Engineering Projects
```bash
# Building compilers, interpreters, or programming languages
cp -r .claude/prompts/lang-engineer /path/to/project/.claude/prompts/
cp CLAUDE.md /path/to/project/

# Example usage:
# Use Language Architect Agent as orchestrator
# Delegate to specialized agents (lexer, parser, compiler, VM, etc.)
```

#### PoC Engineering Projects
```bash
# Rapid prototyping and proof-of-concept development
cp -r .claude/prompts/poc-engineering /path/to/project/.claude/prompts/
cp CLAUDE.md /path/to/project/

# Example usage:
# Use Programming Lead Agent for coordination
# Use Software Architect Agent for system design
# Use specialized agents for analysis, planning, and implementation
```

#### Research Projects
```bash
# Academic research, documentation, or analysis projects
cp -r .claude/prompts/research /path/to/project/.claude/prompts/
cp CLAUDE.md /path/to/project/

# Example usage:
# Use Research Lead Agent for coordination
# Use Research Subagent for execution
# Use Citations Agent for reference management
```

#### Workflow Automation Projects
```bash
# Structured development with quality gates
cp -r .claude/prompts/workflow-automation /path/to/project/.claude/prompts/
cp CLAUDE.md /path/to/project/

# Example usage:
# Sequential workflow: PLANNER → EXECUTER → VERIFIER → TESTER → DOCUMENTER
# Each agent has specific quality gates and responsibilities
```

#### APM (Classic) Projects
```bash
# Traditional Agentic Project Management with Memory Banks
cp .claude/rules/apm_*.md /path/to/project/.claude/rules/
cp -r .claude/prompts/00_Initial_Manager_Setup /path/to/project/.claude/prompts/
cp -r .claude/prompts/01_Manager_Agent_Core_Guides /path/to/project/.claude/prompts/
cp -r .claude/prompts/02_Utility_Prompts_And_Format_Definitions /path/to/project/.claude/prompts/
```

#### SWE-Bench Projects
```bash
# Specialized workflow for software engineering benchmarks
cp .claude/rules/swebench-workflow.md /path/to/project/.claude/rules/
```

#### Security-Critical Projects
```bash
# Enhanced security requirements
cp .claude/rules/security.md /path/to/project/.claude/rules/
```

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

## 🛠️ Customization Guidelines

### Adapting Rules to Your Project
1. **Technology Stack**: Modify technology-specific references in rules
2. **Team Size**: Adjust collaboration guidelines accordingly
3. **Project Complexity**: Scale workflow procedures as needed
4. **Industry Requirements**: Add domain-specific security or compliance rules

### Adding Project-Specific Rules
Create additional `.md` files in `.claude/rules/` for:
- Technology-specific patterns (`react.md`, `python.md`, etc.)
- Domain-specific logic (`finance.md`, `healthcare.md`, etc.)
- Team conventions (`code-review.md`, `deployment.md`, etc.)

Then update `CLAUDE.md` to reference your new rules.

## 🔧 Integration with Claude Code

### Setup
1. Ensure `CLAUDE.md` is in your project root, above `.claude` directory
2. Claude Code will automatically detect and use these rules
3. Reference specific rules in code comments when needed
4. Use prompt templates from `.claude/prompts/` for structured workflows

### Usage in Development
1. Review applicable rules before starting new features
2. Reference rules during code reviews
3. Use rule names in prompts for targeted guidance
4. Leverage multi-agent frameworks for complex projects
5. Update rules based on project learnings

### Multi-Agent Framework Usage

#### For Language Development Projects
```bash
# Use Language Architect Agent as orchestrator
@language_architect_agent "Build a functional programming language with pattern matching"

# Or use specialized agents directly
@lexer_engineer_agent "Design lexer for functional language with ML-style syntax"
@parser_engineer_agent "Implement parser for pattern matching expressions"
```

#### For PoC Development
```bash
# Use Programming Lead Agent for coordination
@programming_lead_agent "Create a real-time collaborative editing system"

# Or use Software Architect Agent for system design
@software_architect_agent "Design architecture for distributed document editing"
```

#### For Research Projects
```bash
# Use Research Lead Agent for comprehensive research
@research_lead_agent "Research modern approaches to distributed consensus algorithms"

# Or use Research Subagent for specific topics
@research_subagent "Find recent papers on Byzantine fault tolerance in blockchain systems"
```

#### For Quality-Assured Development
```bash
# Use sequential workflow agents
@investigator_planner_agent "Users experiencing session timeout issues"
@execute_agent "Implement session management improvements"
@verifier_agent "Validate code quality and standards"
@tester_agent "Test session timeout scenarios"
@documenter_agent "Document session management patterns"
```

#### For Traditional APM Projects
```bash
# Use Manager Agent for project coordination
@manager_agent "Initialize project management for e-commerce platform"

# Use Implementation Agent for specific tasks
@implementation_agent "Implement user authentication system"
```

### Prompt Templates Usage
- **Manager Setup**: Use `00_Initial_Manager_Setup/` prompts to initialize APM workflows
- **Implementation Planning**: Reference `01_Manager_Agent_Core_Guides/` for structured development
- **Handover Protocols**: Apply `02_Utility_Prompts_And_Format_Definitions/` for agent transitions
- **Memory Management**: Utilize memory bank formats for project continuity
- **Framework Selection**: Choose appropriate multi-agent framework based on project type

## 📈 Rule Maintenance

### Regular Review
- Update rules based on project experience
- Collect feedback from development team
- Adapt rules to evolving best practices
- Maintain version history of rule changes

### Version Control
- Track rule modifications in git
- Document reasoning for rule changes
- Create branches for experimental rule updates
- Tag stable rule versions

---

## 🎯 Framework Selection Guide

### Choose Your Framework Based on Project Type:

| Project Type | Recommended Framework | Key Benefits |
|-------------|----------------------|-------------|
| **Programming Language Development** | Language Engineering (10 agents) | Specialized agents for lexer, parser, compiler, VM, runtime systems |
| **Rapid Prototyping** | PoC Engineering (7 agents) | Fast problem analysis, architecture design, and implementation |
| **Research Projects** | Research (3 agents) | Comprehensive research capabilities with citation management |
| **Quality-Critical Development** | Workflow Automation (6 agents) | Sequential quality gates with verification and testing |
| **Traditional Project Management** | APM Framework (Classic) | Memory banks, structured handovers, and formal project management |

### Agent Classification:
- **META-AGENTS**: Orchestrate and delegate work (Language Architect, Programming Lead, Software Architect, Research Lead)
- **Specialists**: Perform specific technical work (all other agents)
- **Use META-AGENTS** for complex multi-phase projects requiring coordination
- **Use Specialists** for focused, single-domain tasks

---

*This comprehensive multi-agent framework provides 26 specialized agents across 4 distinct frameworks, enabling sophisticated development workflows for any project type. From programming language development to research projects, each framework is designed for optimal efficiency and quality assurance with Claude Code.*
