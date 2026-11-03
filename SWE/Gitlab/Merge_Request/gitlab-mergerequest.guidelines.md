---
name: Pull and Merge Request Guideline
version: 1.0
description: Guidelines for preparing clear, evidence-informed pull requests and merge requests
metadata:
  owner: Gaetan Semet <gaetan.semet@ampere.cars>
  keywords: [pull-requests, merge-requests, reviews, evidence, GitHub, GitLab]
  guideline-id: 7e415334-5550-4397-9ff7-f3615d83f984
---

# Pull and Merge Request Guideline

Use these guidelines when preparing a GitHub pull request or GitLab merge request.
The target project's own contribution rules and applicable request template take precedence.

## Follow the project template

1. Check the target project for its applicable request template and instructions.
   Common locations include `.github/PULL_REQUEST_TEMPLATE.md` for GitHub and
   `.gitlab/merge_request_templates/` for GitLab.
2. Follow the selected project template's structure and instructions.
   Do not replace it with this guideline's fallback template.
3. Add supporting details only where the project's template and rules allow.
   Do not create or change a target-project template just because this guideline is installed.
4. If multiple templates are available and it is unclear which applies, ask which to use.
5. Use the fallback below only when no applicable project template exists.

## Write for reviewers

Explain the change for reviewers and future maintainers who were not part of the implementation.
Describe the problem or motivation, what the change delivers, and what its effects are.
Use clear, user-facing language and explain project-specific terms when needed.
Keep internal task identifiers and implementation-session details out of the main narrative unless
the project asks for them.

## Plan appropriate evidence

While planning the work, consider what evidence will help complete the eventual request and arrange
to collect it during development or at the end.
Choose evidence that suits the change; examples include screenshots or KPI results.
Plan to be able to capture before/after screenshots.
Do not assume every change needs the same evidence.

## Fallback template

When no project template applies, use and adapt this single fallback template.
Keep its sections and order unless they are genuinely irrelevant to the change.

```markdown
## Summary

<!-- Explain the problem or motivation and what this change achieves. -->

## Deliverables

<!-- Describe what the reader receives. Include a small diagram, example, or other supporting
material when it helps explain the change; omit visuals that add no useful context.
When possible, especially for visual changes, display screenshots with before/after,
code using diff-style. -->

## Changes

<!-- Summarize the important changes without reproducing a line-by-line diff. -->

## Impacts

<!-- Explain what affected users or developers will notice.
Include relevant evidence when useful. -->

## Blast radius

<!-- Identify affected areas, notable risks, and rollback considerations. -->

## Test plan

<!-- List checks actually run and their outcomes.
Identify checks still pending or not applicable. -->
```

## Report accurately

Only claim checks or outcomes that are supported by what was actually observed.
State whether checks remain pending or were not run, and explain relevant gaps in evidence.
Do not present missing screenshots, metrics, test results, or pending CI as successful.
