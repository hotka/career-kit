---
name: create-skill
description: Create new Agent Skills (SKILL.md files). Use when asked to create, write, or add a new skill for Claude Code, OpenCode, or other skills-compatible agents.
license: MIT
compatibility: Claude Code, OpenCode, Cursor, and other skills-compatible agents
metadata:
  author: mjp
  version: "1.0"
  spec-url: https://agentskills.io/specification
---

# Creating Agent Skills

Agent Skills are a portable, open format for giving AI agents specialized knowledge and capabilities.

## Directory Structure

A skill is a folder containing at minimum a `SKILL.md` file:

```
skill-name/
├── SKILL.md          # Required: instructions + metadata
├── scripts/          # Optional: executable code
├── references/       # Optional: detailed documentation
└── assets/           # Optional: templates, resources
```

## Skill Locations

| Scope | Path | Notes |
|-------|------|-------|
| Global (user) | `~/.agents/skills/<name>/SKILL.md` | Via `npx skills add -g` or `npx skills init` |
| Global (Claude) | `~/.claude/skills/<name>/SKILL.md` | Symlinked to ~/.agents/skills |
| Project | `.claude/skills/<name>/SKILL.md` | Committed with repo |

Project skills take precedence over global skills with the same name.

**Note**: OpenCode also supports `~/.config/opencode/skills/` and `.opencode/skills/` paths.

## SKILL.md Format

Every skill must have YAML frontmatter followed by Markdown content:

```yaml
---
name: skill-name
description: What this skill does and when to use it.
license: MIT                        # Optional
compatibility: Claude Code          # Optional
metadata:                           # Optional
  author: example
  version: "1.0"
---

# Markdown instructions here
```

## Required Fields

### `name`
- 1-64 characters
- Lowercase alphanumeric and hyphens only (`a-z`, `0-9`, `-`)
- Must not start or end with `-`
- Must not contain consecutive hyphens (`--`)
- **Must match the parent directory name**

Valid: `pdf-processing`, `code-review`, `git-workflow`
Invalid: `PDF-Processing`, `-pdf`, `pdf--processing`

### `description`
- 1-1024 characters
- Describe both **what** the skill does and **when** to use it
- Include keywords that help agents identify relevant tasks

Good:
```yaml
description: Extract text and tables from PDF files, fill PDF forms, and merge multiple PDFs. Use when working with PDF documents.
```

Bad:
```yaml
description: Helps with PDFs.
```

## Optional Fields

| Field | Purpose | Max Length |
|-------|---------|------------|
| `license` | License name or file reference | - |
| `compatibility` | Environment requirements (tools needed, etc.) | 500 chars |
| `metadata` | Arbitrary key-value pairs (author, version, etc.) | - |
| `allowed-tools` | Space-delimited pre-approved tools (experimental) | - |

## Body Content Guidelines

The Markdown body contains instructions for the agent. Recommended sections:

1. **Overview** - What this skill accomplishes
2. **When to use** - Specific triggers or scenarios
3. **Step-by-step instructions** - How to perform the task
4. **Examples** - Input/output samples
5. **Edge cases** - Common issues and how to handle them

### Length Guidelines

- Keep main `SKILL.md` under 500 lines (~5000 tokens)
- Move detailed reference material to `references/` directory
- Agents load skills on-demand, so smaller = faster activation

## Progressive Disclosure

Skills are designed for efficient context usage:

1. **Startup**: Only `name` + `description` loaded (~100 tokens per skill)
2. **Activation**: Full `SKILL.md` loaded when skill is selected
3. **Execution**: Scripts/references loaded only when needed

## File References

When referencing other files, use relative paths from the skill root:

```markdown
See [detailed reference](references/REFERENCE.md) for more.

Run the helper script:
scripts/helper.py
```

## Creating a New Skill

Use the skills CLI to scaffold new skills:

### Global Skill (available in all projects)

```bash
cd ~/.agents/skills
npx skills init my-skill
# Edit my-skill/SKILL.md with your instructions
```

### Project Skill (available in current project only)

```bash
cd /path/to/project
mkdir -p .claude/skills
cd .claude/skills
npx skills init my-skill
# Edit my-skill/SKILL.md with your instructions
# Commit to version control
```

### Verify the Skill

After creating, the skill should appear in the agent's available skills list. Test by asking the agent to use it.

## Example: Complete Skill

```yaml
---
name: conventional-commits
description: Create conventional commit messages following the Conventional Commits specification. Use when committing code or asked about commit message format.
license: MIT
metadata:
  author: mjp
  version: "1.0"
---

# Conventional Commits

## Format
```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

## Types
| Type | When to use |
|------|-------------|
| feat | New feature |
| fix | Bug fix |
| docs | Documentation only |
| style | Formatting, no code change |
| refactor | Code change that neither fixes nor adds |
| test | Adding or updating tests |
| chore | Maintenance tasks |

## Rules
- Use present tense ("Add feature" not "Added feature")
- Keep subject line under 72 characters
- Capitalize the description
- No period at the end of subject line

## Examples
- `feat(auth): add OAuth2 login support`
- `fix(api): handle null response from server`
- `docs: update installation instructions`
```

## Managing Skills with the CLI

### Installing Skills from Repositories

```bash
# Install globally (user-level)
npx skills add owner/repo@skill-name -g -y

# Install to current project
npx skills add owner/repo@skill-name -y

# Search for skills
npx skills find <query>
```

### Updating Skills

```bash
# Check for updates
npx skills check

# Update all installed skills
npx skills update
```

### Removing Skills

```bash
# Remove the skill directory
rm -rf ~/.agents/skills/skill-name        # global
rm -rf .claude/skills/skill-name          # project

# Regenerate lock file
npx skills generate-lock
```

### Lock File

The `.skill-lock.json` file tracks installed skills for updates:
- Located in `~/.agents/` for global skills
- Located in `.claude/` for project skills
- Only tracks skills installed via `npx skills add`
- Custom skills created with `npx skills init` are not tracked

## Validation

Use the official reference library to validate skills:

```bash
npx skills-ref validate ./my-skill
```

## Resources

- Skills Directory: https://skills.sh
- Specification: https://agentskills.io/specification
- Example skills: https://github.com/anthropics/skills
- Reference library: https://github.com/agentskills/agentskills/tree/main/skills-ref
