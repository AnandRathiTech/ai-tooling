# ai-tooling

A starter template for configuring AI coding assistants (Claude Code) in your projects. Includes a `CLAUDE.md` template with conventions, architectural guidelines, and behavior instructions that Claude Code loads automatically in every session.

## What's Included

- **`CLAUDE.md`** — Project memory file loaded by Claude Code automatically. Covers:
  - Project overview and tech stack
  - Coding conventions and formatting rules
  - Testing and security rules
  - Architectural guidelines
  - Git and workflow rules
  - Claude Code behavior instructions

## Getting Started

1. Copy `CLAUDE.md` into the root of your project.
2. Fill in the placeholder sections with your project's details.
3. Open the project in VS Code with the Claude Code extension — it will pick up `CLAUDE.md` automatically.

## Usage

Claude Code reads `CLAUDE.md` at the start of every session and uses it to:

- Understand your project structure and conventions
- Follow your coding style and architectural patterns
- Avoid known issues and respect domain-specific rules
- Behave according to your workflow preferences

## Customization

Edit `CLAUDE.md` to match your project. The more specific you are, the more consistent Claude's output will be. Key sections to fill in:

- **Project Overview** — what the project does and its tech stack
- **Repository Structure** — where things live so Claude edits the right files
- **Coding Conventions** — style, formatting, error handling preferences
- **Domain Knowledge** — business rules Claude must always follow
- **Known Issues** — quirks or tech debt to avoid touching

## Resources

- [Claude Code Docs](https://docs.anthropic.com/claude/docs/claude-code)
- [Anthropic API](https://www.anthropic.com/api)
