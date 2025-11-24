# Technical Specification Generator

## Prerequisites

Before starting, ensure:

- PRD exists at `./projects/[feature-name]/prd.md`
- Review project standards in `@.cursor/rules`
- Understand existing codebase architecture

---

## Input

**PRD Location**: `./projects/[feature-name]/prd.md`

[Or paste the PRD content, feature description, or business requirement here if PRD doesn't exist yet]

---

## Instructions

Generate a complete Technical Specification following the `tech-spec-template.md` structure.

### Workflow

Follow this sequence strictly:

1. **Analyze PRD**: Read complete PRD, extract technical requirements
2. **Deep Project Analysis**: Explore codebase, identify affected modules
3. **Technical Clarifications**: Ask questions about missing technical details
4. **Standards Mapping**: Map decisions to `@.cursor/rules`, note deviations
5. **Generate Tech Spec**: Create spec using template structure
6. **Save**: Write to correct location and confirm

### 1. Analyze PRD (Required)

- Read the complete PRD
- Identify misplaced technical content
- Extract core requirements, constraints, success metrics, rollout phases
- Note areas needing technical clarification

### 2. Deep Project Analysis (Required)

Explore the existing codebase to understand:

**Code Structure:**

- Affected files, modules, and interfaces
- Integration points and dependencies
- Existing patterns and architecture

**Technical Landscape:**

- Symbol mapping and critical dependencies
- Configuration management approach
- Middleware and persistence layers
- Concurrency and error handling patterns
- Testing infrastructure
- Deployment and monitoring setup

**Solution Strategies:**

- Existing libraries vs custom development
- Reusable components and interfaces
- Risks and alternatives
- Performance and scalability considerations

**Use Context7 MCP** to access documentation for languages, frameworks, and libraries when needed.

### 3. Technical Clarifications (Required)

**CRITICAL: If you lack information, STOP and ask questions before proceeding.**

Ask focused questions about:

**Domain & Architecture:**

- Module boundaries and ownership
- Where does this feature belong in the architecture?
- Which existing components can be reused?

**Data Flow:**

- Input/output contracts and transformations
- State management approach
- Data persistence strategy

**Dependencies:**

- External services/APIs required
- Failure modes and timeouts
- Idempotency requirements
- Authentication/authorization needs

**Implementation:**

- Core logic location
- Main interfaces and data models
- Integration with existing systems

**Testing:**

- Critical paths to test
- Unit vs integration test boundaries
- Contract testing needs

**Reuse vs Build:**

- Available libraries/components
- License compatibility
- API stability and maintenance

### 4. Standards Mapping (Required)

- Review `@.cursor/rules` for project standards
- Map architectural decisions to these standards
- Highlight any deviations with:
  - Clear justification
  - Conforming alternatives considered
  - Trade-offs analysis

### 5. Generate Tech Spec (Required)

Use `tech-spec-template.md` as exact structure.

**Include:**

- Architecture overview and component design
- Interfaces, data models, and API endpoints
- Integration points and external dependencies
- Performance requirements and scalability approach
- Security considerations
- Error handling strategy
- Testing approach (unit, integration, e2e)
- Deployment strategy and rollback plan
- Monitoring and observability
- Technical decisions with justifications
- Known risks and mitigation

**Keep concise**: ~2,000 words target
**Focus on HOW**: Avoid repeating PRD's functional requirements

### 6. Save Tech Spec (Required)

**Save Location**: `./projects/[feature-name]/techspec.md`

Confirm write operation and provide full path.

---

## Required Information Checklist

Before generating the Tech Spec, ensure you understand:

- [ ] Feature requirements and business context (from PRD)
- [ ] Existing codebase structure and patterns
- [ ] Module boundaries and ownership
- [ ] Data flow and transformations
- [ ] External integrations and dependencies
- [ ] Performance and scale requirements
- [ ] Security and compliance requirements
- [ ] Technology stack and constraints
- [ ] Deployment environment and infrastructure
- [ ] Testing strategy
- [ ] Monitoring and observability approach

---

## Core Principles

- **Tech Spec focuses on HOW**, not WHAT (PRD has the what/why)
- **Prefer simple, evolutionary architecture** with clear interfaces
- **Provide testability and observability** considerations upfront
- **Reuse before build**: Evaluate existing libraries and components
- **Follow project standards**: Align with `@.cursor/rules`
- **Document trade-offs**: Justify decisions with alternatives considered

---

## Output Format

Generate a complete Technical Specification following `tech-spec-template.md`, including all sections properly filled.

### Final Response Should Include

1. **Summary**: Overview of technical decisions and approach
2. **Tech Spec Content**: Complete specification in Markdown
3. **File Path**: Confirm where spec was saved
4. **Standards Compliance**: Note any deviations from `@.cursor/rules`
5. **Open Questions**: Technical items needing stakeholder decisions
6. **Next Steps**: Recommend creating Implementation Tasks using `tasks-generator.md`

---

## Quality Checklist

- [ ] PRD reviewed and technical requirements extracted
- [ ] Deep codebase analysis completed
- [ ] Technical clarifications answered
- [ ] Standards compliance verified against `@.cursor/rules`
- [ ] Tech Spec generated using template structure
- [ ] Architecture decisions justified with trade-offs
- [ ] Performance and security addressed
- [ ] Testing strategy defined
- [ ] Deployment and rollback plan included
- [ ] File saved to `./projects/[feature-name]/techspec.md`
- [ ] File path confirmed
