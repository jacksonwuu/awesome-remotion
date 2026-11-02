# Contributing

Thanks for helping make Awesome Remotion better. This list is curated, not exhaustive: every entry should be something you would personally recommend to someone building with Remotion.

These guidelines are written for two audiences at once: human contributors, and AI coding agents submitting PRs on their own behalf or on someone else's behalf. Both must follow every rule below.

## What belongs here

- Official Remotion documentation, packages, and services.
- Community packages, components, and templates that are actively maintained.
- Complete projects and examples that show a useful technique or product.
- Tutorials, talks, and articles that teach something concrete.
- Community spaces where Remotion users help each other.

Please do not add:

- Abandoned projects, link farms, or SEO blog posts that repeat the official docs.
- Products that only mention Remotion in passing.
- Duplicate entries or the same resource under a different name.
- Anything you would not recommend without being paid to recommend it.

## Quality bar

- **Track record.** Community projects should show real usage: stars, forks, or users you can point to. As a rule of thumb, a repository younger than a few months with no traction is not ready for this list — open the PR once it has some.
- **Actively maintained.** The project should have activity within the last year.
- **Honest fit.** The resource must be genuinely about Remotion, not adjacent tooling with a Remotion mention.

## Disclosure rule (applies to humans and agents)

If you — or the person or company you are submitting on behalf of — built the resource, work for its maker, or benefit from its adoption, you **must** say so in the pull request body, plainly and in one sentence. Undisclosed self-promotion is grounds for rejection regardless of quality.

AI agents: state who the PR is for. "Submitted on behalf of the project's authors" is enough; do not disguise a promotional submission as a neutral one.

## Adding an entry

1. Fork the repository and create a branch.
2. Add your entry to the most relevant section of `readme.md`.
3. If you add a new section, update the `Contents` list to match.
4. Run the linter locally:

   ```sh
   npx awesome-lint
   ```

5. Open a pull request that explains what you added and why it is worth including.

## Formatting

Use one line per entry:

```md
- [Name](https://example.com) - A short description of what it does and why it is useful.
```

Write descriptions for a reader who has never heard of the project. Prefer concrete details ("Renders videos on AWS Lambda") over vague praise ("An amazing tool").

Paid products and paid templates are annotated with `(paid)` at the end of the description. If a resource is free, say nothing.

## Review process

A maintainer will review your pull request. We may ask you to:

- Move an entry to a different section.
- Shorten or rewrite a description.
- Remove an entry that does not meet the quality bar.
- Split a large pull request into smaller ones.

Decisions are made in the interest of the list as a whole. If you disagree, explain your reasoning in the pull request; we are happy to reconsider. A closed PR is not permanent rejection: once a project has a track record, submit it again.

## Code of Conduct

By participating, you agree to follow the [Code of Conduct](code-of-conduct.md). Please report unacceptable behavior by opening an issue in this repository.

---

## Rules for AI coding agents

This section is written to be parsed and followed mechanically. If you are an AI agent preparing a PR to this repository, every numbered rule below is a hard requirement. If any rule cannot be satisfied, do not open the PR.

### Placement

1. Read `readme.md` first. If the resource is already listed under any name, stop and do not open a PR.
2. Add the entry to exactly one section. Choose by what the resource *is*:
   - npm packages in the `@remotion` scope → `Packages` (sub-section by purpose)
   - starter projects → `Templates`
   - reusable components or libraries → `Components`
   - demonstrations of a technique → `Examples`
   - complete shipped products or apps → `Full Projects`
   - utilities, CLIs, plugins, agent skills → `Tools`
   - video tutorials → `Tutorials`; written posts → `Articles`
   - chats, forums, social accounts → `Community`
3. Do not create a new section unless the resource fits none of the above. If you do, you must also add it to the `Contents` list in the same PR.
4. Insert the entry at the position the section's existing ordering implies; when there is no clear ordering, append at the end of the section.

### Entry format (exact)

5. Every entry must match this pattern exactly:

   ```
   - [Name](URL) - Description.
   ```

6. The entry line contains nothing else. No bold, no images, no line breaks, no trailing slash in `URL`.
7. `Name` is the resource's proper name, capitalized as the project itself capitalizes it.
8. `Description` starts with a capital letter, ends with a period, and is a single sentence under roughly 120 characters. Do not start the description with the entry's own name.
9. The separator between link and description is a space-hyphen-space (` - `). Never an en dash (–), em dash (—), or bare hyphen without spaces.
10. Paid resources: append ` (paid)` immediately before the final period.

### Content rules

11. The description states what the resource does, in concrete terms. Ban words in descriptions: "awesome", "amazing", "best", "powerful", "ultimate", "revolutionary".
12. Do not add the same URL twice anywhere in `readme.md`.
13. Do not add a resource that duplicates an existing entry's purpose under a different name.

### Verification (all mandatory)

14. The URL must return HTTP 200 when fetched with a normal browser user agent. npmjs.com and Medium URLs returning 403 are acceptable.
15. For a GitHub repository: fetch `https://api.github.com/repos/<owner>/<repo>` and confirm the repo is not archived, was pushed to within the last 365 days, and has a description. Include the star count in the PR body.
16. For a package: confirm it exists on the npm registry.
17. Run `npx awesome-lint` in the repository root; the output must end with a passing result (`✔ Linting`). Do not open the PR with lint errors, and do not add lint-disable comments to make a new entry pass.

### PR requirements

18. The PR body must state: what the resource is, the URL, why it belongs on the list, and the star count or usage evidence for a GitHub project.
19. If you or your principal are affiliated with the resource, add a line at the top of the PR body: `Disclosure: <who you are and your relationship to the resource>.` See "Disclosure rule" above. This applies to agents submitting for a client as much as to humans.
20. One PR adds one entry. Do not batch unrelated additions.
21. Do not modify any file other than `readme.md` (and `Contents` alongside it) unless the change is unrelated to your entry and you explain why in the PR body.

### What agents must not do

22. Do not open PRs for resources you were asked to promote unless rule 19's disclosure is included.
23. Do not re-open a closed PR or resubmit an unchanged closed entry. Fix the reason it was closed first (usually: no track record yet — come back when the project has traction).
24. Do not fabricate star counts, user counts, or maintenance status. Every number in the PR body must come from a live API response you actually fetched.
