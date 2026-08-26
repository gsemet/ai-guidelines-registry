# Python Module Documentation Guideline

Use the normative [guideline](python-module-documentation.guidelines.md) for
Python docstrings and external documentation.

## Installation

Copy `python-module-documentation.guidelines.md` to the target project's
`.agents/guidelines/` or `.github/guidelines/` directory.

## Scope

The guideline covers module, function, and class docstrings; type hints;
Google-style sections; runnable examples; version directives; Sphinx/MyST
configuration; admonitions; terminology; line wrapping; and doctest guidance.
> [!WARNING]
> Potential pitfalls or issues.
```

## Key Principles

### 1. Clarity for Users

Documentation should answer:

- **What** does this do?
- **How** do I use it?
- **When** should I use it vs. alternatives?
- **Why** does it work this way?

### 2. Consistency

Similar functions should have similar documentation structure. Users learn patterns they can apply across your API.

### 3. Completeness

Every parameter, return value, and exception should be documented with:

- What the value represents
- What formats are valid
- Edge cases or constraints

### 4. Runnable Examples

Examples in docstrings become part of your test suite. They should be executable with actual imports and function calls—not pseudo-code.

## When to Apply This Guideline

Use this guideline when:

✅ Writing new Python modules or packages
✅ Adding or modifying public APIs
✅ Setting up documentation for a project
✅ Implementing Sphinx-based doc generation

Do not use for:

❌ Private/internal functions (though they still need brief docstrings)
❌ Third-party code you don't maintain
❌ Temporary or experimental code
