# Guidelines

Reusable prompt files define thematic rules and best practices for developers
and coding agents. Copy the selected guidelines into a project, commit them,
and describe in `AGENTS.md` when agents must load them.

This repository is a **reference guideline registry**: a plain Git repository with a folder
tree, consumed by the [`ai-guidelines`](https://github.com/gsemet/ai-guidelines) tool.

## Documentation

All conceptual and procedural documentation lives in the tool's documentation, which is the
single authoritative source:

| Question | Where |
|---|---|
| Why commit guidelines instead of using skills or `*.instructions.md`? | [Why guidelines](https://ai-guidelines.readthedocs.io/en/stable/explanation/why-guidelines.html) |
| What exactly is a registry, and why does it have no index? | [Registries](https://ai-guidelines.readthedocs.io/en/stable/explanation/registries.html) |
| How do I build a registry like this one? | [Build your own registry](https://ai-guidelines.readthedocs.io/en/stable/tutorials/build-your-own-registry.html) |
| How do I pin a version? | [Pin a version](https://ai-guidelines.readthedocs.io/en/stable/how-to/pin-a-version.html) |
| What source expressions are accepted? | [Source grammar](https://ai-guidelines.readthedocs.io/en/stable/reference/source-grammar.html) |
| How does this compare to Microsoft APM? | [APM comparison](https://ai-guidelines.readthedocs.io/en/stable/explanation/apm-comparison.html) |

## Contents

- [SWE](SWE/README.md): software-engineering guidelines for Git, GitLab, and Python.

## Using these guidelines

```console
$ uv tool install ai-guidelines
$ guidelines add gsemet/ai-guidelines-registry SWE/Git/Git_Commit_Message
$ guidelines sync
```

Update on your own schedule:

```console
$ guidelines outdated
$ guidelines update
```

## Contributing a guideline

Follow the layout and frontmatter rules in
[Build your own registry](https://ai-guidelines.readthedocs.io/en/stable/tutorials/build-your-own-registry.html).
In short: one leaf folder per guideline, exactly two files inside it
(`README.md` + `<kebab-slug>.guidelines.md`), a stable `guideline-id` UUID that never changes,
and a bumped `name` version string on every content change.
