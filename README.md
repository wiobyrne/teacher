# teacher

`teacher` is a small public repo for a simple idea:

teachers can own a local `teacher.md` profile file that shapes how a local Ollama-based teaching assistant responds.

The goal is not to replace teacher judgment. The goal is to make a teacher-owned AI assistant easier to set up, safer to share, and more useful for lesson prep.

## What this is right now (v1 scope)

This release covers the **profile-building side only**: the `teacher.md` file itself, and `BUILD_PROFILE.md`, a guided interview prompt that helps a teacher build one using any AI chat tool they already have. The Raspberry Pi setup guide and the local Ollama wrapper that actually runs the assistant are coming in a later release - they're not missing by accident, just not built yet. See **Next steps** below.

## What goes in this repo

- `BUILD_PROFILE.md` - a paste-in interview prompt that helps an AI chat tool build `teacher.md`
- a sample `teacher.md` profile
- notes on the local Raspberry Pi workflow
- examples of the kinds of lesson-prep tasks the assistant can help with
- an example response shape that shows the full profile -> request -> output loop
- `PRIVACY.md` - what running this locally actually protects, and what it doesn't
- `CONTRIBUTING.md` - how to propose example profiles or improvements
- future blog-ready documentation about the workflow
- code and scripts are MIT licensed
- prose, templates, and educational content are CC BY 4.0

## How it works

1. A teacher either fills out `teacher.md` directly or pastes `BUILD_PROFILE.md` into an AI chat tool to interview them section by section
2. A small local wrapper reads that profile
3. The wrapper sends the profile and the current request to Ollama
4. The model answers in the teacher's preferred style and structure

## Why this matters

- the teacher keeps control of the profile
- the assistant stays local and openweight
- classroom preferences live in a file instead of being hidden in a black box
- the same pattern can work across grade levels and subjects

## Privacy and safety

This project is built around one hard rule: no real student names, IDs, or other identifying details should ever be entered into `teacher.md` or into a request sent to the assistant. Local doesn't mean automatically safe - see `PRIVACY.md` for what running this locally actually protects, what it doesn't, and why boundary language in `teacher.md` and `BUILD_PROFILE.md` is written the way it is.

## Starter files

- [BUILD_PROFILE.md](BUILD_PROFILE.md) - interview-style builder prompt
- [teacher.md](teacher.md) - a starter classroom profile
- [lesson-request-example.md](lesson-request-example.md) - a sample prompt pattern
- [lesson-response-example.md](lesson-response-example.md) - a sample output shape
- [PRIVACY.md](PRIVACY.md) - data handling and privacy explainer
- [CONTRIBUTING.md](CONTRIBUTING.md) - how to contribute
- [LICENSE](LICENSE) - MIT license for code and scripts
- [CONTENT_LICENSE](CONTENT_LICENSE) - CC BY 4.0 for written content

## Contributing

This repo is open to contributions - example profiles for different grade bands and subjects, improvements to the interview logic in `BUILD_PROFILE.md`, and documentation fixes are all welcome. See `CONTRIBUTING.md` for what's in scope and how to submit changes.

## Next steps

- add a Raspberry Pi setup guide
- build the local Ollama wrapper script
- tailor the sample profile for different grade bands
- add a blog post draft about the `teacher.md` idea
