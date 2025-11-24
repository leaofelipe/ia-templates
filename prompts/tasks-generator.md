# Implementation Tasks Generator

## Input

[Paste the Technical Specification or provide the feature description]

## Instructions

Generate a detailed, actionable task breakdown for implementation based on the provided Tech Spec.

### CRITICAL: Information Gathering

**If you lack information to complete any section:**

1. DO NOT make assumptions or fill with generic placeholders
2. STOP and ask the user specific questions about what's missing
3. List all questions clearly before proceeding
4. Wait for answers before generating the tasks

**Only generate the complete task breakdown after you have sufficient information.**

### Required Information Checklist

Before generating tasks, ensure you understand:

- [ ] The technical specification and architecture decisions
- [ ] Development team capacity and experience level
- [ ] Dependencies between components and external services
- [ ] Testing and quality requirements
- [ ] Deployment and rollback procedures
- [ ] Priority and timeline constraints

---

### Task Structure

Each task should follow the structure in `task-template.md` and include:

- Clear, actionable title
- Size estimate (S/M/L) with criteria
- Dependencies (blocks/blocked by)
- Acceptance criteria
- Technical notes if relevant

### Sizing Criteria

- **S (Small)**: 1-3 hours, single file/component, no external dependencies
- **M (Medium)**: 1-3 days, multiple files, moderate scope, may have dependencies
- **L (Large)**: 3+ days, cross-cutting changes, multiple integrations, significant complexity

### Grouping

Group tasks by:

1. **Foundation** - Core infrastructure, data models, base setup
2. **Core Features** - Main functionality implementation
3. **Integration** - External services, API connections
4. **Testing** - Unit, integration, e2e tests
5. **Deployment** - Configuration, monitoring, documentation

---

## Output Format

Generate individual task files following `task-template.md` structure:

- One markdown file per task: `task-X.Y-[descriptive-name].md`
- Each file must use the complete structure from `task-template.md`
- Tasks should be numbered sequentially (1.0, 1.1, 2.0, 2.1, etc)

---

## Summary: Implementation Tasks for [Feature Name]

### 1. Foundation

- [ ] 1.1 [Task title] (S/M/L) - `task-1.1-[name].md`
- [ ] 1.2 [Task title] (S/M/L) - `task-1.2-[name].md`

### 2. Core Features

- [ ] 2.1 [Task title] (S/M/L) - `task-2.1-[name].md`
- [ ] 2.2 [Task title] (S/M/L) - `task-2.2-[name].md`

### 3. Integration

- [ ] 3.1 [Task title] (S/M/L) - `task-3.1-[name].md`

### 4. Testing

- [ ] 4.1 [Task title] (S/M/L) - `task-4.1-[name].md`

### 5. Deployment

- [ ] 5.1 [Task title] (S/M/L) - `task-5.1-[name].md`

---

## Implementation Order

1. [Task IDs in recommended order with reasoning]
2. [Explain critical path and parallelization opportunities]

## Estimated Timeline

- Total tasks: X
- Estimated effort: Y hours/days
- Critical path duration: Z days
- Parallelizable work: W days

## Risk Items

- [ ] [Task or dependency that could cause delays]
- [ ] [Complex task needing research]
- [ ] [External dependency out of our control]

---

## Task Files

For each task listed above, generate a separate markdown file using `task-template.md` structure with all sections properly filled.
