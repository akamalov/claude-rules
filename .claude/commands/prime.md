## READ
@README.md

## Remember
`docs/planning/` - is where useful reference material exists to guide our work which includes planning for our appliation/project
`docs/tasks/` - is where we have outstanding tasks and PRD docs regarding our current application/project

# Project Understanding Prompt

    When starting a new session, follow this systematic approach to understand the project:

    ## 1. Project Overview & Structure
    - **READ** the README.md file in the project's root folder, if available. This provides the user-facing perspective and basic setup instructions.
    - **RUN** `git ls-files` to get a complete file inventory and understand the project structure.
    - **EXAMINE** the project's directory structure to understand the architectural patterns (e.g., `/cmd`, `/internal`, `/pkg` for Go projects).

    ## 2. Core Documentation
    - **READ and UNDERSTAND** the PLANNING.md file for:
      - Project architecture and design decisions
      - Technology stack and dependencies
      - Build, test, and deployment instructions
      - Future considerations and roadmap
    - **READ and UNDERSTAND** the TASK.md file for:
      - Completed work and implementation status
      - Current blockers or known issues
      - Next steps and priorities

    ## 3. Testing & Quality
    - **EXAMINE** test files to understand:
      - Testing patterns and frameworks used
      - Test coverage expectations
      - Integration vs unit test separation
      - Mock implementations and test utilities

    ## 4. Development Workflow
    - **CHECK** for automation files:
      - CI/CD pipelines (.github/workflows, .gitea/workflows)
      - Development environment setup (devenv.nix, .devcontainer)
      - Code quality tools (linting, formatting configurations)

    ## 5. Data & External Systems
    - **IDENTIFY** data models and schemas:
      - Database migrations or schema files
      - API specifications or OpenAPI docs
      - Data transfer objects (DTOs) and validation rules
    - **UNDERSTAND** external service integrations:
      - Authentication providers (Keycloak, Auth0)
      - Databases and connection patterns
      - Third-party APIs and clients

    ## 6. Documentation Maintenance
    - **UPDATE TASK.md** with each substantial change made to the project, including:
      - Features implemented or modified
      - Issues resolved or discovered
      - Dependencies added or updated
      - Configuration changes
    - **UPDATE PLANNING.md** if changes affect:
      - Architecture decisions
      - Technology stack
      - Development workflows
      - Future roadmap items

    ## 7. Knowledge Validation
    Before proceeding with any work, confirm understanding by being able to answer:
    - What is the primary purpose of this project?
    - How do I build, test, and run it locally?
    - What are the main architectural components and their responsibilities?
    - What external systems does it integrate with?
    - What's the current implementation status and what's next?
