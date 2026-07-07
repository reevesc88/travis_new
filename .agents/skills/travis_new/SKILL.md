```markdown
# travis_new Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development patterns and conventions used in the `travis_new` TypeScript repository. It covers file organization, code style, commit practices, and testing approaches to help contributors maintain consistency and quality in the codebase.

## Coding Conventions

### File Naming
- **Style:** kebab-case
- **Example:**  
  ```
  user-profile.ts
  api-client.ts
  ```

### Import Style
- **Style:** Relative imports
- **Example:**
  ```typescript
  import { fetchData } from './api-client';
  ```

### Export Style
- **Style:** Named exports
- **Example:**
  ```typescript
  // In api-client.ts
  export function fetchData() { ... }
  ```

### Commit Messages
- **Type:** Conventional commits
- **Prefix:** `feat`
- **Example:**
  ```
  feat: add user authentication to login endpoint
  ```

## Workflows

### Feature Development
**Trigger:** When adding a new feature  
**Command:** `/feature-development`

1. Create a new file using kebab-case naming.
2. Write TypeScript code using named exports.
3. Use relative imports for dependencies.
4. Write or update corresponding test files (`*.test.*`).
5. Commit changes with a message starting with `feat:`.
6. Open a pull request for review.

### Testing
**Trigger:** When verifying code functionality  
**Command:** `/run-tests`

1. Identify or create test files matching the `*.test.*` pattern.
2. Run the test suite using the project's test runner (framework unknown; check project scripts).
3. Review test results and fix any failing tests.

## Testing Patterns

- **Test File Pattern:** `*.test.*`
- **Example:**  
  ```
  api-client.test.ts
  ```
- **Framework:** Not explicitly detected; check for scripts or dependencies in the project for details.
- **Approach:** Write tests in separate files using the above pattern, colocated with or near the code under test.

## Commands
| Command              | Purpose                                      |
|----------------------|----------------------------------------------|
| /feature-development | Step-by-step guide for adding new features   |
| /run-tests           | Instructions for running the test suite      |
```
