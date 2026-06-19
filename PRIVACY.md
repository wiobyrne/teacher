# Privacy & Data Handling

This document explains what running a local, `teacher.md`-driven assistant actually protects - and what it doesn't. Read this before you trust it with anything related to your classroom.

## What "local" means here

The intended setup runs an open-weight model (via Ollama) on hardware you control, like a Raspberry Pi, with no required internet connection for the assistant itself to function. That means:

- Your `teacher.md` profile and the requests you send to the assistant are not sent to a cloud AI provider.
- There's no remote account, login, or company server in the loop for the assistant's day-to-day use.
- Nothing about how you use the assistant is logged by a third party by default.

This is the core reason the project exists: classroom preferences and workflows should live in a file you own, on hardware you control, not inside a black box you have to trust blindly.

## What "local" does not mean

Running locally is not the same as being automatically safe or private in every sense. Specifically:

- **Local doesn't mean encrypted.** If your Raspberry Pi or the device it's on is lost, stolen, or accessed by someone else, anything stored on it - including your `teacher.md` file - is readable unless you've taken separate steps to encrypt the device or the file.
- **Local doesn't protect you from what you type in.** If you type a real student's name, ID number, or other identifying detail into a request or into `teacher.md` itself, that information now lives in a file on your device. The assistant has no way to know that information is sensitive and remove it for you - the protection has to come from you not entering it in the first place.
- **Local doesn't mean backed up.** If you want to keep a copy of your profile somewhere safe, that's a separate step you'd need to take deliberately - and if you do, think about where that copy lives and who can access it.
- **Local doesn't mean the assistant can detect a crisis.** If a student ever uses the assistant directly (most setups described in this repo assume they won't, but some teachers may choose to allow it), the assistant has no reliable way to detect distress, self-harm risk, or other safety concerns on its own. `teacher.md`'s Boundaries section should always state a clear, explicit rule - like "tell the student to find a trusted adult right away" - rather than relying on the assistant to notice and respond appropriately on its own. It won't reliably notice.

## Our one hard rule: no real student data, ever

Every part of this project - `teacher.md`, `BUILD_PROFILE.md`, and any example profiles in this repo - is built around one rule: **no real student names, ID numbers, or other identifying details should ever be entered into this assistant.** Describe patterns, groups, and general needs instead ("a few students reading below grade level," not "Jamie, who reads at a 1st grade level"). If you ever want to reference a specific situation in a request (like drafting a parent email), use a placeholder like "Student A" instead of a real name.

This rule exists because a local assistant has no built-in mechanism to recognize or protect sensitive student information the way a vetted, FERPA-compliant school system might. The protection here is structural - keep the data out in the first place - not something the software does for you after the fact.

## If your school or district has its own policies

Nothing in this repo overrides your school or district's data privacy policies, student data agreements, or applicable laws (like FERPA in the US). If your school has rules about what tools can touch student information, those rules still apply here. When in doubt, check with your school's IT or administration before connecting this to anything that touches real student records.

## Questions or concerns

If you find a privacy or safety gap in how this repo's files are written, please open an issue. Boundary and safety language in `teacher.md` and `BUILD_PROFILE.md` should be treated as load-bearing, not cosmetic - see `CONTRIBUTING.md` for how to propose changes to that logic.
