# Contributing

Thanks for considering a contribution to `teacher`. This repo is intentionally small and focused - please read this before opening a PR.

## What this project is right now

This is v1, and v1 is scoped to the **profile-building side only**: `teacher.md` (the profile a teacher's local assistant reads) and `BUILD_PROFILE.md` (the guided interview prompt that helps a teacher build one). The Raspberry Pi setup script and Ollama wrapper that actually *runs* the assistant are coming later and are intentionally not in scope yet. If you're looking for that and don't see it, it's not missing by accident - it's just not built yet.

## What's welcome

- **Example profiles** for different grade bands, subjects, or classroom contexts (elementary self-contained, secondary multi-period, special education, etc.)
- **Improvements to `BUILD_PROFILE.md`** - the interview logic, question wording, edge cases it should handle better
- **Improvements to `teacher.md`** - the static template's structure or wording
- **Documentation fixes** - typos, unclear instructions, broken links
- **New example request/response pairs** following the pattern in `lesson-request-example.md` / `lesson-response-example.md`

## What's not in scope yet

- The Pi setup guide or wrapper script (coming in a later release)
- Anything that requires a specific hardware setup to test
- Major restructuring of the file layout - open an issue first to discuss

## Rules for example profiles

If you contribute a sample `teacher.md`:

- **It must be fictional or a composite, never a real filled-out profile from an actual classroom.** Even anonymized real profiles can carry identifying details about a specific school, schedule, or student population that shouldn't end up in a public repo.
- It should follow the existing section structure in `teacher.md` - don't introduce new sections without discussing them in an issue first.
- It should respect the same boundaries already baked into the template (no student names/IDs, no grading authority handed to the assistant, distress always redirects to a trusted adult).

## Changing `BUILD_PROFILE.md`

This file is functional, not just descriptive - it's a prompt that an AI actually executes when a teacher pastes it in. Small wording fixes are fine as a direct PR. Anything that changes its *behavior* (the interview flow, what it asks, how it handles edge cases like interruptions or vague answers) should start as an issue describing the problem you're solving, so we can talk through it before code changes land. This file gets tested conversationally, not just read - if you're proposing a behavior change, include an example of how a sample conversation would go differently with your change.

## How to submit

1. Open an issue first for anything beyond a small wording fix.
2. Fork, branch, make your change.
3. Open a PR referencing the issue (if applicable) and briefly explain what you changed and why.

## License note

By contributing, you agree your contribution is licensed under the same terms as the rest of the repo: MIT for code/scripts, CC BY 4.0 for prose, templates, and educational content.
