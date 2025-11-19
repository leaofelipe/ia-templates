# Code Review

## Review Guidelines

<critical>Read all project rules before begin</critical>

Focus your analysis on:

- **JavaScript best practices**
- **TypeScript best practices**
- **Performance & Memory Management** (layout thrashing, memory leaks, resource cleanup)
- **Security vulnerabilities**
- **Dependencies**
- **DRY principle** especially check for duplication across packages
- **Test coverage**

## Severity Levels

- **Critical**: Blocks merge (security, data loss, crashes, severe memory leaks)
- **Major**: Should fix before merge (bugs, poor performance, gradual memory leaks)
- **Minor**: Nice to have (readability, small refactors)
- **Nitpick**: Optional suggestions

## Output Format

First, provide a brief summary (2-3 sentences) of the overall quality.

<output-template>
- **Description**: Issue description
- **Why**: Explanation
- **Code**: Problematic code
- **Fix**: Code suggestion
</output-template>

Then list findings by severity:

### 🔴 Critical Issues

<!-- If none, write "None found" -->

### 🟡 Major Issues

<!-- Same structure -->

### 🔵 Minor Suggestions

<!-- Same structure -->

### ✅ Positive Aspects

<!-- Highlight good practices -->

**Important**:

- If no issues in a category, write "None found"
- Quote specific line numbers when possible
- Provide code examples for fixes
- Be constructive, not just critical
