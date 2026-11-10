# todo-adlc-mobile

Mobile app for the todo ADLC pilot. The stack and target platforms are not chosen yet: they are decided in the accepted spec.md for CHG-001. Until then, sections marked "Not defined" stay empty. Do not fill them by guessing.

## Commands
Not defined. Phase 2 adds one command each for build, test and lint, each with an example of healthy output, plus a way for the agent to see the UI (screenshot or simulator).

## Verifying your work
Run the build, test and lint commands above before reporting any task complete, and paste the output. Never skip or delete a failing test. For UI work, compare a screenshot against the approved design and iterate.

## Conventions
Not defined. Filled from the accepted CHG-001 spec.md.

## Architecture
Not defined, except: this app consumes the API contract owned by todo-adlc-api. Pin the contract version you build against in plan.md and test against it. Never change the contract from this repo; propose the change in the spec instead. A mobile change that needs a new API version merges after the API change.

## Change artifacts
- Plan: `docs/changes/<id>/plan.md`, from `../todo-adlc-specs/templates/plan.md`.
- Intent and spec: `../todo-adlc-specs/changes/<id>/`, read at the commit pinned in plan.md.

<!-- adlc-rules:begin v1 -->
## ADLC rules (shared by Claude Code and Codex)

1. Every change has an ID `CHG-NNN-slug`. Its intent.md and spec.md live in `todo-adlc-specs/changes/<id>/`. Its plan.md lives in each affected code repo at `docs/changes/<id>/plan.md`.
2. No implementation without an accepted plan.md for the change ID. If there is none, stop and produce a plan instead.
3. Read intent.md and spec.md at the specs-repo commit recorded in the plan.md header, not at the latest commit.
4. If the implementation departs from plan.md, update plan.md in the same commit.
5. For a bug fix, write a failing test first and commit it. After that, do not edit test files during the fix.
6. Before reporting a task done, run the build, test and lint commands listed under "Commands" and paste their output. If a test fails, fix the code, not the test.
7. Never push to `main`, approve a pull request, merge your own pull request, or deploy beyond the dev environment.
8. Never read, print or commit secrets (`.env*`, keys, tokens). Never disable TLS verification or authentication, not even for testing.
9. Do not introduce a language, framework or dependency that the accepted spec.md does not name.
10. When the same mistake is corrected twice, propose adding it to "Things agents get wrong" in AGENTS.md.
<!-- adlc-rules:end -->

## Things agents get wrong
None recorded yet.
