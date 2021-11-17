# Elementary OS 6 installation

## If installation fails

Delete all partitions manually, and the try again the default install process.

## Post installation

- Go to `flathub.org` and install an application to add the Flathub remote to AppCenter.
- Open AppCenter and update everything.
- Open Terminal and install possibly missing drivers (NVidia for example): `sudo ubuntu-drivers install`.
- Go to Settings -> Power and disable automatic display brightness adjustment.
- Go to Settings -> Mouse & Touchpad -> Touchpad and turn off natural scrolling.
- Right click on the Dock in an empty part and select Prefereces. Change Position to whatever you prefer.
- Go to Settings -> Keyboard. Disable Super key behaviour, disable layout switch, replace the Close shortcut with Super+Q

After all applications are installed, go to Settings -> Applications -> Startup and set up auto-startup applications.

## Applications

### Generally useful

Utilities:

- Eddy (.deb installer GUI)
- Dropbox
- Antivirus (ClamTK/ClamAV)

Browsers:

- Firefox
- Brave
- Chromium
- Chrome

Text editors, office suites, etc.:

- LibreOffice
- OnlyOffice
- Joplin (complete notes application)
- Quilter (text editor)
- GIMP
- Inkscape

Other:

- Spotify
- VLC
- qBittorrent
- Steam (add i386 architecture first using `sudo dpkg --add-architecture i386`)

### Development

- VSCode (Python, ESLint, Markdown All in One, Prettier, Git Graph, Docker)
- Homebrew (Python, Node, NPM, Pipenv, ...)
- MongoDB & MongoDB Compass
- NVidia CUDA
- Slack
- VirtualBox + Guest additions
- Docker

### Useful apt packages

- curl
- gnome-disk-utility
- ffmpeg
- hardinfo
- gnome-system-monitor
