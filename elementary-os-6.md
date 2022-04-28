# Elementary OS 6 installation

## If installation fails

Delete all partitions manually, and the try again the default install process.

## Post installation

Open the Terminal and run `sudo ubuntu-drivers install` in case some drivers are missing.

- Go to `flathub.org` and install an application to add the Flathub remote to AppCenter.
- Open AppCenter and update everything.
- Go to Settings -> Power and disable automatic display brightness adjustment.
- Go to Settings -> Mouse & Touchpad -> Touchpad and turn off natural scrolling.
- Right click on the Dock in an empty part and select Preferences. Change Position to whatever you prefer.
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
- Norka (text editor)
- GIMP
- Inkscape
- Zoom
- Annotator (image annotate)

Other:

- Skype
- Spotify
- Tuner (web radio app)
- VLC
- qBittorrent
- Steam (add i386 architecture first using `sudo dpkg --add-architecture i386`)
- Fondo (wallpaper finder)

### Development

- VSCode (Extensions: Python, ESLint, Markdown All in One, Prettier, Git Graph, Docker; Preferences: format on save, default formatter, disable Accept Suggestion On Commit Character, disable explorer auto reveal feature)
- Homebrew (Python, Node, NPM, Pipenv, ...)
- MongoDB & MongoDB Compass
- NVidia CUDA
- Slack
- VirtualBox + Guest additions
- Docker

Generate `~/.ssh/id_rsa` and `~/.ssh/id_rsa.pub` using `ssh-keygen` and upload the public key to GitHub/GitLab/etc.

### Useful apt packages

- ack
- curl
- ffmpeg
- gnome-disk-utility
- gnome-system-monitor
- hardinfo
- net-tools

## Convenience

- Create `~/.bash_aliases` and define the command aliases you need (eg. `alias vscode="flatpak run com.visualstudio.code"`).
