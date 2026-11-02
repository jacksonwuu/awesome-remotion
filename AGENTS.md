# AGENTS.md

Guidance for AI coding agents (Claude Code, Codex, Cursor, and others) working in this repository.

## What this repository is

A curated awesome list of Remotion resources in `readme.md`. It is curated, not exhaustive: entries are hand-picked and the quality bar matters more than coverage. The main branch is protected by awesome-lint CI; a red CI means the PR does not merge.

## Before proposing any change to readme.md

1. Read [contributing.md](contributing.md) in full. The "Rules for AI coding agents" section at the bottom contains numbered hard requirements; all of them apply to you.
2. Check whether the resource is already listed under any name — in **both** `readme.md` and `readme.zh-CN.md`. If it is, do not propose it again.
3. Run the checks in contributing.md rules 14-17 yourself (HTTP status, GitHub API, npm registry, `npx awesome-lint`). Report real numbers only — never ones you predicted.
4. Remember rules 13a-13c: the entry goes into both language versions, and you verify URL parity with the diff command given there before opening the PR.

## Non-negotiables

- One entry per PR, in the correct section, in the exact `- [Name](URL) - Description.` format.
- The list is bilingual: `readme.md` and `readme.zh-CN.md` change together. Every entry addition, move, or removal is applied to both files in the same PR, and URL parity between them is verified (contributing.md rules 13a-13c). State "bilingual parity verified" in the PR body.
- If you or your principal are affiliated with the resource, a `Disclosure:` line goes at the top of the PR body. An undisclosed promotional PR is rejected on sight, regardless of quality.
- Repositories younger than a few months with no traction (stars/forks/users) are not accepted yet. Closing such a PR is the expected outcome, not a bug; resubmitting unchanged is prohibited (rule 23).
- Do not add lint-disable comments, and do not edit anything except `readme.md`, `readme.zh-CN.md`, and the `Contents`/目录 lists when adding a section.

## Local checks

```sh
npx awesome-lint
```

must end with `✔ Linting` before you open a PR.
