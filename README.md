# ADP Router

A simple ADP (Application Data Protocol) routing tool built with **Rust** and a modern **UI*.


## Overview

This project provides a lightweight routing utility for ADP-based networks, featuring:

- **Rust core** — performant, memory-safe routing logic
- **Modern UI** — built with HeroUI / BoardUI components (see [UI/UX Pro Max skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill))
- **CLI + GUI** — terminal interface and web-based dashboard
- **Cross-platform** — Linux, macOS, Windows

## Architecture

``a
adp-router/
├── core/           # Rust routing engine (library)
├── cli/            # Terminal interface (clap)
├── gui/            # Web UI (Tauri + React + HeroUI)
└── shared/         # Common types, protocol definitions
```

## Getting Started

### Prerequisites

- Rust 1.75+ (`rustup`)
- Node.js 20+ (for GUI)
- Tauri CLI (`cargo install tauri-cli`)

### Build CLI

```bash
cd core && cargo build --release
```

### Run GUI (dev)

```bash
cd gui && npm install && npm run tauri dev
```

## Protocol

Implements ADP routing per spec:
- Path vector routing
- Link-state advertisements
- Policy-based forwarding

## Contributing

1. Check [UI component libraries](https://uupm.cc) before building cutom components
2. Follow the 192 reasoning rules for UI/UX consistency
3. Run `cargo fmt && cargo clippy` before PR

## License

MIT | ali98afshari-star