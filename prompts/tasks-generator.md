# Implementation Tasks Generator

## Prerequisites

Before starting, ensure these files exist:

- **PRD**: `./projects/[feature-name]/prd.md`
- **Tech Spec**: `./projects/[feature-name]/techspec.md`

---

## Input

**Tech Spec Location**: `./projects/[feature-name]/techspec.md`

[Or paste the Technical Specification content here if not yet saved]

---

## Instructions

Generate a detailed, actionable task breakdown for implementation based on PRD and Tech Spec.

**Target Audience**: Assume the reader is a junior developer who needs clear guidance.

### Workflow

Follow this sequence strictly:

1. **Analyze Documents**: Read PRD and Tech Spec, extract requirements and technical decisions
2. **Generate High-Level Structure**: Create task list with grouping and sequencing
3. **Get Approval**: **CRITICAL - Show high-level task list and wait for user approval before generating files**
4. **Generate Individual Tasks**: Create detailed task files using template
5. **Save Files**: Write all files to correct locations
6. **Report**: Provide summary and next steps

### CRITICAL: Approval Required

**Before generating any task files:**

1. Present complete high-level task breakdown
2. Show grouping, dependencies, and timeline
3. Wait for user approval
4. Only proceed after explicit approval

### 1. Analyze Documents (Required)

Read and extract:

- Requirements from PRD
- Technical decisions from Tech Spec
- Main components and their relationships
- Dependencies and integrations
- Testing requirements
- Deployment considerations

### 2. Generate Task Structure (Required)

**Grouping Guidelines:**

- Group by domain (e.g., agent, tool, flow, infra)
- Order logically: dependencies before dependents
- Make each main task independently completable
- Include testing as subtasks within each main task
- Define clear scope and deliverables

**Task Categories:**

1. **Foundation** - Core infrastructure, data models, base setup
2. **Core Features** - Main functionality implementation
3. **Integration** - External services, API connections
4. **Testing** - Unit, integration, e2e tests
5. **Deployment** - Configuration, monitoring, documentation

**For Large Features (>10 main tasks):**

- Suggest breaking into implementation phases
- Define MVP and subsequent phases
- Mark optional/future enhancements

### 3. Get User Approval (Required)

Present high-level breakdown including:

- All main tasks with sizing
- Grouping and dependencies
- Critical path and parallelization opportunities
- Estimated timeline
- Implementation phases (if applicable)

**Wait for explicit approval before proceeding.**

### 4. Generate Individual Tasks (Required)

For each task, create a separate file using `task-template.md` structure.

**Task Structure:**
Each task must include:

- Clear, actionable title
- Size estimate (S/M/L)
- Dependencies (blocks/blocked by)
- Acceptance criteria (functional, quality, technical)
- Prerequisites (what to read first)
- Implementation details
- Testing strategy
- References

**Sizing Criteria:**

- **S (Small)**: 1-3 hours, single file/component, no external dependencies
- **M (Medium)**: 1-3 days, multiple files, moderate scope, may have dependencies
- **L (Large)**: 3+ days, cross-cutting changes, multiple integrations, significant complexity

**Numbering Format:**

- X.0 for main tasks (1.0, 2.0, 3.0)
- X.Y for subtasks (1.1, 1.2, 2.1, 2.2)

### 5. Save Files (Required)

**Directory Structure:**

```
./projects/[feature-name]/
├── prd.md
├── techspec.md
├── tasks/
│   ├── tasks.md              (summary - generate this)
│   ├── task-1.0-[name].md    (individual tasks)
│   ├── task-1.1-[name].md
│   ├── task-2.0-[name].md
│   └── ...
```

**Files to Generate:**

1. **Summary**: `./projects/[feature-name]/tasks/tasks.md` using `tasks-template.md`
2. **Individual Tasks**: `./projects/[feature-name]/tasks/task-X.Y-[name].md` using `task-template.md`

---

## Required Information Checklist

Before generating tasks, ensure you understand:

- [ ] Technical specification and architecture decisions
- [ ] Main components and their responsibilities
- [ ] Dependencies between components
- [ ] External service integrations
- [ ] Testing strategy and quality requirements
- [ ] Deployment and rollback procedures
- [ ] Development team capacity and experience level
- [ ] Priority and timeline constraints

---

## Task Creation Guidelines

**Make Tasks:**

- **Independently completable**: Each can be done without waiting for others (except explicit dependencies)
- **Clearly scoped**: Specific deliverables and acceptance criteria
- **Appropriately sized**: Break large tasks into smaller ones
- **Well-ordered**: Dependencies before dependents
- **Testable**: Include testing as part of the task

**Indicate:**

- Dependencies clearly (blocks/blocked by)
- Tasks that can run in parallel
- Critical path items
- Risks and blockers

---

## Output Format

### Summary File (tasks.md)

Follow `tasks-template.md` structure exactly, including:

- Grouped task list with checkboxes
- Size estimates for each task
- Implementation order and dependencies
- Estimated timeline with critical path
- Risk items
- Implementation phases (if feature is large)

### Individual Task Files (task-X.Y-[name].md)

Follow `task-template.md` structure exactly, including:

- Status, size, assignment
- Context (domain, type, complexity)
- Overview and prerequisites
- Requirements and subtasks
- Implementation details with file references
- Acceptance criteria (functional, quality, technical)
- Testing strategy
- Notes and references

---

## Final Response Should Include

1. **High-Level Summary**: Task breakdown awaiting approval
2. **After Approval**:
   - Confirmation that all files were generated
   - File paths for tasks.md and all task files
   - Summary of task distribution and timeline
   - Next steps: ready for implementation using Cursor Plan mode

---

## Quality Checklist

- [ ] PRD and Tech Spec reviewed
- [ ] High-level task structure created
- [ ] User approval obtained
- [ ] Summary file generated using `tasks-template.md`
- [ ] Individual task files generated using `task-template.md`
- [ ] All files saved to `./projects/[feature-name]/tasks/`
- [ ] Dependencies clearly marked
- [ ] Critical path identified
- [ ] Parallel work opportunities noted
- [ ] Timeline estimated
- [ ] File paths confirmed

---

## Core Principles

- **Junior-developer friendly**: Write for someone with less experience
- **Clear dependencies**: Make execution order obvious
- **Independent tasks**: Minimize blocking dependencies
- **Testability built-in**: Testing is part of each task, not separate
- **Phased approach**: For large features, suggest implementation phases
- **Approval-driven**: Don't generate files without user approval
