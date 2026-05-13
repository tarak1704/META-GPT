# Part 3 — Prompt Preparation

# Selected PR:
PR #1061 — Repo to Markdown

## 3.1.1 Repository Context

MetaGPT is a Python-based framework that allows multiple AI agents to work together like a real software development team. Each AI agent is assigned a role such as project manager, software engineer, or architect. These agents collaborate with each other to complete software-related tasks in a more organized way.

The project is mainly designed for developers, AI researchers, and organizations exploring AI-driven automation. Instead of relying on a single AI response, MetaGPT follows structured workflows to improve output quality and reduce errors.

The repository uses Python along with asynchronous workflows and modular components. It supports tasks such as project planning, requirement analysis, coding assistance, and workflow automation. The overall goal of the project is to improve collaboration between AI agents and make AI-based software development more reliable and efficient.

## 3.1.2 Pull Request Description

This pull request introduces a feature that converts repositories into Markdown format. Before this change, repository files and folders existed only in their raw structure, making them difficult to process or summarize efficiently.

The new implementation scans repository contents and generates a clean Markdown representation of the project structure and file contents. This makes repositories easier to read, summarize, and analyze. It also improves compatibility with AI systems because Markdown is easier for language models to process compared to raw directory structures.

The PR improves documentation workflows and helps AI agents better understand repository information. It also creates a more organized and consistent representation of project files, making repository analysis simpler for developers and automated systems.

## 3.1.3 Acceptance Criteria

✓ When a valid repository path is given, the system should generate a proper Markdown document.

✓ The generated Markdown should maintain the original folder hierarchy.

✓ Unsupported or binary files should be skipped safely without crashing the program.

✓ Invalid repository paths should return meaningful error messages.

✓ The generated output should remain clean and properly formatted.

✓ The implementation should handle large repositories without major failures.

✓ Unit tests should successfully validate repository conversion behavior.

## 3.1.4 Edge Cases

1. Empty repositories should still generate a valid Markdown structure without errors.

2. Large repositories with deeply nested folders should be processed correctly.

3. Unsupported or binary files should be ignored safely.

4. Files with restricted permissions should not crash the program and should display proper error handling.

## 3.1.5 Initial Prompt

You are working on the MetaGPT repository, a Python-based AI framework where multiple AI agents collaborate to perform software engineering tasks.

Your task is to implement functionality that converts repository structures and supported source files into a clean Markdown format. The implementation should recursively scan folders, read valid files, and generate structured Markdown output that preserves the repository hierarchy.

The generated Markdown should be readable, well-structured, and properly separated into sections. Unsupported or binary file types should be skipped safely without interrupting the process. Proper error handling should also be implemented for invalid repository paths or inaccessible files.

The implementation should follow the existing coding style of the project and keep the utility functions modular and reusable. The system should also be capable of handling large repositories with deeply nested directories.

Acceptance criteria:
- Valid repositories should generate proper Markdown output.
- Folder hierarchy should be preserved.
- Unsupported files should not cause failures.
- Invalid paths should display meaningful errors.
- Unit tests should validate repository conversion functionality.

Edge cases:
- Empty repositories
- Binary files
- Deeply nested folders
- Permission-related errors

Testing requirements:
- Add unit tests for repository traversal.
- Validate Markdown formatting output.
- Test invalid repository handling.
- Verify behavior on large repositories.

## Integrity Declaration

"I declare that all written content in this assessment is my own work, created without the use of AI language models or automated writing tools. All technical analysis and documentation reflects my personal understanding and has been written in my own words."
