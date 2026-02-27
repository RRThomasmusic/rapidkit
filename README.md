# RapidKit

> **The workspace engineering platform for production-grade backend projects.**  
> Scaffold, operate, and evolve your stack — from first commit to enterprise scale.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Website](https://img.shields.io/badge/website-getrapidkit.com-0f172a?logo=google-chrome&logoColor=white)](https://www.getrapidkit.com)
[![Organization](https://img.shields.io/badge/GitHub-getrapidkit-1f6feb?logo=github)](https://github.com/getrapidkit)

RapidKit is an open-source workspace platform that brings together a CLI, IDE extension, core engine, and curated examples into one cohesive workspace experience. Whether you are starting a new service or scaling an existing one, RapidKit enforces consistency, automates boilerplate, and keeps your team in flow.

---

## Get Started

| Tool | Install | Docs |
|---|---|---|
| CLI | `npm install -g rapidkit` | [rapidkit-npm →](https://github.com/getrapidkit/rapidkit-npm) |
| VS Code Extension | [Marketplace](https://marketplace.visualstudio.com/items?itemName=rapidkit.rapidkit-vscode) | [rapidkit-vscode →](https://github.com/getrapidkit/rapidkit-vscode) |
| Examples | — | [rapidkit-examples →](https://github.com/getrapidkit/rapidkit-examples) |

> **Fastest path to a running project:**  
> Install the VS Code extension, open the **RapidKit Welcome** panel, browse the official example workspaces, and clone any of them directly into your environment — no CLI commands needed to get started.

---

## Ecosystem

| Layer | Repository | Purpose |
|---|---|---|
| CLI | [rapidkit-npm](https://github.com/getrapidkit/rapidkit-npm) | Developer entrypoint and command UX |
| IDE | [rapidkit-vscode](https://github.com/getrapidkit/rapidkit-vscode) | VS Code integration and workflow automation |
| Core Engine | [rapidkit-core](https://github.com/getrapidkit/rapidkit-core) | Core scaffolding engine and runtime contracts |
| Examples | [rapidkit-examples](https://github.com/getrapidkit/rapidkit-examples) | Reference architectures and production-grade templates |

## Platform Topology

```text
  +------------------+
  | rapidkit-vscode  |  (IDE layer)
  +---------+--------+
            |
+-----------+----------+     +----------------+
| rapidkit-npm  (CLI)  |<--->| rapidkit-core  |
|  Developer UX        |     | Engine + APIs  |
+-----------+----------+     +----------------+
            |
  +---------+----------+
  | rapidkit-examples  |  (Reference & adoption)
  +--------------------+
```

## About This Repository

This repo is the **ecosystem hub** — it does not contain runnable code.  
It exists to:

- Provide a single discovery point for contributors and adopters
- Define ecosystem-level architecture and ownership boundaries
- Track cross-repo direction, roadmap, and release plans

## Docs

- [Architecture](ARCHITECTURE.md)
- [Roadmap](ROADMAP.md)
- [Contributing](CONTRIBUTING.md)

---

## Contributing

Contributions are welcome across all layers. Read [CONTRIBUTING.md](CONTRIBUTING.md) to understand how the ecosystem is structured and where to start.
