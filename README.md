# Guidelines

Reusable prompt files define thematic rules and best practices for developers
and coding agents. Copy the selected guidelines into a project, commit them,
and describe in `AGENTS.md` when agents must load them.

## Why guidelines?

See the full rationale explained in the following project:
[gsemet/ai-guidelines](https://github.com/gsemet/ai-guidelines).

TL;DR:
- **why committing guidelines?**
  - guidelines are the 'guardrails' of a project
  - they must be versioned and reviewed like any other code.
  - any undesired update of a guideline may have a significant impact on the project.
  - project owner shall decide when to update them
- **why not skills?**
  - you can, but you will place them all in .agents/skills/
  - they will mix with non-guardrail skills.
  - You do **not** want to use skill auto-activation (the `description` frontmatter)
  - You want your project harness (`AGENTS.md`) to control when to load them.
  - Because the same exact guidelines might be activated on two different scenario on two
    different projects.
- **why not Copilot's `*.instructions.md` ?**
  - Because they are activated by the Coding Agent based on the opened files.

If you choose to use `*.instructions.md` or `SKILL.md` to carry reusable domain-specific rules,
I strongly advise you to use Microsoft Agent Package manager (APM - https://github.com/microsoft/apm).

As a matter of fact, I opened a Feature Requests to support `*.guidelines.md` in APM:
[apm#2525](https://github.com/microsoft/apm/issues/2525).

## Software Engineering

See the [SWE catalog](SWE/README.md) for Git and Python guidelines.

## Usage

Install the guideline manager with uv:

`uv tool install ai-guidelines`

Then inspect available commands:

```bash
guidelines --help
```

Register a guideline collection:

```bash
guidelines add gsemet/ai-guidelines-registry SWE/Git/Git_Commit_Message
```

Update registered guidelines when you choose:

```bash
guidelines update
```
