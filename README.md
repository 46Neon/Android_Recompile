# Android_Recompile

Archive of compiled Blender and Godot packages that run on Termux for Android ARM64.

## Scope

- Include only the Termux-ready compiled Blender and Godot packages and their release checksums.
- Publish binary packages as GitHub Release assets, not in Git history.
- Do not mix in MiniOS, Shooter Score, other personal projects, source checkouts, SDKs, or build directories.

## Important distinction

These packages run in the Termux environment and may use Termux:X11. They are not standalone Android APKs and do not replace the separate goal of building independent Blender and Godot APKs.

## Artifact status

No binary releases have been uploaded yet. Blender 5.2.2 has a local Termux package file reported in the development environment; the corresponding Godot package still needs to be located and verified before release. Each release must state its exact version, Android ABI, Termux/X11 requirements, dependencies, SHA-256 checksum, and test result.
