# Android_Recompile

Archive of compiled Blender and Godot packages that run on Termux for Android ARM64.

## Scope

- Store only the Termux-ready Blender and Godot package files and their checksums as GitHub Release assets.
- Do not mix in other projects, source checkouts, SDKs, or build directories.
- These packages are references for the separate goal of building standalone Android APKs; they are not APKs themselves.

## Published release

[termux-arm64-2026-10](https://github.com/46Neon/Android_Recompile/releases/tag/termux-arm64-2026-10)

| Package | Version | File | SHA-256 |
|---|---|---|---|
| Blender | 5.2.2 | `blender5_5.2.2_aarch64.deb` | `962b91de9454a57787ba1045c515f66d60cc2e08936c881633da9e4aa6b4d3f3` |
| Godot | 4.7.2 | `godot_4.7.2_aarch64.deb` | `4b2238d176a55177a5b940af43739aa1d1780da01247f9790f0c658c1a0dc93b` |

The release also includes `Termux-ARM64-SHA256SUMS.txt`.

## Compatibility

These are Termux packages for Android ARM64 and may be used with Termux:X11. They are not standalone Android APKs and require their dependencies from Termux repositories.
