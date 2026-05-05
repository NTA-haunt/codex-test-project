# Repository Guidelines

## Project Structure & Module Organization

This repository is currently a small JavaScript project with a single entry point:

- `index.js`: main script and current function implementation.
- `.idea/`: local IDE metadata; do not rely on this for project behavior.

As the project grows, place reusable source files under `src/`, tests under `test/` or `tests/`, and static assets under `assets/`. Keep modules focused and export functions that need to be tested rather than only exercising behavior through `console.log`.

## Build, Test, and Development Commands

No package manifest or build system is currently defined. Use direct Node execution for the current code:

- `node index.js`: runs the script locally.
- `git status --short`: checks changed and untracked files before committing.

If you add `package.json`, define standard scripts such as `npm test`, `npm run lint`, and `npm run start`, then keep this section updated.

## Coding Style & Naming Conventions

Use JavaScript with clear, small functions. Prefer:

- 2-space indentation for new JavaScript files.
- `camelCase` for functions and variables, for example `divideNumbers`.
- Descriptive names over abbreviations.
- `const` by default, `let` only when reassignment is required.

Avoid committing debugging-only `console.log` calls unless the script is intentionally command-line output. Keep comments short and useful; explain why something exists, not what each line does.

## Testing Guidelines

There is no test framework configured yet. When adding tests, prefer a common JavaScript runner such as Node's built-in test runner or Jest. Name test files after the module they cover, for example `test/index.test.js` or `tests/divide.test.js`.

At minimum, cover normal cases, edge cases, and invalid inputs. For the current division behavior, tests should clarify expected handling of division by zero.

## Commit & Pull Request Guidelines

The repository has no commit history yet, so use a simple, consistent convention:

- Write commit messages in the imperative mood, for example `Add division tests`.
- Keep each commit focused on one logical change.
- Include a short PR description, testing notes, and linked issue when applicable.
- Add screenshots only for user-visible UI changes.

Before opening a PR, run the available commands and confirm `git status --short` only shows intentional changes.

## Agent-Specific Instructions

Respond to repository users in Vietnamese by default. Keep code, commands, filenames, API names, and quoted error messages in their original language when that preserves accuracy.
