# Security Policy

Ankor is a desktop SSH terminal application for infrastructure engineers.

Security is critical because Ankor connects to local and remote shell environments. This document explains what is currently supported, how to report vulnerabilities, and the security principles behind the project.

## Supported Versions

Ankor is currently in early MVP / beta development.

| Version | Supported |
|---|---|
| 0.1.x | Yes |
| Older versions | No |

## Security Principles

Ankor follows these principles:

- Local-first by default.
- SSH credentials stay on the user’s machine.
- Terminal sessions are initiated by the user.
- Autocomplete must never execute commands automatically.
- Space and Enter must never accept autocomplete suggestions.
- If Ankor is unsure, it should do nothing.
- Terminal input/output must not depend on autocomplete, history, or background processing.

## Current Security Model

In Ankor v0.1:

- No cloud backend is required.
- No AI/LLM service is used.
- SSH sessions run from the local desktop app.
- Saved hosts are stored locally.
- Command history, if enabled, is stored locally.
- Remote command discovery, if enabled, runs in the background and should not print output into the visible terminal session.

## Sensitive Data

Ankor may process sensitive data locally, such as:

- hostnames and IP addresses
- usernames
- SSH connection metadata
- terminal commands
- command history
- discovered command names from remote hosts

Ankor should not intentionally collect:

- passwords in command history
- private key contents
- secrets/tokens from terminal output

If you find a case where Ankor stores or exposes sensitive data unexpectedly, please report it as a security issue.

## Reporting a Vulnerability

Please do not open a public GitHub issue for security vulnerabilities.

Report security issues by email:

```text
security@ankor.sh

Please include:

Ankor version
operating system
clear reproduction steps
expected behavior
actual behavior
screenshots/logs if safe to share