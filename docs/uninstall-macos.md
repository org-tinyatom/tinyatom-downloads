# Uninstall TinyAtom on macOS

1. Quit TinyAtom.
2. Move `/Applications/TinyAtom.app` to the Trash.

That removes the application but intentionally leaves user data. Before deleting anything else, back up atoms or data you want to keep.

Optional cleanup locations:

- atom library: `~/TinyAtom` by default, or the custom library selected in Settings;
- managed runtimes: `<atom-library>/.tinyatom/cache/runtimes`;
- settings, Chromium session data, caches, and Electron application data: `~/Library/Application Support/TinyAtom`;
- logs: `~/Library/Logs/TinyAtom`;
- macOS preferences, if present: `~/Library/Preferences/ai.tinyatom.desktop.plist`;
- saved window state, if present: `~/Library/Saved Application State/ai.tinyatom.desktop.savedState`.

Removing an installed atom from TinyAtom is separate from removing the desktop application. Use the installed atom's data menu to export data or choose whether uninstall should also delete that atom's runtime data.
