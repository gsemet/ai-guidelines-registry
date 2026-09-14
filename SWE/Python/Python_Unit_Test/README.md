# Python Unit Test Guidelines

Use the normative [guideline](python-unittest.guidelines.md) for Python unit
tests.

## Installation

```console
$ guidelines add gsemet/ai-guidelines-registry SWE/Python/Python_Unit_Test
$ guidelines sync
```

Alternatively, copy `python-unittest.guidelines.md` to the target project's
`.agents/guidelines/` or `.github/guidelines/` directory.

## Scope

The guideline covers pytest function-based tests, the
`pytest-parametrization` library, fixtures, readable formatting, test and
`vectors/` placement, repository-root discovery via `conftest.py`, slow-test
marking, fixture scopes, and coverage validation.
