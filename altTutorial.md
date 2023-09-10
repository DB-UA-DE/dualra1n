# Alternative Tutorial on dualbooting your device
This is an alternative and more detailed tutorial on how you can
dualboot your **iDevice** with iOS 15, 14 or 13.
## Getting the script
First of all, you need to have `git` installed on your system, to install it, 
write the command in the terminal depending on what distribution you have.
### Ubuntu and Debian-based
> sudo apt install git
### Fedora and RHEL
> sudo dnf install git
### Arch-based
> sudo pacman -S git
### OpenSUSE
> sudo zypper install git
### macOS
You will need to instal XCode Command Line Tools with this following command:
> xcode-select --install

### Downloading the script
If you have any other distribution, please check on how to install packages 
and try to install `git` with it.

Then, go to folder where you want to download your script (f.e. Documents) and write the next:
> git clone --recursive https://github.com/dualra1n/dualra1n.git

or if you want to dualboot iOS 13:
> git clone -b ios13 --recursive https://github.com/dualra1n/dualra1n.git

After that you will have the script downloaded.

## Preparing to dualboot
To start the dualbooting process, you have to make sure that you have your TouchID/FaceID and Passcode disabled
since you may get errors during the install process. Then make sure that you have `ramdisk` folder since it is 
needed to complete the setup. After you make sure that everything's ok, you can go to the next step. If 
you have problems then go to the Troubleshooting.

## Dualboot
Now you can start the dualboot. Open the terminal and go to the dualra1n folder,
and write the following depending to what you need:

For example, dualboot iOS 13 with `palera1n` ever installed on the host iOS:

`./dualboot.sh --dualboot 13.7 --jail-palera1n`

or just iOS 14.3:

`./dualboot.sh --dualboot 14.3`

Lorem ipsum
