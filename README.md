# PtView Workstation — Official Releases

[![Platform](https://img.shields.io/badge/Platform-Windows%20x64-0078D6)](https://github.com/vntradesoft/ptview-releases/releases)
[![.NET 10](https://img.shields.io/badge/.NET-10.0-512BD4)](https://dotnet.microsoft.com/)
[![Docs](https://img.shields.io/badge/Docs-PTView%20Portal-2962FF)](https://vntradesoft.github.io/ptview-docs/)

Official distribution repository for **PtView Workstation** — a native `.NET 10` Windows desktop cryptocurrency charting workstation featuring a 60 FPS `DrawingVisual` WPF chart engine, multi-exchange real-time WebSocket streaming (`Binance`, `OKX`, `Bybit`), an integrated **ReAct AI Copilot & MCP Server**, and isolated out-of-process custom indicator plugins (`PTView.SDK`).

---

## Download & Installation

Visit the **[Releases](https://github.com/vntradesoft/ptview-releases/releases)** page and choose your preferred distribution package:

| Package | Description | Recommended For |
|---|---|---|
| **`PTViewWorkstation-win-Setup.exe`** | One-click user-scope Windows installer (`%LocalAppData%\PTViewWorkstation`, no Administrator rights required) with Desktop/Start Menu shortcuts and **Velopack background delta auto-updates**. | **Most Users (Recommended)** |
| **`PTViewWorkstation-win-Portable.zip`** | Self-contained portable archive. Extract anywhere and launch `PTView.Desktop.exe`. | USB drives, sandboxed or restricted environments |
| **`checksums-sha256.txt`** | SHA-256 verification hashes for every release artifact. | Integrity verification |

### System Requirements
- **OS**: Windows 10 (version 1809 or later) / Windows 11 — **64-bit (`win-x64`)**
- **Runtime**: Self-contained (`.NET 10` Desktop Runtime is bundled inside the installer and portable package)
- **Network**: Internet connection for live exchange WebSocket/REST streams and optional AI Copilot providers

---

## Editions: Community vs. Pro (Unified Binary)

PTView ships as a **single unified binary** — no separate downloads or reinstalls are needed to upgrade:
- **28-Day Complimentary Pro Trial**: Automatically activated on first launch (unlimited indicators, 4-chart grid layouts, external `PTView.SDK` plugins, full ReAct AI Copilot & MCP automation, 50,000+ historical bars).
- **Community Edition (Free Forever)**: Up to 2 concurrent charts per grid, up to 3 active indicators per chart, real-time Binance/OKX/Bybit feeds, and built-in drawing/analysis tools.

See the **[Editions & Update Channels Guide](https://vntradesoft.github.io/ptview-docs/editions-and-channels)** for full comparison details.

---

## Release Channels (`Stable` vs. `Beta`)

- **Stable Channel** (`vX.Y.Z`): Production-vetted releases recommended for daily live trading.
- **Beta Channel** (`vX.Y.Z-beta.N`): Early-access pre-releases featuring new UI workflows, AI Copilot / MCP enhancements, and experimental indicators.

To switch channels inside the app: **Settings (`Ctrl+,`) -> General -> Updates -> Select Channel (`Stable` / `Beta`) -> Check for Updates**.

---

## Checksum Verification (PowerShell)

Verify downloaded artifacts against `checksums-sha256.txt` before installing:

```powershell
Get-FileHash .\PTViewWorkstation-win-Setup.exe -Algorithm SHA256
```

---

## Ecosystem Links

- **Official Documentation & Release Notes**: [vntradesoft.github.io/ptview-docs](https://vntradesoft.github.io/ptview-docs/)
- **Indicator & Plugin SDK (`PTView.SDK`)**: [github.com/vntradesoft/ptview-sdk](https://github.com/vntradesoft/ptview-sdk)
- **Bug Reports & Feature Requests**: [Issues](https://github.com/vntradesoft/ptview-releases/issues)

---

## License & Third-Party Notices

Copyright (c) 2026 PtView. All rights reserved.

Application binaries are licensed under the PtView End-User License Agreement (EULA) presented on first launch. Open-source component notices are included in `ThirdPartyNotices.txt` inside the distribution package.

