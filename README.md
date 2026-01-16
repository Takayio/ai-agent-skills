# AI Agent Skills

This repository contains a collection of specialized "skills" for AI agents. Each skill is designed to handle specific tasks with expert-level proficiency, following strict protocols and guidelines.

## How to Use on  AI Agent

To use a skill, an AI agent should:

Workspace skills
```
cd <workspace-root>/.agent/
git clone https://github.com/your-username/ai-agent-skills.git
rm -rf skills/.git
```

Global skills
```
cd ~/.gemini/antigravity/
git clone https://github.com/your-username/ai-agent-skills.git
rm -rf skills/.git
```

## Available Skills

### 1. Git Commit Guardian (`git-commit-guardian`)

**Description:** Generates Git commit messages that strictly follow the [Conventional Commits](https://www.conventionalcommits.org/) specification.
**Key Features:**

- Enforces `<type>(<scope>): <description>` format.
- Supports types: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `chore`.
- Ensures descriptions are concise (under 50 chars), imperative, and in Traditional Chinese (繁體中文).

### 2. Harsh Code Reviewer (`harsh-code-reviewer`)

**Description:** Acts as a strict, senior Technical Lead for code reviews. Focuses on security, performance, and readability with a direct, no-nonsense style.
**Key Features:**

- **Security Checks:** SQL Injection, XSS, hardcoded secrets.
- **Performance Checks:** Unnecessary loops, re-renders, memory leaks.
- **Readability & Type Safety:** Variable naming, function length, `any` usage.
- **Output:** Markdown table of issues and a strict 0-100 score.

### 3. Unit Test Architect (`unit-test-architect`)

**Description:** Generates comprehensive unit tests for existing code, ensuring robust coverage including edge cases.
**Key Features:**

- **Frameworks:** Jest + React Testing Library (JS/TS), Pytest (Python).
- **Structure:** Follows the AAA (Arrange-Act-Assert) pattern.
- **Coverage:** Mandatory checks for Edge Cases (null, undefined, negative numbers, etc.) and Error Handling.
