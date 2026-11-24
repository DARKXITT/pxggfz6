# PXGG FZ6

**PXGG FZ6** is a local-first companion app for **Forza Horizon 6**: live driving
tools, garage control, teleportation, photo mode, and tuning, in one clean
Windows app.

This repository hosts the official installer and release notes only. The
application source is closed and is not published here.

## Download

Grab the latest installer from the [Releases](../../releases/latest) page:

```
PXGG FZ6 Setup.exe
```

No accounts, no sign-up, no bundled extras.

## Install

Run `PXGG FZ6 Setup.exe` and follow the wizard. The app installs per-user to:

```
%LOCALAPPDATA%\Programs\PXGG FZ6
```

Desktop and Start Menu shortcuts are optional. The installer can also run
silently:

```powershell
& ".\PXGG FZ6 Setup.exe" --install "D:\Games\PXGG FZ6" --desktop --start-menu
```

## Uninstall

Use **Settings → Apps → PXGG FZ6 → Uninstall**, or run `Uninstall.exe` from the
install folder:

```powershell
"Uninstall.exe" --uninstall --quiet                # keeps reports, presets, backups, settings
"Uninstall.exe" --uninstall --quiet --remove-data  # removes everything
```

## Updates

The app checks this repository's latest release on startup and every 6 hours.
When a newer version is published, the HUB shows an update card and installs it
over the current version, keeping your data. You can also check manually in
**Settings → Updates**.

## What the app writes

Everything stays inside the app folder:

```
reports\             Local feedback reports and SQL reference
dumps\               Optional database dumps
save_backups\        Local save backups
teleport_lists\      Local teleport lists
driving_presets\     Local driving presets
car_lists\           Local car lists
PXGG_FZ6.log         Local log
PXGG_FZ6.ini         Local settings
```

## Disclaimer

PXGG FZ6 is an independent, fan-made companion tool intended for single-player
use. It is not affiliated with, endorsed by, or connected to Microsoft, Xbox
Game Studios, Playground Games, or Turn 10 Studios. Forza and Forza Horizon are
trademarks of Microsoft Corporation. Use at your own risk.
