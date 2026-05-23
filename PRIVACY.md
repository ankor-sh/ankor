# Privacy Policy

Ankor is designed as a local-first desktop SSH terminal.

This policy describes what Ankor stores, what it does not collect, and how data is handled in the current MVP/beta version.

---

## Summary

In Ankor v0.1:

- No account is required.
- No cloud backend is required.
- No AI/LLM provider is used.
- Terminal data is not uploaded to cloud.
- SSH hosts and command history are stored locally on your machine.
- You stay in control of your SSH sessions.

---

## Data Stored Locally

Ankor may store the following data locally:

- Saved SSH host entries
- Display names for hosts
- Hostnames or IP addresses
- Ports
- Usernames
- Recent sessions
- Terminal settings
- Command history, if enabled
- Discovered command names from remote hosts, if enabled
- App preferences

This data is stored locally for app functionality such as saved sessions, recent sessions, and autocomplete.

---

## SSH Credentials

Ankor may support different SSH authentication methods, such as:

- Password authentication
- Private key authentication
- SSH agent authentication

The preferred model is to use existing local SSH mechanisms, such as SSH agent or key files, without copying private key contents into Ankor storage.

Ankor should not upload SSH credentials to any cloud service.


## Autocomplete

Ankor includes a local autocomplete feature to make common terminal commands faster to type.

Autocomplete in Ankor v0.1 is conservative and local-first:

- It does not use AI or LLMs.
- It does not send terminal input to external services.
- It does not execute commands automatically.
- It only shows one visual ghost suggestion at a time.
- Suggestions are accepted only when the user presses `Tab`.
- `Space` and `Enter` always behave like normal terminal input.

Autocomplete suggestions may be based on:

- Curated built-in command packs, such as common Linux, Git, Docker, systemd, and package-manager commands.
- Commands discovered from the connected host, if remote command discovery is enabled.
- Local command history, if command history is enabled.

Command history does not create arbitrary new autocomplete suggestions in Ankor v0.1. It may only help rank suggestions that are already known to be valid commands or supported subcommands.

Remote command discovery, when enabled, may run a background command such as:

```bash
compgen -c
