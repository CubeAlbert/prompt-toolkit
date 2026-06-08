# Prompt Toolkit

A personal collection of reusable AI/LLM prompt templates for software engineering workflows.

## Structure

All prompts live as Markdown files at the repository root, following the naming convention:

```
[Type]-[Software/LLM/Agent Name]-[Usage].md
```

### Components

| Field | Description | Example |
|-------|-------------|---------|
| **Type** | The kind of prompt | `agent`, `system`, `user`, `tool` |
| **Software/Agent Name** | Target tool or LLM | `kilo`, `claude`, `cursor`, `copilot` |
| **Usage** | The specific task it addresses | `commit-message`, `code-review`, `refactor` |

### Example

`agent-kilo-commit-message.md` — an AI agent prompt for generating Conventional Commits messages from `git diff` output.

## Usage

Prompt files may contain `{{variable}}` placeholders that are substituted at invocation time. Load the appropriate prompt and inject your context into the placeholders before sending to the LLM.

## License

MIT — see [LICENSE](LICENSE).
