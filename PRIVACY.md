# Privacy & Data Handling

This document explains what a local, `teacher.md`-driven assistant protects and what it does not.
Read this before you trust it with anything related to your classroom.

## What "local" means here

The intended setup runs an open-weight model on hardware you control, like a Raspberry Pi, with no required internet connection for the assistant itself to function.
That means:

- Your `teacher.md` profile and the requests you send to the assistant are not sent to a cloud AI provider.
- There is no remote account or vendor dashboard in the day-to-day loop.
- Nothing about how you use the assistant is logged by a third party by default.

This is the main reason the project exists: classroom preferences and workflows should live in a file you own, on hardware you control.

## What "local" does not mean

Running locally is not the same as being automatically safe or private in every sense.
Specifically:

- **Local does not mean encrypted.** If your Raspberry Pi or the device it's on is lost, stolen, or accessed by someone else, anything stored on it, including `teacher.md`, is readable unless you have separate encryption in place.
- **Local does not protect you from what you type in.** If you type a real student's name, ID number, or other identifying detail into a request or into `teacher.md`, that information now lives in a file on your device.
- **Local does not mean backed up.** If you want a safe copy of your profile, that is a separate step you need to take on purpose.
- **Local does not mean the assistant can detect a crisis.** If a student ever uses the assistant directly, the assistant has no reliable way to detect distress, self-harm risk, or other safety concerns on its own. `teacher.md` should always state a clear rule, like "tell the student to find a trusted adult right away," instead of relying on the assistant to notice and respond correctly.

## Our one hard rule: no real student data, ever

Every part of this project is built around one rule: **do not enter real student names, ID numbers, or other identifying details into this assistant.** Describe patterns, groups, and general needs instead.

This rule exists because a local assistant does not have a built-in way to protect sensitive student information the way a vetted school system might.
The protection here is structural: keep the data out in the first place.

## If your school or district has its own policies

Nothing in this repo overrides your school or district's data privacy policies, student data agreements, or applicable laws, including FERPA in the US.
If your school has rules about what tools can touch student information, those rules still apply here.
When in doubt, check with your school's IT or administration before connecting this to anything that touches real student records.

## Questions or concerns

If you find a privacy or safety gap in how this repo's files are written, please open an issue.
Boundary and safety language in `teacher.md` and `BUILD_PROFILE.md` should be treated as load-bearing, not cosmetic.
