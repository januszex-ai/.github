# Contributing rules

## Workflow
1. Every change begins with an **issue** on the project board.
2. Assign the issue to yourself and move it to the **In Progress** column.
3. Create a branch from the current `main` branch, following the naming convention.
4. Open a **pull request (PR)**, fill out the template, and include `Closes #<number>`.
5. Request a code review from at least one team member.
6. Once approved and the CI pipeline passes, the author merges the PR using the **squash** method.

## Branch Naming
`<issueNumber>/<type>/<description>`

| Type | Usage |
|---|---|
| `feature/` | New functionality |
| `fix/` | Bug fix |
| `chore/` | Configuration, dependencies, maintenance tasks |
| `docs/` | Documentation |

Example: `B012/feature/user-registration`

## Commits and PR Titles (Conventional Commits)
`<type>: <description in the imperative mood>`

Types: `feat`, `fix`, `docs`, `chore`, `test`, `refactor`, `ci`, `style`

Examples:
- `feat: add user registration endpoint`
- `fix: correct email address validation`
- `ci: add test workflow`

## Code Review
- Aim to complete reviews within **24 hours** of the request.
- Provide objective and constructive feedback; every comment must be resolved before merging.
- The PR author may not approve their own changes. ## Coding Standards
- Backend: PSR-12, with style enforced by Laravel Pint.
- Frontend: ESLint + Prettier.
- Do not commit `.env` files or any secrets.
