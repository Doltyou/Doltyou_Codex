# Upstream PR Summary: skill doc portability wording sweep

## Summary

- normalize legacy slash-style skill invocation wording to the current `$skill-name` convention across the active skill catalog
- remove targeted stale runtime/tool references from source skill docs (`AskUserQuestion`, `ToolSearch(`, `ask_codex`, `mcp__x__ask_codex`, bare `learner`)
- align the package source skill docs with the already-corrected installed copies so future `omx setup` runs inherit the cleaned content

## Why

- the installed skill copies and the package source had drifted
- several source docs still described old invocation styles or unavailable tool surfaces
- these wording mismatches create confusion during setup/refresh and make docs less portable across runtimes

## Scope

- doc-only changes in `skills/*/SKILL.md`
- no runtime code changes
- no skill names, triggers, or install paths changed

## Verification

- source catalog search for legacy slash-style invocation patterns: **0 matches**
- source catalog search for stale tool/reference patterns (`AskUserQuestion`, `ToolSearch(`, `ask_codex`, `mcp__x__ask_codex`, bare `learner`): **0 matches**
- `omx setup --scope user` completed successfully after the sweep
- active installed/source hashes match for the synchronized active skills (`ask-claude`, `ask-gemini`, `autopilot`, `cancel`, `code-review`, `configure-notifications`, `deep-interview`, `help`, `note`, `plan`, `ralph`, `ralplan`, `security-review`, `skill`, `web-clone`)

## Non-goals

- broad stylistic rewriting beyond the targeted portability/drift fixes
- semantic workflow redesign
- runtime or tmux implementation changes

## Changed files

- `skills/ask-claude/SKILL.md`
- `skills/ask-gemini/SKILL.md`
- `skills/analyze/SKILL.md`
- `skills/autopilot/SKILL.md`
- `skills/build-fix/SKILL.md`
- `skills/cancel/SKILL.md`
- `skills/code-review/SKILL.md`
- `skills/configure-notifications/SKILL.md`
- `skills/deep-interview/SKILL.md`
- `skills/frontend-ui-ux/SKILL.md`
- `skills/git-master/SKILL.md`
- `skills/help/SKILL.md`
- `skills/note/SKILL.md`
- `skills/plan/SKILL.md`
- `skills/ralph/SKILL.md`
- `skills/ralph-init/SKILL.md`
- `skills/ralplan/SKILL.md`
- `skills/review/SKILL.md`
- `skills/security-review/SKILL.md`
- `skills/skill/SKILL.md`
- `skills/swarm/SKILL.md`
- `skills/tdd/SKILL.md`
- `skills/ultraqa/SKILL.md`
- `skills/web-clone/SKILL.md`

## Attachments

- Patch: `upstream-source-skill-sweep.patch`
- Manifest: `upstream-source-skill-sweep-manifest.json`
