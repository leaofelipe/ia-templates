# Technical Specification Generator

## Input

[Paste the PRD, feature description, or business requirement here]

## Instructions

Generate a complete Technical Specification following this template structure.

### Analysis Process

1. **Problem Understanding**: Clarify what needs to be built and why
2. **Architecture Design**: Define system components and their relationships
3. **Implementation Details**: Specify interfaces, data models, and endpoints
4. **Integration Points**: Identify external services and dependencies
5. **Performance & Security**: Define non-functional requirements
6. **Deployment Plan**: Outline rollout and monitoring strategy

### CRITICAL: Information Gathering

**If you lack information to complete any section:**

1. DO NOT make assumptions or fill with generic placeholders
2. STOP and ask the user specific questions about what's missing
3. List all questions clearly before proceeding
4. Wait for answers before generating the Tech Spec

**Only generate the complete Tech Spec after you have sufficient information.**

### Required Information Checklist

Before generating the Tech Spec, ensure you understand:

- [ ] The feature requirements and business context
- [ ] Target scale and performance requirements
- [ ] External integrations or dependencies needed
- [ ] Security and compliance requirements
- [ ] Technology stack constraints
- [ ] Deployment environment and infrastructure

---

## Output Format

Generate a complete Technical Specification following the structure in `tech-spec-template.md`, including:

- All sections properly filled with specific information
- Architecture decisions justified with trade-offs
- Clear API contracts and data models
- Performance and security considerations
- Testable acceptance criteria
