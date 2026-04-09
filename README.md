# Google Drive in Windows 11 Explorer
Adds a Google Drive shortcut to the Windows File Explorer sidebar, just like OneDrive and Dropbox.

![Imagen de Carpeta Google Drive File Stream instalada en el explorador de windows 10](https://raw.githubusercontent.com/Dsantoscollazo/drive-explorer/master/drive-explorer.jpg
)

Requirements

Windows 11 (64-bit or 32-bit)
Google Drive for Desktop installed
Google Drive mapped to a drive letter (default: G:\)


Installation

Install Google Drive for Desktop and sign in
Note the drive letter assigned to your Google Drive (e.g. G:\)
Download and unzip this repository
Copy the Google Drive folder to C:\
Run the appropriate .reg file for your system:

drive-explorer-64bit.reg — for 64-bit Windows (most common)
drive-explorer-32bit.reg — for 32-bit Windows


Accept the UAC prompt to apply the registry changes
Restart File Explorer (or sign out and back in) for the changes to take effect


If your Google Drive is mapped to a different letter than G:\, open the .reg file in a text editor and replace G:\\ with your actual drive letter before running it.


Uninstall

Run remove-drive-explorer.reg
Accept the UAC prompt
Restart File Explorer


Files
FileDescriptiondrive-explorer-64bit.regAdds Google Drive to Explorer sidebar (64-bit)drive-explorer-32bit.regAdds Google Drive to Explorer sidebar (32-bit)remove-drive-explorer.regRemoves Google Drive from Explorer sidebarGoogle Drive/drive.icoIcon used in the sidebar

Notes

This does not install Google Drive — it only adds the sidebar shortcut
The shortcut points to your locally synced Google Drive folder, not the web
Tested on Windows 11 22H2 and later
No third-party software or scripts are executed — registry only


License
MIT


