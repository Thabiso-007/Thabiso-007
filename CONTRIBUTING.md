# Maintaining this profile

This repository powers the README on [Thabiso's GitHub profile](https://github.com/Thabiso-007). Changes merged into `main` become public. Keep the content concise, accurate and welcoming.

## Local setup

Use Node.js 22 or newer and npm.

```sh
npm ci
npm run check
```

- `npm run lint` checks Markdown structure, headings and link fragments.
- `npm run format:check` checks consistent formatting.
- `npm run format` applies formatting; review the diff before committing.
- `npm run check` runs both checks and is the same command used in CI.

The lockfile keeps tool versions reproducible. Commit `package-lock.json` whenever dependencies change. Do not commit `node_modules`, environment files or credentials.

The `katex` and `re2js` overrides in `package.json` supply patched transitive dependencies for the Markdown linter. When upgrading the linter, run `npm audit`, check whether these overrides are still needed, and remove them once its own dependencies include the fixes.

## Updating content

1. Edit `README.md` and keep its section navigation in sync with the headings.
2. Verify project descriptions against the actual source, not just an old summary.
3. Link both source and deployment when available. Check that hosted projects still load and note any setup limitations.
4. Separate demonstrated work, additional skills and active learning. Do not invent employment history, metrics, endorsements or completed certifications.
5. Keep contact details consistent with the portfolio and the profile owner's approved public information.
6. Prefer local assets for essential branding. Give images descriptive alternative text and keep third-party statistics optional.
7. Preview the Markdown on GitHub, including light and dark themes and a narrow viewport, before merging.

## Visual assets

The header is an editable SVG at `assets/profile-header.svg`. Keep its text consistent with the README, preserve the accessibility title and description, and check legibility when scaled down.

## Pull requests

Use the pull request checklist and include the validation you performed. The profile-quality workflow checks formatting and Markdown; it does not verify external deployment availability or the truth of biographical claims. Those still need human review.

This is a personal profile, not a general-purpose open-source library. Content changes should be approved by the profile owner. No license is granted for reusing the personal biography or branding.
