<p align="center">
  <img src="assets/logo/atelier.svg" alt="Atelier IDE" width="128">
</p>

<h1 align="center">Atelier IDE</h1>

<p align="center">
  <a href="https://github.com/atelier-ide-org/releases/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/atelier-ide-org/releases?color=6d3df5&label=release"></a>
  <a href="LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-8b39f6"></a>
  <img alt="Platforms" src="https://img.shields.io/badge/platforms-Windows%20%7C%20macOS%20%7C%20Linux-555">
</p>

<p align="center">
  A fast, modern desktop IDE written in Rust.<br>
  <a href="https://atelier-ide-org.github.io/docs/"><b>Documentation</b></a> ·
  <a href="https://atelier-ide-org.github.io/docs/fr/">Documentation en français</a> ·
  <a href="https://github.com/atelier-ide-org/releases/releases/latest">Download</a> ·
  <a href="https://github.com/atelier-ide-org/releases/releases">All releases</a>
</p>

This repository holds the downloads of Atelier: its [releases](https://github.com/atelier-ide-org/releases/releases), and no code.

## Features

- **A clean, modern interface**: Islands themes, tool window rails, Search Everywhere, run widget and familiar shortcuts. Interface in English and French.
- **Code intelligence** for JavaScript, TypeScript, Rust and Java: tree-sitter right away, then tsserver, rust-analyzer or jdtls (completion, navigation, rename, quick actions, reformat).
- **Git**: commit window, log with branch graph, branch widget, diff, conflict resolution, blame.
- **Project tools**: terminal, run configurations, npm, Maven, Gradle, translations, Kubernetes, and viewers for Markdown, Mermaid, SVG, CSV, images and Office documents.
- **For AI agents**: an MCP server for Claude Code, Codex and Gemini CLI, AI sessions, a context graph, and commits that follow the conventions of the repository.
- **Native plugins**: libraries that draw in the IDE, such as the 3D model viewer (glTF, GLB).
- **Updates itself**: a Windows installer, an `atelier` command on the PATH, and a launcher that keeps the IDE up to date.

## Install

- **Windows**: run `atelier-setup-windows-x86_64.exe` from the [latest release](https://github.com/atelier-ide-org/releases/releases/latest).
- **Linux and macOS**: download the launcher of your platform (`atelier-<os>-<arch>`) from the latest release and start it; it installs and updates the IDE next to itself.

Then `atelier .` opens the current folder. See [Installation](https://atelier-ide-org.github.io/docs/guide/getting-started).

The launcher checks this repository at every start and updates the IDE by itself.

## Releases

| Tag | Contents |
| --- | --- |
| `app/vX.Y.Z` | Atelier X.Y.Z: the installer `atelier-setup-windows-x86_64.exe`, the launchers `atelier-<os>-<arch>`, the archives `atelier-ide-<os>-<arch>` the launcher installs, and their `SHA256SUMS` |
| `plugins/<name>/vX.Y.Z` | The native plugin `<name>` for Atelier X.Y.Z: `<name>.atelier-plugin`, the file to install (its manifest and the library of each system), and `<name>-SHA256SUMS` |

The latest release of the repository is always the IDE's.

## Native plugins

A native plugin loads only in the version of Atelier it was built for: download `<name>.atelier-plugin` from the release `plugins/<name>/vX.Y.Z`, where X.Y.Z is the version of the IDE you run. Then in Atelier open **Plugins**, click **Install a plugin from a file** (the + button) and choose it: it is installed once, for every project. See [Plugins](https://atelier-ide-org.github.io/docs/plugins/).

| Plugin | Name |
| --- | --- |
| `gltf-viewer` | 3D Model Viewer: glTF and GLB models, with their animations |

## License

Atelier IDE is released under the [MIT License](LICENSE). The bundled Source Sans 3, Inter, Source Code Pro and JetBrains Mono fonts are under the SIL Open Font License.
