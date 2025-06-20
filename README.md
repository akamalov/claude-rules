# Claude Code Development Rules

This repository contains a comprehensive collection of development rules, guidelines, and prompt templates specifically designed for Claude Code. These resources provide consistent, high-quality development practices across diverse project types and requirements, along with structured prompt templates for Agentic Project Management (APM) workflows.

## 📁 Repository Structure

```
claude-rules/
├── README.md                                                # This file
├── CLAUDE.md                                                # Main rules file (references all others)
└── .claude/
    ├── prompts/                                             # Claude Code prompt templates
    │   ├── 00_Initial_Manager_Setup/                        # Manager Agent initialization
    │   │   ├── 01_Initiation_Prompt.md                      # Primary Manager Agent activation
    │   │   └── 02_Codebase_Guidance.md                      # Guided project discovery protocol
    │   ├── 01_Manager_Agent_Core_Guides/                    # Core APM process guides
    │   │   ├── 01_Implementation_Plan_Guide.md              # Implementation Plan formatting
    │   │   ├── 02_Memory_Bank_Guide.md                      # Memory Bank system setup
    │   │   ├── 03_Task_Assignment_Prompts_Guide.md          # Task prompt creation
    │   │   ├── 04_Review_And_Feedback_Guide.md              # Work review protocols
    │   │   └── 05_Handover_Protocol_Guide.md                # Agent handover procedures
    │   └── 02_Utility_Prompts_And_Format_Definitions/
    │       ├── Handover_Artifact_Format.md                  # Handover file formats
    │       ├── Imlementation_Agent_Onboarding.md            # Implementation Agent setup
    │       └── Memory_Bank_Log_Format.md                    # Memory Bank entry formatting
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

### 📝 Prompt Templates
- **`00_Initial_Manager_Setup/`** - Manager Agent initialization prompts (2 files)
- **`01_Manager_Agent_Core_Guides/`** - Core APM process guides (5 files)
- **`02_Utility_Prompts_And_Format_Definitions/`** - Utility prompts and formats (3 files)

## 🎯 Usage Examples

### For a New Project
```bash
# Copy the complete rule set
cp -r .claude /path/to/new/project/

# Or just the main file
cp .claude/CLAUDE.md /path/to/new/project/
```

### For an Existing Project
```bash
# Review your current practices, then integrate relevant rules
mkdir -p /path/to/existing/project/.claude
cp .claude/CLAUDE.md /path/to/existing/project/.claude/
cp -r .claude/rules /path/to/existing/project/.claude/
```

### For Specialized Workflows
```bash
# APM Projects - include all APM files and prompts
cp .claude/rules/apm_*.md /path/to/project/.claude/rules/
cp -r .claude/prompts /path/to/project/.claude/

# SWE-Bench Projects
cp .claude/rules/swebench-workflow.md /path/to/project/.claude/rules/

# Security-Critical Projects
cp .claude/rules/security.md /path/to/project/.claude/rules/

# Manager Agent Setup - APM workflow initialization
cp -r .claude/prompts/00_Initial_Manager_Setup /path/to/project/.claude/prompts/
cp -r .claude/prompts/01_Manager_Agent_Core_Guides /path/to/project/.claude/prompts/
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
4. Leverage APM prompt templates for complex project management
5. Update rules based on project learnings

### Prompt Templates Usage
- **Manager Setup**: Use `00_Initial_Manager_Setup/` prompts to initialize APM workflows
- **Implementation Planning**: Reference `01_Manager_Agent_Core_Guides/` for structured development
- **Handover Protocols**: Apply `02_Utility_Prompts_And_Format_Definitions/` for agent transitions
- **Memory Management**: Utilize memory bank formats for project continuity

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

*These rules and prompt templates provide a comprehensive foundation for consistent, high-quality development with Claude Code across diverse project types and requirements. The structured APM prompts enable sophisticated project management workflows, while the development rules ensure code quality and best practices.*
