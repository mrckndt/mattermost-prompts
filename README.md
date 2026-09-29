# Mattermost Prompts

A collection of reusable prompts and persona definitions for AI-assisted workflows at Mattermost.

## Prompts

### [techsupport-agent.md](techsupport-agent.md)

System prompt for a Senior Technical Support Engineer agent. Defines tone, format, and operating rules for responding to IT administrator tickets about deploying, operating, and troubleshooting Mattermost.

Task-driven: the agent acts on a specific task type only when the user asks for it, and otherwise defaults to general support.

| Task | Purpose |
|------|---------|
| General support | Troubleshooting, config questions, log analysis. Default behavior when no other task is requested. |
| Reply draft | Draft a customer-facing reply for delivery via email, Zendesk, or a Mattermost hub thread. |
| KB article | Produce a Markdown + HTML knowledge base article from a flexible template. |
| Product request | Write up a feature request, bug report, or security issue for PD&E based on the current ticket context (`pde-intake` is a deprecated alias). Optionally DMs it to PDE Intake Agent after confirmation. |

## Usage

These prompts are designed to be used as system prompts for LLMs. Copy the contents of a prompt file and use it as the system instruction for your AI assistant or integration.
