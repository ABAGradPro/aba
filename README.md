# ABA — Application Builder Agent

ABA turns a plain-language description into a small, working web app, with a live
preview, click-to-edit, drag-and-drop, code download and version history.

Built by Ahmad, Eyad and Mohammad as a graduation project.

## Layout

| Folder      | Contents                                                        |
|-------------|-----------------------------------------------------------------|
| `apps/`     | `web` (React), `api` (NestJS), `preview`, `verifier`            |
| `packages/` | shared types, edit-mode script                                  |
| `skills/`   | SKILL.md files for Hermes and Claude Code                       |
| `infra/`    | compose files, Dockerfiles, scripts, terraform, ansible         |
| `docs/`     | `SPEC.md`, `adr/`, `build-log.md`, `design/`, `testing/`        |

## Rules

- `main` is protected: every change goes through a pull request with one approval.
- Secrets (API keys, passwords, bot tokens) never go into this repo.
- Every finished step adds one line to `docs/build-log.md`.
