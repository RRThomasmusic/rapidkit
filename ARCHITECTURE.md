# RapidKit Ecosystem Architecture

This document describes repository boundaries, ownership model, and cross-repo contracts for the RapidKit platform.

## 1) System Model

RapidKit is a multi-repository platform with clear role separation:

- `rapidkit-npm`: distribution-grade CLI entrypoint and developer bootstrap UX
- `rapidkit-vscode`: IDE-native workflow layer and command orchestration
- `rapidkit-core`: canonical engine contracts, generators, and platform logic
- `rapidkit-examples`: reference architectures that prove production usability

The design goal is to keep each repository independently evolvable while preserving stable platform contracts.

## 2) Contract Boundaries

### CLI (`rapidkit-npm`)
- Must expose stable commands and flags for workspace bootstrapping
- Must avoid coupling to editor internals
- Must defer generation contracts to `rapidkit-core`

### IDE (`rapidkit-vscode`)
- Must consume standardized command execution utilities
- Must keep platform-dependent behavior behind utility boundaries
- Must track command/API drift through tests and guardrails

### Core (`rapidkit-core`)
- Defines canonical project/module contracts
- Owns scaffolding semantics and compatibility policies
- Ships machine-readable contracts where applicable

### Examples (`rapidkit-examples`)
- Demonstrates canonical adoption patterns
- Serves as integration confidence layer for real-world scenarios
- Prioritizes reproducible reference architectures over toy demos

## 3) Integration Principles

- Source of truth lives in the owning repository
- Cross-repo changes require compatibility notes and migration guidance
- Breaking changes require coordinated release notes across affected repos
- Docs should reflect current utility and architecture patterns

## 4) Quality and Release Discipline

- Type/lint/format/test gates required per repository
- Drift guards required for contract-sensitive modules
- Multi-OS validation required for CLI and IDE layers
- Packaging and smoke checks required before release publication

## 5) Governance Model

- Hub repository defines ecosystem narrative and high-level direction
- Implementation details stay in domain repos
- RFC-style discussion is recommended for cross-repo breaking changes

## 6) North-Star Outcome

RapidKit should be perceived and operated as:

- an engineering platform ecosystem
- not a collection of disconnected tools
