# Ankor Roadmap
---

## v0.1 — MVP

Goal: fast SSH terminal with saved sessions and conservative local autocomplete.

Planned:

- Fast terminal workspace
- Multiple terminal tabs
- Saved SSH hosts
- Local terminal support
- Local SQLite persistence
- Basic settings
- Conservative autocomplete
- Curated command packs
- Basic command history
- Remote command discovery

Autocomplete v0.1:

- One ghost suggestion only
- No AI/LLM
- No fuzzy matching
- No typo correction
- No flags/options suggestions
- No full-line history suggestions

---

## v0.2 — Stability

Focus:

- SSH config import
- SSH agent support
- Better private key auth
- Better connection errors
- Better local terminal profiles
- History/cache controls
- More tests
- Signed Windows builds

---

## v0.3 — Workflow

Focus:

- Session groups
- Host tags
- Better quick connect
- Recent sessions
- Split panes
- User snippets
- Per-host notes

---

## Later

Possible future features:

- Kubernetes support
- SFTP/file browser
- SSH tunnels
- Bastion host support
- Optional AI-assisted explanations
- Team workspaces
- Shared runbooks

AI features, if added, should be optional, transparent, and never execute commands without explicit user approval.