# Workflow and principles for implementing code (ACT/Code MODE).

## 💻 Implementation Workflow (ACT/Code MODE)

*   **MODE Selection:** Determine if the current request implies ACT/Code MODE. User can explicitly set `MODE = ACT MODE`.

```mermaid
flowchart TD
    Start[Start] --> Context[Check Memory Files (Core Files always, rest based on context) ]
    Context --> Update[Update Documentation]
    Update --> Rules[Update [lessons-learned.md].md:.cursor/rules/lessons-learned.md), [error-documentation.md].md:.cursor/rules/error-documentation.md) if needed]
    Rules --> Execute[Execute Task]
    Execute --> Document[Document Changes in Memory Files]
```

**<PROGRAMMING PRINCIPLES>**
*   **Efficiency:** Use efficient algorithms and data structures.
*   **Modularity:** Write modular code. Break complex logic into smaller, atomic parts (classes, functions, files, modules).
*   **File Management:** Keep files small (target < 200-300 lines). Refactor larger files. Organize files into directories.
*   **Imports:** Prefer importing functions over modifying files directly.
*   **Reuse:** Reuse existing code where possible.
*   **Design Patterns:** Apply appropriate patterns for maintainability, flexibility, scalability.
*   **Task Focus:** Understand requirements from `tasks/tasks_plan.md` and PRD.
*   **Impact Analysis:** Before significant changes, identify affected components, dependencies, side effects, and plan testing.
*   **Status Updates:** Keep `docs/status.md` and `tasks/tasks_plan.md` updated.

**<SYSTEMATIC CODE PROTOCOL>**

**[Step 1: Analyze Code]**
    *   **<ANALYZE CODE>**
        *   **<DEPENDENCY ANALYSIS>** Identify affected components, dependencies (local vs. core logic), affected functionalities, and cascading effects.
        *   **<FLOW ANALYSIS>** Conduct end-to-end flow analysis for the use case. Track data and logic flow.
        *   Document dependencies thoroughly.
        *   Use Context 7

**[Step 2: Plan Code]**
    *   **<PLAN CODE>**
        *   Use <CLARIFICATION> if needed.
        *   Use <STEP BY STEP REASONING> to outline a detailed plan considering dependencies and architecture.
        *   Use <REASONING PRESENTATION> to explain changes and effects.
        *   **<STRUCTURED PROPOSALS>** Specify: files/lines changed, *why* (bug fix, feature, improvement), direct impacts, potential side effects, trade-offs.
        *   **Interaction Guidance:**
            *   Be clear, specific, and provide context. Reference previous interactions if needed.
            *   Clearly state "Suggestion:" vs. "Applying fix:". Apply directly only with high confidence on well-defined tasks.
            *   Humans: Critically review AI code. Question assumptions.
            *   Focus the AI on specific parts. Avoid broad requests.
            *   Leverage AI for boilerplate, refactoring known patterns, syntax errors, test generation. Maintain human oversight for complex logic, architecture, security.
            *   Use incremental steps for complex tasks.
            *   AI Check-in: Before major suggestions, confirm understanding: "Confirming understanding: I've reviewed [source]. The goal is [goal], adhering to [constraint]. Proceeding with [step]."
            *   Use Context 7
            *   If you're using Python, ALWAYs create and use Python virtual environment. Create virtual environment first and work off this virtual environment
            *   If you're using NodeJS, use npm. Modularity and portability is the key!
            *   Leverage Docker containers as much as you can

**[Step 3: Make Changes]**
    *   **<MAKE CHANGES>**
        *   Document current state (what works, error, affected files) in memory files.
        *   **<INCREMENTAL ROLLOUTS>** Implement one logical change at a time, fully resolving dependencies and issues it creates. Preserve existing architecture.
        *   **<SIMULATION ANALYSIS>** Perform dry runs/trace calls to analyze impact on expected and edge cases. Generate feedback on side effects.
        *   **<SIMULATION VALIDATION>** Do not propose changes unless simulation passes and verifies functionality preservation. Fix simulation breaks before proceeding.
        *   Implement only if simulation passes.
        *   After adding a major feature or completing a milestone, update [project-name].md.
        *   Document the entire database schema in docs/planning/[project-name]-planning.md.
        *   User project folder as current working directory
        *   If chat session is getting too big, do the following:
                ** Update tasks/implemented.md file on phase/tasks that have already been implemented
		** Update tasks/todo.md file on phase/tasks yet to be implemented
                ** Create a detailed summarization of tasks that has been completed and tasks that needs to be implemented and move into a new chat session with descriptive name
        *   If you have updated the file, please say so. Example: "I have updated the file xxxx". If you want me to update it, state it clearly. Example: "Please update the following file xxxx". Also, If you do want me to modify a file because you cannot, print out file fully. I will overwrite it. 
        *   Always implement changes on my behalf. If you cannot change files, you need state so and print out full copy of the edited file so I can overwrite/replace current file. Do not offer partial code, augmentation-in-place. It is always overwrite of the existing file if you cannot change it.
   
**[Step 4: Testing]**
    *   Perform **<TESTING>** (see `testing.md`).

**[Step 5: Loop]**
    *   Repeat steps 1-4 systematically for all changes.

**[Step 6: Optimize]**
    *   Optimize implemented code after all changes are tested and verified.

**[Step 7: Checkpointing]**
    *  Create named and numbered checkpoints after each successful milestone, phase.
    *  Keep a track of each named and numbered checkpoints.
    *  Commit and push out git changes 
    *  Project Git configuration file is always at the root of the project folder. When trying to push out to Git, go the root of the project folder, there you'll find .git.

**[Step 8: Progress-Recording]**
    *  Record remaining implementation phases and steps in [project-name]-todo.md document with not complete marks, such as [ ]
    *  Record successfull implementation phases and steps in [project-name]-implemented.md document, marking tasks as complete [X]
    *  When asking for user input for displayed options, create options like this:
          - Example:
             1. This is first option
                 a) This is sub-option A
                 b) This is sub-option B
          This is all done in order to correct identify which suboption a user can select (i.e., "Option 1a" or "Option 1b")
    *  Record technology stack in [project-name]-technology-stack.md
    *  Record software stack,modules and versions in [project-name]-technology-stack.md
    *  Record current problems and the latest you're working on in file called docs/tasks/update.md 
**<REFERENCE>**
*   Reference relevant documentation and best practices. Use <WEB USE> if needed.
