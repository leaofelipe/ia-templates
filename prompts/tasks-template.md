# Implementation Tasks for [Feature Name]

## Overview

[Brief description of the feature and implementation approach]

**Total Tasks**: X
**Estimated Effort**: Y hours/days
**Critical Path**: Z days

---

## Task Groups

### 1. Foundation

Core infrastructure, data models, and base setup required before other work can begin.

- [ ] 1.0 [Task Title] (S/M/L) - `task-1.0-[name].md`
- [ ] 1.1 [Task Title] (S/M/L) - `task-1.1-[name].md`

### 2. Core Features

Main functionality implementation for the feature.

- [ ] 2.0 [Task Title] (S/M/L) - `task-2.0-[name].md`
- [ ] 2.1 [Task Title] (S/M/L) - `task-2.1-[name].md`
- [ ] 2.2 [Task Title] (S/M/L) - `task-2.2-[name].md`

### 3. Integration

External services, API connections, and system integrations.

- [ ] 3.0 [Task Title] (S/M/L) - `task-3.0-[name].md`
- [ ] 3.1 [Task Title] (S/M/L) - `task-3.1-[name].md`

### 4. Testing

Comprehensive testing coverage for the feature.

- [ ] 4.0 [Task Title] (S/M/L) - `task-4.0-[name].md`
- [ ] 4.1 [Task Title] (S/M/L) - `task-4.1-[name].md`

### 5. Deployment

Configuration, monitoring, documentation, and production readiness.

- [ ] 5.0 [Task Title] (S/M/L) - `task-5.0-[name].md`
- [ ] 5.1 [Task Title] (S/M/L) - `task-5.1-[name].md`

---

## Implementation Order

**Critical Path** (must be done sequentially):

1. Task 1.0 → Task 2.0 → Task 3.0 → Task 4.0 → Task 5.0

**Parallel Work** (can be done simultaneously after dependencies):

- Tasks 2.1 and 2.2 can run in parallel after 2.0
- Tasks 3.1 can run parallel to 2.x tasks if 1.0 is complete

**Dependencies Summary**:

- Group 2 (Core Features) depends on Group 1 (Foundation)
- Group 3 (Integration) depends on relevant Group 2 tasks
- Group 4 (Testing) depends on Groups 2 & 3
- Group 5 (Deployment) depends on all previous groups

---

## Timeline Estimate

**By Size**:

- Small tasks (S): X tasks × 1-3h = Y-Z hours
- Medium tasks (M): X tasks × 1-3d = Y-Z days
- Large tasks (L): X tasks × 3+d = Y+ days

**Total Effort**: ~X hours / Y days
**Critical Path Duration**: Z days (assuming sequential execution of critical tasks)
**Parallelizable Work**: W days can be saved with parallel execution

---

## Risk Items

High-priority risks that could impact delivery:

- [ ] **[Task X.Y]**: [Description of risk and potential delay]
- [ ] **[External Dependency]**: [What we're waiting for and impact]
- [ ] **[Complex Implementation]**: [Area needing research or spike]

---

## Implementation Phases

[Only include this section if feature has >10 tasks]

**Phase 1 - MVP** (Week 1-2):

- Tasks: 1.0, 2.0, 4.0
- Goal: [Basic working version]

**Phase 2 - Enhancement** (Week 3-4):

- Tasks: 2.1, 2.2, 3.0
- Goal: [Full feature set]

**Phase 3 - Production Ready** (Week 5):

- Tasks: 4.1, 5.0, 5.1
- Goal: [Production deployment]

---

## Task File Structure

Each task is documented in a separate file following `task-template.md` structure:

- Location: `./projects/[feature-name]/tasks/task-X.Y-[name].md`
- Contains: Context, requirements, implementation details, acceptance criteria, testing strategy

---

## Size Legend

- **S (Small)**: 1-3 hours, single file/component, no external dependencies
- **M (Medium)**: 1-3 days, multiple files, moderate scope, may have dependencies
- **L (Large)**: 3+ days, cross-cutting changes, multiple integrations, significant complexity

---

## References

- **PRD**: `../prd.md`
- **Tech Spec**: `../techspec.md`
- **Task Template**: Used for all individual task files
