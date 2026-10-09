# Android_Recompile

Experimental, reproducible build recipes and patches for adapting open-source desktop software to Android ARM64, primarily for Termux.

> **Status: experimental.** This repository has not yet produced a complete Blender or Godot build or APK.

## Goals

- Build and validate Android ARM64 software from pinned upstream source revisions.
- Keep build scripts, small patches, manifests, hashes, and test results in Git.
- Publish verified binaries through GitHub Releases rather than storing large binaries in Git history.

## Compatibility

- Ordinary Linux/PC x86_64 binaries do not run natively on Android ARM64. Software must be built or ported for the Android/Bionic environment, or packaged using a compatible runtime.
- A program that runs inside Termux is not automatically a standalone APK; it may depend on Termux libraries and services.

## Planned targets

| Project | Status | Notes |
|---|---|---|
| Blender | Experimental, in progress | The Android CMake configure/generate stage has succeeded after local host-tool adaptations. The generated `makesdna` host tool still fails at runtime because the link command contains both `-pie` and a later `-no-pie`. No complete Blender build or APK exists yet. |
| Godot Engine | Planned | No build has been attempted in this repository yet. |

## Current Blender experiment

- Target ABI: `arm64-v8a`; the experiment is focused on Android API 29 or later.
- Build host: Termux on Android ARM64.
- The current build uses an experimental Termux-backed NDK-layout shim, not a validated official NDK toolchain.
- Local CMake adaptations are experimental and have not been upstreamed.
- Smoke tests, host-tool builds, full Blender builds, and installed APK tests must be reported as separate milestones.

## Release checklist

For every published artifact, record the upstream commit, ABI and Android API level, toolchain and build commands, applied patches, SHA-256 checksum, required license notices, and actual device-test results. Do not describe a smoke test or partial build as a complete application.
