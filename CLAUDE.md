# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) and other AI
assistants when working with code in this repository.

## Current state of the repository

> **Important:** As of the last update to this file, this repository is a
> fresh, essentially empty project. The only tracked content is `README.md`
> (which currently holds just the project title, "Fanfic"). There is **no**
> source code, build system, dependency manifest, test suite, or CI
> configuration yet.
>
> Do not assume a language, framework, or directory layout that is not
> actually present. When you add the first real code, **update this file** in
> the same change so it always reflects the true state of the project.

### What this means for you, the assistant

- Don't fabricate build/test/lint commands. None exist yet — if asked to run
  them, say so and offer to set them up.
- Don't invent an architecture or module structure. There isn't one to
  describe.
- When scaffolding the project for the first time, propose a structure to the
  user (or follow their stated intent), then record the decisions here.

## Project intent

The repository is named **Fanfic**. The README is a single title line, so the
concrete goals are not yet defined in the codebase. If the purpose is unclear
for a given task, ask the user rather than guessing.

## Repository layout

```
.
├── README.md     # Project title only (to be expanded)
└── CLAUDE.md     # This file — guidance for AI assistants
```

Update this tree as directories and files are added.

## Development workflow

### Branching

- The default branch is `main`.
- Active development for AI-assisted work happens on feature branches.
- **Never** push directly to `main` without explicit permission. Create a
  feature branch, commit there, and push that branch.
- Use `git push -u origin <branch-name>` so the upstream is set.

### Commits

- Write clear, descriptive commit messages in the imperative mood
  (e.g. "Add story model", not "Added story model").
- Keep commits focused: one logical change per commit where practical.
- Only commit or push when the user asks you to.

### Pull requests

- Do **not** open a pull request unless the user explicitly requests one.

## Conventions to establish

The following are not yet decided. Capture each decision here as it is made:

- **Language / runtime** — TBD
- **Package manager** — TBD
- **Build command** — TBD
- **Test command** — TBD
- **Lint / format tooling** — TBD
- **Directory structure** — TBD

## Keeping this file accurate

Treat `CLAUDE.md` as living documentation. Whenever you:

- add a build, test, or lint command,
- introduce a framework or major dependency,
- establish a directory convention, or
- change the development or release workflow,

…reflect that change here in the same commit. An out-of-date CLAUDE.md is
worse than none, because it misleads future assistants.
