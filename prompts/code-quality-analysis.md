# Code Quality Analysis

Perform a comprehensive code quality assessment of this repository, identifying technical debt, inconsistencies, and improvement opportunities.

## Objective

Generate a technical debt and quality report in Markdown at the repository root, prioritizing findings by impact and effort.

## Analysis Scope

### Architectural Inconsistencies

- Violations of stated architectural patterns
- Mixed or conflicting architectural approaches
- Improper separation of concerns
- Coupling and cohesion issues
- Missing or inadequate abstractions

### Code Smells & Anti-Patterns

- Duplicated code and logic
- God objects/functions
- Inappropriate intimacy between modules
- Feature envy
- Long methods and large classes
- Dead code and unused dependencies

### Code Conventions & Standards

- Inconsistent naming conventions
- Mixed coding styles
- Lack of or inconsistent documentation
- Inconsistent error handling patterns
- Variable code formatting

### Technical Debt

- Legacy code vs modern patterns
- Outdated dependencies and security vulnerabilities
- Hard-coded values and magic numbers
- Missing tests or low coverage areas
- Performance bottlenecks
- Scalability concerns

### Maintainability Issues

- Complex or cryptic code sections
- Lack of modularity
- Tight coupling making changes risky
- Missing or outdated documentation
- Configuration management problems

## Output Format

Organize findings in sections with:

- **Severity**: Critical, High, Medium, Low
- **Effort**: High, Medium, Low
- **Impact**: Performance, Security, Maintainability, Scalability
- Code examples showing the problem
- Suggested refactoring approach
- Mermaid diagrams for architectural improvements when relevant

## Prioritization Matrix

Create a priority matrix considering:

1. Critical security or performance issues (fix immediately)
2. High impact, low effort (quick wins)
3. High impact, high effort (strategic refactoring)
4. Low impact items (backlog)

## Deliverables

- Executive summary with key metrics
- Detailed findings per category
- Prioritized action plan
- Estimated effort for main improvements
