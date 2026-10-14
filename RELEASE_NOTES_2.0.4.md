# OpenHomeB 2.0.4

OpenHomeB 2.0.4 is a security and dependency maintenance release. Upgrading from earlier versions is recommended.

## What changed

- Updated rustls from 0.23.45 to 0.23.46 to address RUSTSEC-2026-0346, RUSTSEC-2026-0347, RUSTSEC-2026-0348, and RUSTSEC-2026-0349.
- Updated quinn-proto from 0.11.16 to 0.11.18 to address RUSTSEC-2026-0338, RUSTSEC-2026-0340, and RUSTSEC-2026-0342 in the lockfile's optional QUIC dependency chain.
- Updated log to 0.4.34, tokio to 1.53.2, and openaction to 2.8.0.
- Includes x86_64 and aarch64 Linux binaries and the universal plugin package.

## Installation

Download `openhomeb-2.0.4-linux-universal.streamDeckPlugin` and install it through OpenDeck's Plugins screen. Restart OpenDeck after replacing the older build.

This release does not change action identifiers or the project's saved-settings format. No action reassignment is required when upgrading from 2.0.3.

## Validation

Automated Rust, JavaScript, Python API/package, dependency-review, CodeQL, and security-audit checks are required before publication. Live OpenDeck/Homebridge interaction has not been retested for this maintenance release.

The existing allowed warning for yanked `chacha20 0.10.1` remains in the optional QUIC dependency chain.
