# teacher

`teacher` is a small public repo for a simple idea:

teachers can own a local `teacher.md` profile file that shapes how a local Ollama-based teaching assistant responds.

The goal is not to replace teacher judgment. The goal is to make a teacher-owned AI assistant easier to set up, safer to share, and more useful for lesson prep.

## What goes in this repo

- a sample `teacher.md` profile
- notes on the local Raspberry Pi workflow
- examples of the kinds of lesson-prep tasks the assistant can help with
- future blog-ready documentation about the workflow
- code and scripts are MIT licensed
- prose, templates, and educational content are CC BY 4.0

## How it works

1. A teacher fills out `teacher.md`
2. A small local wrapper reads that profile
3. The wrapper sends the profile and the current request to Ollama
4. The model answers in the teacher's preferred style and structure

## Why this matters

- the teacher keeps control of the profile
- the assistant stays local and openweight
- classroom preferences live in a file instead of being hidden in a black box
- the same pattern can work across grade levels and subjects

## Starter files

- [teacher.md](teacher.md) - a starter classroom profile
- [lesson-request-example.md](lesson-request-example.md) - a sample prompt pattern
- [LICENSE](LICENSE) - MIT license for code and scripts
- [CONTENT_LICENSE](CONTENT_LICENSE) - CC BY 4.0 for written content

## Next steps

- tailor the sample profile for different grade bands
- add a Pi setup guide
- add a blog post draft about the teacher.md idea
