# Development log

## 2026-09-13 - Reconcile published source into main

The current build-only workflow supersedes the older release action. Its old no-overwrite change is retained in Git history. Later catalog identities and the current recomp-ui repository URL are preserved. The pinned runtime and UI commits match v0.1.3. No new package, release, gameplay test, or source-pin promotion is claimed.

Corpus consulted: PSX-PUB-031 and FAIL-142. The existing audit_release_workflow.py parser and regression supply the repair. Primary reference: https://github.com/softprops/action-gh-release documents overwrite_files under with. Source checks cover YAML structure, Actionlint, title executable-name tests when present, manifest versions, and exact release gitlinks.
