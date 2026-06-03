# Awesome Claude Code [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome resources, skills, MCP servers, tips, and tools for [Claude Code](https://docs.anthropic.com/en/docs/claude-code) — Anthropic's agentic coding tool.

Claude Code is a command-line tool, desktop app, and IDE extension that lets Claude work directly in your codebase. It understands your project context, makes real code changes, and runs commands — all from natural language.

**This list helps you get the most out of it.**

## Contents

- [Official Resources](#official-resources)
- [Skills](#skills)
- [MCP Servers](#mcp-servers)
- [CLAUDE.md Templates](#claudemd-templates)
- [Hooks](#hooks)
- [Tips & Workflows](#tips--workflows)
- [CLI Tricks](#cli-tricks)
- [Configuration](#configuration)
- [Tutorials & Articles](#tutorials--articles)
- [Videos](#videos)
- [Community](#community)
- [Contributing](#contributing)

## Official Resources

- [Claude Code Docs](https://docs.anthropic.com/en/docs/claude-code) - Official documentation.
- [Claude Code GitHub](https://github.com/anthropics/claude-code) - Official repository for issues and discussions.
- [Claude Code Hooks](https://docs.anthropic.com/en/docs/claude-code/hooks) - Automate actions on tool calls and events.
- [Claude Code IDE Extensions](https://docs.anthropic.com/en/docs/claude-code/ide-integrations) - VS Code and JetBrains plugins.
- [Claude Code SDK](https://docs.anthropic.com/en/docs/claude-code/sdk) - Build custom agents on top of Claude Code.
- [Max Plan](https://www.anthropic.com/pricing) - Unlimited Claude Code usage with Anthropic Max subscription.

## Skills

Skills are reusable prompt-driven capabilities you can install and invoke with `/skill-name`.

### Design & Frontend

- [impeccable](https://github.com/pbakaus/impeccable) - Production-grade frontend design: UX review, visual hierarchy, typography, color, motion, accessibility. 20+ commands including `craft`, `shape`, `critique`, `audit`, `polish`.
- [frontend-design](https://github.com/anthropics/claude-code) - Built-in skill for avoiding AI-slop patterns in UI design. Distinctive typography, no generic templates.
- [web-design-guidelines](https://github.com/anthropics/claude-code) - Built-in web design audit and best practices.
- [shadcn-ui](https://github.com/anthropics/claude-code) - Built-in skill for building with shadcn/ui components.
- [react-components](https://github.com/anthropics/claude-code) - Built-in skill for React component patterns.

### AI-Powered Design Tools

- [stitch-skills](https://github.com/google-labs-code/stitch-skills) - 7 skills for Google Stitch integration: `stitch-design`, `stitch-loop`, `design-md`, `enhance-prompt` and more. Generate UI screens, maintain design systems, and build sites iteratively.

### Video & Motion

- [remotion-skills](https://github.com/remotion-dev/skills) - Skills for building programmatic videos with Remotion. Includes `remotion` and `remotion-best-practices`.

### Workflow & Process

- [brainstorming](https://github.com/anthropics/claude-code) - Built-in structured brainstorming sessions.
- [writing-plans](https://github.com/anthropics/claude-code) - Built-in skill for creating implementation plans.
- [executing-plans](https://github.com/anthropics/claude-code) - Built-in skill for following plans step by step.
- [test-driven-development](https://github.com/anthropics/claude-code) - Built-in TDD workflow.
- [systematic-debugging](https://github.com/anthropics/claude-code) - Built-in structured debugging methodology.
- [subagent-driven-development](https://github.com/anthropics/claude-code) - Built-in skill for parallelizing work across agents.

### Code Quality

- [review](https://github.com/anthropics/claude-code) - Built-in code review skill.
- [security-review](https://github.com/anthropics/claude-code) - Built-in security audit skill.
- [simplify](https://github.com/anthropics/claude-code) - Built-in skill for reducing code complexity.
- [verification-before-completion](https://github.com/anthropics/claude-code) - Built-in skill for double-checking work.

### Deployment

- [deploy-to-vercel](https://github.com/anthropics/claude-code) - Built-in Vercel deployment skill.
- [vercel-react-best-practices](https://github.com/anthropics/claude-code) - Built-in Vercel + React optimization.
- [firebase-auth-basics](https://github.com/anthropics/claude-code) - Built-in Firebase authentication patterns.
- [firebase-firestore-standard](https://github.com/anthropics/claude-code) - Built-in Firestore best practices.
- [firebase-app-hosting-basics](https://github.com/anthropics/claude-code) - Built-in Firebase hosting setup.

### Meta / Skill Management

- [find-skills](https://github.com/anthropics/claude-code) - Built-in skill to discover and search available skills.
- [writing-skills](https://github.com/anthropics/claude-code) - Built-in guide for creating your own skills.
- [init](https://github.com/anthropics/claude-code) - Built-in project initialization skill.

## MCP Servers

MCP (Model Context Protocol) servers extend Claude Code with external tools and data sources.

### Browser & Web

- [Puppeteer MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/puppeteer) - Browser automation: navigate, screenshot, click, fill forms.
- [Chrome DevTools MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/chrome-devtools) - Connect to Chrome for live debugging and visual inspection.
- [Fetch MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/fetch) - HTTP requests with structured response handling.

### Databases

- [PostgreSQL MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/postgres) - Query and manage PostgreSQL databases.
- [SQLite MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/sqlite) - Local SQLite database operations.

### Cloud & APIs

- [Google Drive MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/google-drive) - Read and search Google Drive files.
- [Slack MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/slack) - Send messages and read channels.
- [GitHub MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/github) - Extended GitHub operations beyond the CLI.
- [Linear MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/linear) - Issue tracking integration.
- [Sentry MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/sentry) - Error monitoring integration.

### Design & Media

- [Google Stitch MCP](https://stitch.withgoogle.com/) - AI-powered UI generation from text prompts.
- [Figma MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/figma) - Read Figma designs and extract tokens.

### File & Search

- [Filesystem MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/filesystem) - Extended file operations.
- [Memory MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/memory) - Persistent key-value memory across sessions.
- [Brave Search MCP](https://github.com/anthropics/anthropic-quickstarts/tree/main/mcp-servers/brave-search) - Web search via Brave.

## CLAUDE.md Templates

`CLAUDE.md` files tell Claude about your project. Place them at the repo root.

### Starter Template

```markdown
# Project

## Tech Stack
- [Your stack here]

## Commands
- `npm run dev` — start dev server
- `npm test` — run tests
- `npm run lint` — lint code

## Code Style
- Use TypeScript strict mode
- Prefer named exports
- Write tests for new features

## Architecture
- `src/` — source code
- `src/components/` — React components
- `src/lib/` — utilities and helpers
- `tests/` — test files
```

### Conventions to Include

- Build and test commands (so Claude can run them)
- Code style rules (formatting, naming)
- Architecture overview (folder structure)
- Do's and don'ts specific to your project
- Links to relevant docs

### Tips

- Keep it under 500 lines — Claude reads this on every conversation start.
- Put repo-level rules in root `CLAUDE.md`, folder-specific rules in `src/CLAUDE.md`.
- Use `CLAUDE.local.md` (gitignored) for personal preferences.
- Add your commonly used slash commands and workflows.

## Hooks

Hooks run shell commands automatically when Claude performs specific actions.

### Examples

```json
// .claude/hooks.json
{
  "pre-tool-use": [
    {
      "tool": "Write",
      "command": "echo 'Writing file: $CLAUDE_FILE_PATH'"
    }
  ],
  "post-tool-use": [
    {
      "tool": "Bash",
      "command": "npm run lint --silent 2>/dev/null || true"
    }
  ],
  "post-commit": [
    {
      "command": "npm test --silent"
    }
  ]
}
```

### Use Cases

- Auto-lint after file writes
- Run tests after commits
- Notify Slack when a PR is created
- Auto-format with Prettier on save
- Block commits to main branch

## Tips & Workflows

### Effective Prompting

- **Be specific**: "Add input validation to the signup form email field" beats "improve the form".
- **Reference files**: "In `src/auth/login.ts`, the token refresh logic..." gives Claude immediate context.
- **Use plans for big tasks**: Start with `/plan` or ask Claude to plan before implementing.
- **Iterate, don't restart**: Follow up on Claude's work instead of starting new conversations.

### Power Workflows

- **Parallel agents**: Ask Claude to spawn sub-agents for independent tasks. "Research the API while writing tests in parallel."
- **Git worktrees**: Use `/worktree` to have agents work on isolated branches without conflicts.
- **Background tasks**: Run long builds or tests in background while continuing to work with Claude.
- **Loop mode**: Use `/loop` for repetitive tasks — Claude paces itself and keeps going.

### CLAUDE.md as a Team Tool

- Commit `CLAUDE.md` to your repo — every team member gets the same Claude behavior.
- Add PR review guidelines so Claude reviews consistently.
- Include deployment checklists.

## CLI Tricks

```bash
# Pipe input directly
echo "explain this error" | claude

# Start with a specific prompt
claude "add tests for the auth module"

# Resume last conversation
claude --continue

# Run in non-interactive mode
claude --print "what does this repo do?"

# Use a specific model
claude --model opus

# Add a directory for context
claude --add-dir ../shared-lib

# Run with a system prompt
claude --system-prompt "You are a senior Go developer"
```

## Configuration

### Settings File (~/.claude/settings.json)

```json
{
  "permissions": {
    "allow": [
      "Bash(npm run *)",
      "Bash(git *)",
      "Read",
      "Write",
      "Edit"
    ],
    "deny": [
      "Bash(rm -rf *)",
      "Bash(sudo *)"
    ]
  }
}
```

### Project Settings (.claude/settings.json)

```json
{
  "permissions": {
    "allow": [
      "Bash(npm test)",
      "Bash(npm run lint)",
      "Bash(npm run build)"
    ]
  }
}
```

### Environment Variables

| Variable | Purpose |
|---|---|
| `ANTHROPIC_API_KEY` | API key for direct API access |
| `CLAUDE_CODE_MAX_TOKENS` | Limit response length |
| `DISABLE_PROMPT_CACHING` | Disable prompt caching |

## Tutorials & Articles

- [Claude Code: Best Practices for Agentic Coding](https://docs.anthropic.com/en/docs/claude-code/best-practices) - Official best practices guide.
- [Building with Claude Code SDK](https://docs.anthropic.com/en/docs/claude-code/sdk) - Build custom AI agents.
- [Creating Custom Skills](https://docs.anthropic.com/en/docs/claude-code/skills) - Write your own reusable skills.
- [Configuring MCP Servers](https://docs.anthropic.com/en/docs/claude-code/mcp-servers) - Add external tools.
- [Claude Code Hooks Guide](https://docs.anthropic.com/en/docs/claude-code/hooks) - Automate with hooks.

## Videos

- [Claude Code Introduction](https://www.youtube.com/results?search_query=claude+code+anthropic) - Getting started walkthrough.
- [Claude Code Tips & Tricks](https://www.youtube.com/results?search_query=claude+code+tips+tricks) - Community tips.

## Community

- [Claude Code GitHub Discussions](https://github.com/anthropics/claude-code/discussions) - Official community forum.
- [Anthropic Discord](https://discord.gg/anthropic) - Chat with other Claude Code users.
- [r/ClaudeAI](https://www.reddit.com/r/ClaudeAI/) - Reddit community.
- [X/Twitter #ClaudeCode](https://twitter.com/search?q=%23ClaudeCode) - Follow the conversation.

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

If you find a resource that should be here, open a pull request. Quality over quantity — every item should genuinely help someone be more productive with Claude Code.

---

**Star this repo** if you find it useful. It helps others discover it.

Licensed under [CC0 1.0](LICENSE).
