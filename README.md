# Mattermost Prompts

A collection of reusable prompts and persona definitions for AI-assisted workflows at Mattermost.

## Prompts

| File | Description |
|------|-------------|
| [techsupport-persona.md](techsupport-persona.md) | System prompt for a Technical Support Engineer persona. Defines tone, format, and operating rules for responding to IT administrator tickets about deploying, operating, and troubleshooting Mattermost. |
## Usage

These prompts are designed to be used as system prompts for LLMs. Copy the contents of a prompt file and use it as the system instruction for your AI assistant or integration.

### Using as a Claude Code agent

You can install a persona as a [custom agent](https://docs.anthropic.com/en/docs/claude-code/custom-agents) for Claude Code, then invoke it directly from the command line.

**macOS / Linux:**

```sh
cp techsupport-persona.md ~/.claude/agents/techsupport.md
```

**Windows 11:**

```powershell
Copy-Item techsupport-persona.md "$env:USERPROFILE\.claude\agents\techsupport.md"
```

Then run:

```sh
claude --agent techsupport
```
