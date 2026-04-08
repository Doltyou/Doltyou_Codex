# oh-my-codex skill doc upstream bundle

This repository packages the local documentation-only skill changes prepared for upstream submission.

## Contents

- `skills/*/SKILL.md`: current cleaned source copies from the local `oh-my-codex` package
- `exports/patch.diff`: upstream-friendly relative-path patch
- `exports/manifest.json`: per-file change manifest
- `exports/pr-summary.md`: PR/body draft
- `exports/commit-message.txt`: Lore-format commit message draft

## Provenance

Source files were collected from:
`C:\Users\doltyou\AppData\Roaming\npm\node_modules\oh-my-codex\skills`

The bundle was created from the validated portability/source-sync sweep run on 2026-04-08.

## Verification performed

- source catalog search for legacy slash-style invocation patterns returned zero matches
- source catalog search for targeted stale tool/reference patterns returned zero matches
- `omx setup --scope user` completed successfully after the sweep
- synchronized active installed/source skill hashes matched after reinstall