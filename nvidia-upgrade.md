# (HARD) Nvidia proprietary driver upgrade

Only do this if the operating system is unable to upgrade the driver using its own tooling (app/software center or update manager application).

## Ubuntu 20-based distros (e.g. elementary OS 6)

1. Remove all nvidia packages: `sudo apt remove --purge '^nvidia-.*'`
2. Remove automatically install, but unused packages: `sudo apt autoremove`
3. Update package list: `sudo apt update`
4. Reinstall recommended NVidia proprietary drivers: `sudo ubuntu-drivers install`
5. Restart the operating system.
