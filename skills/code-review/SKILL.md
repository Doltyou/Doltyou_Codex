---
name: code-review
description: Use for structured review of code changes before merge, handoff, or approval. Focus on correctness, requirement fit, maintainability, safety, and missing verification.
---

# Code Review

Run a review that is useful to the author, not just descriptive.

## Use this skill when

- reviewing a patch, PR, or changed files
- checking whether work matches requirements
- looking for correctness, maintainability, or safety risks
- validating whether verification is sufficient

## Workflow

1. Understand the intended change.
2. Review behavior and requirement fit first.
3. Review defect risk, edge cases, and safety concerns.
4. Review maintainability and unnecessary complexity.
5. Review verification adequacy.
6. Summarize findings by severity and actionability.

## Review priorities

1. incorrect behavior
2. missing requirement coverage
3. unsafe assumptions or security issues
4. fragile or overcomplicated design
5. missing or weak verification

## Reporting contract

For each issue include:

- severity
- what is wrong
- why it matters
- what change would resolve it

If no issues are found, still report what was checked and any remaining unverified risk.

## References

- For review dimensions and severity guidance, read `references/review-rubric.md`.
