# oh-my-codex skill doc upstream bundle

This repository packages the local documentation-only skill changes prepared for upstream submission.

## Contents

- `skills/*/SKILL.md`: current cleaned source copies from the local `oh-my-codex` package
- `exports/upstream-source-skill-sweep.patch`: upstream-friendly relative-path patch
- `exports/upstream-source-skill-sweep-manifest.json`: per-file change manifest
- `exports/UPSTREAM_PR_SUMMARY.md`: PR/body draft
- `exports/UPSTREAM_LORE_COMMIT_MESSAGE.txt`: Lore-format commit message draft

## Provenance

Source files were collected from:
`C:\Users\doltyou\AppData\Roaming\npm\node_modules\oh-my-codex\skills`

The bundle was created from the validated portability/source-sync sweep run on 2026-04-08.

## Verification performed

- source catalog search for legacy slash-style invocation patterns returned zero matches
- source catalog search for targeted stale tool/reference patterns returned zero matches
- `omx setup --scope user` completed successfully after the sweep
- synchronized active installed/source skill hashes matched after reinstall