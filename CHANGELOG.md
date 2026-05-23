# Changelog

All notable changes to Ankor will be documented in this file.

This project follows a simple changelog format during early development. Versioning may change before the first stable release.

---

## [Unreleased]

### Added

- Initial desktop app shell.
- Saved SSH sessions sidebar.
- Terminal tab workspace.
- Local terminal entry point.
- SSH host creation flow.
- Conservative autocomplete prototype.
- Curated command-pack concept.
- Local persistence groundwork.
- Project documentation.
- Public security policy.
- Public privacy policy.
- Initial roadmap.

### Changed

- Simplified autocomplete design for v0.1.
- Removed multi-suggestion popup from the default autocomplete UX.
- Removed fuzzy matching from MVP scope.
- Removed typo correction from MVP scope.
- Removed flags/options suggestions from MVP scope.
- Removed full-line history suggestions from MVP scope.
- Limited autocomplete scope to command and first subcommand only.
- Added simple `sudo` exception for command and first subcommand completion.

### Fixed

- Prevented autocomplete from extending complete commands like `docker` into `docker-compose`.
- Prevented autocomplete from suggesting alternatives when the active token is already valid.
- Prevented malformed history fragments from becoming command candidates.
- Prevented autocomplete from guessing the next token after trailing spaces.
- Prevented flags, options, arguments, and path fragments from appearing as command-name suggestions.

### Security

- Clarified local-first security model.
- Documented that SSH credentials should remain local.
- Documented that no AI/LLM or cloud backend is required for v0.1.
- Documented privacy expectations for command history and remote command discovery.

---

## [0.1.0] - TBD

Initial MVP release.

Expected scope:

### Added

- Fast desktop SSH terminal.
- Saved SSH hosts.
- Local terminal support.
- Multiple terminal tabs.
- Local SQLite persistence.
- Conservative one-ghost autocomplete.
- Curated command packs.
- Basic settings.
- Autocomplete behavior tests.
- Public issue tracker and release notes.

### MVP Non-goals

- AI chat.
- LLM autocomplete.
- Kubernetes.
- RDP/VNC.
- Cloud sync.
- Team collaboration.
- Secrets vault.
- SFTP/file manager.
- SSH tunnels.
- Command correction.
- Fuzzy matching.
- Flags/options completion.
- Full-line history completion.
- Multi-suggestion popup.

---
