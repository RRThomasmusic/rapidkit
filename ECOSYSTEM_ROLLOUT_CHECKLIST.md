# RapidKit Ecosystem Rollout Checklist

Use this checklist to align all repositories with the central platform hub.

## 1) README Alignment (All Repos)

- Add platform badge at top of README
- Add one-line repo role statement
- Add “Part of RapidKit Ecosystem” section linking this hub

Badge snippet:

```md
[![Part of RapidKit Platform](https://img.shields.io/badge/Part%20of-RapidKit%20Workspace%20Platform-0f172a?logo=github)](https://github.com/getrapidkit/rapidkit)
```

## 2) Cross-Repo Navigation

- Ensure each repo links to the other primary repos:
  - `rapidkit-npm`
  - `rapidkit-vscode`
  - `rapidkit-core`
  - `rapidkit-examples`
- Keep links in a dedicated “Ecosystem” section

## 3) Positioning Consistency

- Use language that presents RapidKit as a platform ecosystem
- Avoid repo descriptions that make the system look disconnected
- Keep CLI/IDE/Core/Examples responsibilities explicit

## 4) Release and Quality Expectations

- Ensure each repo exposes its quality gates in docs
- Ensure tests are actually executed in CI for each repo
- Ensure platform-sensitive drift checks remain active where needed

## 5) Examples Upgrade Path

Target structure for `rapidkit-examples`:

- `fastapi-ai-agent`
- `nestjs-microservice`
- `gofiber-api`
- `polyglot-workspace`
- `enterprise-workspace`

Each example should include:

- architecture diagram
- local run instructions
- production notes
- why this reference matters

## 6) Governance Rhythm

- Monthly ecosystem sync issue in this hub
- Quarterly roadmap refresh in `ROADMAP.md`
- Cross-repo breaking changes tracked with linked issues
