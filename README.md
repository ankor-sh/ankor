# Ankor

Ankor is a fast desktop SSH terminal for infrastructure engineers.

This repository is used for public issues, releases, roadmap, and documentation.  
The source code is currently maintained in a private repository.

## Status

Ankor is currently in early MVP/beta development.

## Tech Stack

Ankor is built with:

- **Wails** — desktop application framework
- **Go** — backend, SSH/session logic, local services
- **React + TypeScript** — frontend UI
- **xterm.js** — terminal rendering
- **SQLite** — local persistence
- **TailwindCSS** — UI styling

## Maintainer

Ankor is maintained by [Dumitru Catan](https://www.linkedin.com/in/dumitru-catan-214225177/), a DevOps engineer focused on infrastructure, automation, and developer tooling.

Feedback, bug reports, and feature requests are welcome through GitHub Issues.

## Privacy & Security

Ankor is local-first. In v0.1, it does not use AI/LLMs, does not require a cloud backend, and does not upload terminal input, terminal output, SSH hosts, or command history.

See [PRIVACY.md](./PRIVACY.md) and [SECURITY.md](./SECURITY.md).

## Roadmap & Releases

- [Roadmap](./ROADMAP.md)
- [Changelog](./CHANGELOG.md)