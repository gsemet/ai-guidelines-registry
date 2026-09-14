# Markdown Line Wrap by Clause

This guidelines will force your agent to write Markdown content
with line breaks inserted at appropriate clause boundaries,
improving readability and maintainability.

## Example

````md
# Release Checklist

Before publishing a release, verify that the change is documented,
the compatibility notes are accurate,
and the validation suite passes on a clean checkout.

## Workflow

1. Review the user-facing changes,
   including new options, changed defaults, and migration notes.
2. Run the focused tests first;
   then run the complete quality gate if the focused checks pass.
3. Inspect the generated artifacts,
   confirm that no credentials or local paths were included,
   and attach the final report to the release.

> Keep each line break at a natural clause boundary,
> rather than splitting a phrase in the middle.

````

This allows to edit a line more easily and avoid complete rewraps
of the paragraph at every minor change
