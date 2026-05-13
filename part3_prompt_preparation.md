# PART 3 — Prompt Preparation

## 3.1.1 Repository Context

MetaGPT is a Python-based AI framework that enables multiple AI agents to collaborate like a real software development team. Different agents work together to perform software engineering tasks in a structured and organized manner.

The framework is mainly designed for developers, AI researchers, and organizations exploring AI-driven automation. Instead of relying on a single AI response, MetaGPT follows a workflow-oriented approach to improve output quality and reduce errors.

The repository uses Python, modular components, and asynchronous processing techniques. It supports tasks such as project planning, requirement analysis, coding assistance, and workflow automation.

The main objective of the project is to improve cooperation between AI agents and make AI-based software development more reliable and efficient.

## 3.1.2 Pull Request Description

This pull request introduces functionality that converts repositories into Markdown format.

Before this implementation, repository files and folders were only available in their raw structure, making them difficult to summarize or process efficiently.

The new implementation scans repository contents and generates clean Markdown representations while preserving the original project structure. This makes repositories easier to read, analyze, summarize, and process using AI systems.

The pull request also improves documentation workflows and provides a more structured representation of project files for both developers and automated systems.

## 3.1.3 Acceptance Criteria

- The system should generate valid Markdown output when a correct repository path is provided.
- The generated Markdown should preserve the original folder hierarchy.
- Unsupported or binary files should be skipped safely without crashing the program.
- Invalid repository paths should return meaningful error messages.
- The generated output should remain properly formatted and readable.
- The implementation should handle large repositories efficiently.
- Unit tests should validate repository conversion behavior successfully.

## 3.1.4 Edge Cases

- Empty repositories should still generate valid Markdown output.
- Large repositories with deeply nested folders should be processed correctly.
- Unsupported or binary files should be ignored safely.
- Files with restricted permissions should not crash the program.
- Proper error handling should be displayed for inaccessible files.

## 3.1.5 Initial Prompt

Working on the MetaGPT repository, a Python-based AI framework that enables multiple AI agents to collaborate on software engineering tasks.

Implement functionality that converts supported repository files and directory structures into a clean Markdown format.

The implementation should:

- Recursively scan repository folders
- Read supported files
- Preserve folder hierarchy
- Generate structured Markdown output
- Skip unsupported or binary files safely
- Handle invalid repository paths properly
- Maintain modular and reusable utility functions
- Follow the repository’s existing coding style

### Acceptance Criteria

- Valid repositories should generate proper Markdown output.
- Folder hierarchy should remain preserved.
- Unsupported files should not cause failures.
- Meaningful errors should be displayed for invalid paths.
- Repository conversion behavior should be validated through unit tests.

### Edge Cases

- Empty repositories
- Binary files
- Deeply nested folders
- Permission-related errors

### Testing Requirements

- Include unit tests for repository traversal
- Verify Markdown formatting output
- Test invalid repository handling
- Validate behavior on large repositories
