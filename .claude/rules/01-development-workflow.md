# Development Workflow Rules

## 🚀 Core Development Process

### MODE Selection
- **PLAN MODE**: Architecture, planning, requirements analysis
- **ACT MODE**: Implementation, coding, testing
- User can explicitly set `MODE = PLAN MODE` or `MODE = ACT MODE`

### Systematic Development Protocol

#### Phase 1: Analysis & Planning
1. **Requirements Understanding**
   - **<CLARIFICATION>**: Ask for clarifications, identify underspecified requirements
   - Review documentation: PRD, README.md, docs/architecture.md, docs/technical.md
   - **<DECOMPOSE>**: Break problems into smaller sub-problems
   - Use **<STEP BY STEP REASONING>** for solution formulation

2. **Code Analysis**
   - **<ANALYZE CODE>**: Identify affected components, dependencies
   - **<DEPENDENCY ANALYSIS>**: Map local vs core logic dependencies
   - **<FLOW ANALYSIS>**: End-to-end flow analysis for use cases
   - Use Context 7 for comprehensive analysis

#### Phase 2: Implementation
1. **Planning**
   - **<PLAN CODE>**: Detailed plan considering dependencies and architecture
   - **<STRUCTURED PROPOSALS>**: Specify files/lines changed, impacts, trade-offs
   - **<REASONING PRESENTATION>**: Explain changes and effects

2. **Development**
   - **<INCREMENTAL ROLLOUTS>**: One logical change at a time
   - **<SIMULATION ANALYSIS>**: Dry runs to analyze impact
   - **<SIMULATION VALIDATION>**: Verify functionality preservation
   - Preserve existing architecture and patterns

#### Phase 3: Validation & Documentation
1. **Testing** (See testing rules)
2. **Documentation Updates**: Update relevant docs when changes impact architecture
3. **Progress Recording**: Update status files and task plans

### Programming Principles
- **Efficiency**: Use efficient algorithms and data structures
- **Modularity**: Break complex logic into atomic parts
- **File Management**: Keep files < 200-300 lines, organize in directories
- **Reuse**: Leverage existing code and patterns
- **Design Patterns**: Apply appropriate patterns for maintainability

### Technology Guidelines
- **Python**: Always create and use virtual environments
- **NodeJS**: Use npm, focus on modularity and portability
- **Docker**: Leverage containers for consistency
- **Environment**: Use project folder as current working directory

### Checkpointing & Progress
- Create named checkpoints after successful milestones
- Commit and push git changes from project root
- Update implementation tracking files
- Record technology stack and versions
- Document current problems in docs/tasks/update.md

### Architecture Adherence
- Load and parse complete Mermaid diagrams from docs/architecture.md
- Understand module boundaries, relationships, data flow
- Validate changes against architectural constraints
- Maintain separation of concerns
- **Error Handling**: Stop if architecture.md missing, warn on violations

### Quality Standards
- **Code Style**: Follow established conventions, clean code principles
- **DRY Principle**: Don't Repeat Yourself - eliminate code duplication
- **KISS Principle**: Keep It Simple, Stupid - prefer simple solutions
- **Error Handling**: Implement comprehensive error handling
- **Performance**: Consider performance implications of all changes
- **Documentation**: Maintain clear, up-to-date documentation