# Fix VirtualBox Kernel Driver Not Installed Error

1. Reinstall VirtualBox dynamic kernel module support package: `sudo apt install --reinstall virtualbox-dkms`. If this command fails because Linux kernel headers are not installed, run `sudo apt install linux-headers-$(uname -r)` and then retry the previous command.
2. Run the command that is suggested in the VirtualBox error dialog:`sudo modprobe vboxdrv`.
3. Reboot the system if necessary.
