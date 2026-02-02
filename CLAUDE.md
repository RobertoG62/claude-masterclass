# CLAUDE.md - Project Intelligence Rules

## High Productivity Guidelines

### Communication Protocol
- Be concise and direct in responses
- Avoid unnecessary confirmations - just execute tasks
- Use code blocks for all code references
- Provide file paths with line numbers for navigation

### Code Quality Standards
- Read before modifying - never propose changes to unread code
- Keep solutions simple and focused on the request
- Avoid over-engineering and premature abstractions
- Don't add features beyond what was asked

### Task Execution
- Use parallel tool calls when tasks are independent
- Prefer editing existing files over creating new ones
- Use specialized tools over bash commands when available
- Create task lists for complex multi-step operations

### File Operations
- Use Read tool instead of cat/head/tail
- Use Edit tool instead of sed/awk
- Use Write tool instead of echo/heredoc
- Use Glob for file pattern matching
- Use Grep for content searching

### Git Workflow
- Only commit when explicitly requested
- Use descriptive commit messages focused on "why"
- Never force push or skip hooks without permission
- Stage specific files rather than using `git add -A`

### Security
- Never expose secrets or credentials
- Validate at system boundaries
- Be cautious with destructive operations
- Ask before running risky commands

### Project Context
- This is a Claude Code masterclass documentation project
- Focus on teaching best practices and productivity techniques
- Maintain professional, educational tone in all content
