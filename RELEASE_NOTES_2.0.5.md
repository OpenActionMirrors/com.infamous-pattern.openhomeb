# OpenHomeB 2.0.5

OpenHomeB 2.0.5 is a dependency maintenance release.

## What changed

- Updated tokio from 1.53.2 to 1.53.3 (PR #14).
- Updated serde_json from 1.0.151 to 1.0.154 (PR #15).
- Retained the security fixes delivered in 2.0.4.
- Includes x86_64 and aarch64 Linux binaries and the universal plugin package.

## Installation

Download `openhomeb-2.0.5-linux-universal.streamDeckPlugin` and install it through OpenDeck's Plugins screen. Restart OpenDeck after replacing the older build.

Action identifiers and the project's saved-settings format are unchanged. No action reassignment is required when upgrading from 2.0.4.

## Validation

Automated Rust, JavaScript, Python API/package, dependency-review, CodeQL, and security-audit checks must pass before publication. Both Linux packages and their checksums are verified before publication. Live OpenDeck/Homebridge interaction has not been retested for this maintenance release.

The existing allowed warning for yanked `chacha20 0.10.1` remains in the optional QUIC dependency chain.
