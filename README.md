# Atelier IDE — Releases

The downloads of [Atelier IDE](https://atelier-ide-org.github.io/app/), a fast, modern desktop IDE written in Rust. This repository holds no code, only its [releases](https://github.com/atelier-ide-org/releases/releases).

## Install

- **Windows**: run `atelier-setup-windows-x86_64.exe` from the [latest release](https://github.com/atelier-ide-org/releases/releases/latest).
- **Linux and macOS**: download the launcher of your platform (`atelier-linux-x86_64`, `atelier-macos-aarch64` or `atelier-macos-x86_64`) from the latest release and start it. It installs and updates the IDE next to itself.

The launcher checks this repository at every start and updates the IDE by itself.

## What a release contains

| File | What it is |
| --- | --- |
| `atelier-setup-windows-x86_64.exe` | Windows installer |
| `atelier-<os>-<arch>` | The launcher, downloaded once |
| `atelier-ide-<os>-<arch>.zip` / `.tar.gz` | The IDE and the next launcher, installed by the launcher |
| `gltf-viewer-<os>-<arch>.zip` / `.tar.gz` | The 3D model viewer, a native plugin (see below) |
| `SHA256SUMS` | Checksums of the archives |

## Native plugins

A native plugin only loads in the IDE of **the same release**: take it from the release of the IDE you run. Extract the archive into `<project>/.atelier/plugins/gltf-viewer/`, then in Atelier open **Plugins**, click **Reload** and enable it. See [Plugins](https://atelier-ide-org.github.io/app/plugins/).

---

[Documentation](https://atelier-ide-org.github.io/app/) · [Documentation en français](https://atelier-ide-org.github.io/app/fr/)
