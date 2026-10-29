# AIConn Homebrew Tap

Official Homebrew tap for [AgentShield](https://github.com/aiconnai/agentshield) — deterministic, offline security scanner and runtime guard for AI agent tools and MCP servers.

## Formulas

| Formula | Version | Platforms | Description |
|---------|---------|-----------|-------------|
| `agentshield` | `1.0.2` | macOS (Apple Silicon, Intel), Linux (ARM64, x86_64) | Offline security scanner and runtime guard for AI agent extensions (`SHIELD-001..037`, SARIF, auto-fix, MCP proxy) |

## Installation

```bash
brew tap aiconnai/tap
brew install agentshield
```

Or in a single command:

```bash
brew install aiconnai/tap/agentshield
```

## Quick Start

```bash
# Verify installed version
agentshield --version

# First-run setup and explained scan
agentshield quickstart

# Scan an MCP server or AI agent repository
agentshield scan . --ignore-tests --fail-on high --explain

# Generate SARIF 2.1.0 report
agentshield scan . --ignore-tests --format sarif --output results.sarif
```

## Updating

```bash
brew update
brew upgrade agentshield
```

## License

MIT — see [LICENSE](LICENSE).
