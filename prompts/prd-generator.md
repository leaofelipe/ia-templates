# PRD Generator

## Input Problem/Opportunity

[Paste or describe the problem, feature request, or opportunity here]

---

## Instructions

Given a product problem or opportunity, generate a complete PRD following the PRD_TEMPLATE structure.

### Workflow

Follow this sequence strictly:

1. **Clarify**: Ask questions to gather missing information (see checklist below)
2. **Plan**: Present section-by-section approach and wait for user approval
3. **Generate**: Create complete PRD using `prd-template.md` structure
4. **Save**: Create directory and save file to correct location
5. **Report**: Provide summary, file path, and next steps

### Analysis Process

1. **Problem Analysis**: Clarify the core problem and its business impact
2. **User Context**: Identify affected users, their needs, and pain points
3. **Solution Design**: Define features that address the problem
4. **Success Definition**: Establish measurable business outcomes
5. **Scope Management**: Determine clear boundaries of what's included/excluded

### CRITICAL: Information Gathering

**If you lack information to complete any section:**

1. DO NOT make assumptions or fill with generic placeholders
2. STOP and ask the user specific questions about what's missing
3. List all questions clearly before proceeding
4. Wait for answers before generating the PRD

**Only generate the complete PRD after you have sufficient information.**

### Required Information Checklist

Before generating the PRD, ensure you understand:

- [ ] The problem being solved and who experiences it
- [ ] Business goals and how success will be measured
- [ ] Target users and their characteristics
- [ ] Core features needed to solve the problem
- [ ] Technical constraints or integrations required
- [ ] What is explicitly out of scope

### Clarification Question Categories

When gathering information, ask about:

- **Problem & Goals**: What problem are we solving? What's the business impact?
- **Users**: Who are the primary users? What are their pain points?
- **Features**: What are the must-have capabilities? What actions can users take?
- **Success Metrics**: How do we measure if this succeeds?
- **Constraints**: Any technical, timeline, or budget limitations?
- **Scope**: What is explicitly NOT included in this version?

---

## File Structure

Create the following structure:

```
./projects/[feature-name]/     (use kebab-case)
├── prd.md                      (generate this now)
├── techspec.md                 (next step)
└── tasks/                      (after tech spec)
```

**Save Location**: `./projects/[feature-name]/prd.md`

## Output Format

Generate a complete PRD following the structure in `prd-template.md`, including:

- All sections properly filled with specific information
- User stories that reflect real user needs
- Features with clear business value
- Measurable success metrics
- Technical constraints at high level only
- Explicit non-goals
- Open questions for items needing clarification

### Final Response Should Include

1. **Summary**: Brief overview of the PRD created
2. **PRD Content**: Complete PRD in Markdown
3. **File Path**: Confirm where file was saved
4. **Open Questions**: Any items still needing stakeholder input
5. **Next Steps**: Recommend creating Tech Spec using `tech-spec-generator.md`
