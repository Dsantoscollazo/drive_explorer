# Google Drive in Windows 11 Explorer
Adds a Google Drive shortcut to the Windows File Explorer sidebar, just like OneDrive and Dropbox.

![Imagen de Carpeta Google Drive File Stream instalada en el explorador de windows 10](https://raw.githubusercontent.com/Dsantoscollazo/drive-explorer/master/drive-explorer.jpg
)

---

## Requirements

- Windows 11 (64-bit or 32-bit)
- [Google Drive for Desktop](https://www.google.com/drive/download/) installed
- Google Drive mapped to a drive letter (default: `G:\`)

---

## How to check if your Windows is 32-bit or 64-bit

1. Press `Win + I` to open **Settings**
2. Go to **System** → **About**
3. Under **Device specifications**, look for **System type**

You will see one of these:

| System type | Use this file |
|---|---|
| 64-bit operating system | `drive-explorer-64bit.reg` |
| 32-bit operating system | `drive-explorer-32bit.reg` |

> Almost all modern PCs running Windows 11 are 64-bit. If you are unsure, use the 64-bit version.

---

## Installation

1. Install **Google Drive for Desktop** and sign in
2. Note the drive letter assigned to your Google Drive (e.g. `G:\`)
3. Download and unzip this repository
4. Copy the `Google Drive` folder to `C:\`
5. Run the appropriate `.reg` file for your system:
   - `drive-explorer-64bit.reg` — for 64-bit Windows (most common)
   - `drive-explorer-32bit.reg` — for 32-bit Windows
6. Accept the UAC prompt to apply the registry changes
7. **Restart File Explorer** (or sign out and back in) for the changes to take effect

> If your Google Drive is mapped to a different letter than `G:\`, open the `.reg` file in a text editor and replace `G:\\` with your actual drive letter before running it.

---

## Uninstall

1. Run `remove-drive-explorer.reg`
2. Accept the UAC prompt
3. Restart File Explorer

---

## Files

| File | Description |
|------|-------------|
| `drive-explorer-64bit.reg` | Adds Google Drive to Explorer sidebar (64-bit) |
| `drive-explorer-32bit.reg` | Adds Google Drive to Explorer sidebar (32-bit) |
| `remove-drive-explorer.reg` | Removes Google Drive from Explorer sidebar |
| `Google Drive/drive.ico` | Icon used in the sidebar |

---

## Notes

- This does **not** install Google Drive — it only adds the sidebar shortcut
- The shortcut points to your locally synced Google Drive folder, not the web
- The sidebar icon uses `C:\Google Drive\drive.ico` — make sure this file exists before running the `.reg`
- Tested on Windows 11 22H2 and later
- No third-party software or scripts are executed — registry only

---

## License

MIT
