# teacher

`teacher` is a small public repo for one simple idea: a teacher should own the file that shapes how a local AI assistant helps them.

The heart of the workflow is a plain text profile called `teacher.md`. It captures classroom context, preferences, supports, and boundaries so the assistant can give help that feels consistent and useful instead of generic.

## Start here

1. Open [`BUILD_PROFILE.md`](BUILD_PROFILE.md) if you want a guided interview that helps you build a profile from scratch.
2. Open [`teacher.md`](teacher.md) if you want a starter profile you can fill in directly.
3. Read [`PRIVACY.md`](PRIVACY.md) before adding any real classroom details.
4. Keep the file local and update it as your classroom changes.

## What this repo includes now

- [`BUILD_PROFILE.md`](BUILD_PROFILE.md) - a copy/paste interview prompt for building `teacher.md`
- [`teacher.md`](teacher.md) - a starter classroom profile
- [`lesson-request-example.md`](lesson-request-example.md) - a simple request pattern to test against
- [`lesson-response-example.md`](lesson-response-example.md) - the kind of short, usable output this project aims for
- [`PRIVACY.md`](PRIVACY.md) - what local use protects, and what it does not
- [`CONTRIBUTING.md`](CONTRIBUTING.md) - how to propose improvements
- [`LICENSE`](LICENSE) - MIT license for code and scripts
- [`CONTENT_LICENSE`](CONTENT_LICENSE) - CC BY 4.0 for prose, templates, and educational content

## How it works

1. A teacher fills out `teacher.md` directly, or uses `BUILD_PROFILE.md` in any chat tool to build one section by section.
2. The profile lives on hardware the teacher controls.
3. A local assistant reads the profile and a lesson request.
4. The assistant answers in the teacher's preferred style, length, and format.

## What this repo is not

- It is not a full product yet.
- It does not include the Raspberry Pi launcher or the Ollama wrapper that runs the assistant.
- It does not replace teacher judgment.
- It does not make classroom privacy automatic.

## Privacy in plain language

Local use keeps the profile off a cloud AI account, but local does not mean magically safe.
Do not put real student names, ID numbers, or other identifying details into `teacher.md` or any request you send to the assistant.
If you want the fuller version, read [`PRIVACY.md`](PRIVACY.md).

## Want to contribute?

Contributions are welcome, especially:

- clearer wording in `BUILD_PROFILE.md`
- stronger example profiles
- better request/response examples
- documentation fixes

If you are proposing a behavior change, open an issue first so we can talk through the tradeoffs.
