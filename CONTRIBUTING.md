# Contributing

Thanks for helping improve `teacher`.
This repo is intentionally small and focused, so the best contributions are the ones that make it easier for a teacher to use.

## What this project is right now

This is v1, and v1 is scoped to the profile-building side only: `teacher.md` and `BUILD_PROFILE.md`.
The Raspberry Pi launcher and Ollama wrapper that actually run the assistant are coming later and are intentionally not in scope yet.

## What is welcome

- clearer wording in `BUILD_PROFILE.md`
- stronger example profiles
- better request/response examples
- documentation fixes
- sample profiles for different grade bands or classroom contexts

## What is not in scope yet

- the Pi setup guide or wrapper script
- anything that depends on a specific hardware setup to test
- major restructuring of the file layout without discussion first

## Rules for example profiles

If you contribute a sample `teacher.md`:

- It must be fictional or a composite, never a real filled-out profile from an actual classroom.
- It should follow the existing section structure in `teacher.md`.
- It should respect the same boundaries already baked into the template: no student names or IDs, no grading authority handed to the assistant, and distress always redirects to a trusted adult.

## Changing `BUILD_PROFILE.md`

`BUILD_PROFILE.md` is functional, not just descriptive. It is a prompt that an AI actually executes when a teacher pastes it in.
Small wording fixes are fine as a direct PR.
Anything that changes its behavior should start as an issue describing the problem you are trying to solve.

## How to submit

1. Open an issue first for anything beyond a small wording fix.
2. Fork, branch, and make your change.
3. Open a PR that briefly explains what changed and why.

## License note

By contributing, you agree your contribution is licensed under the same terms as the rest of the repo: MIT for code and scripts, CC BY 4.0 for prose, templates, and educational content.
