# dualra1n

A script that lets you dualboot iOS 13.7 (semi-tethered) on [checkm8](https://www.theiphonewiki.com/wiki/Checkm8_Exploit)-vulnerable devices.

- WARNING, in this branch both jailbreak is automatically installed so the --jailbreak so you mustn't use in this branch.
# Usage

Example: `./dualboot.sh --dualboot 13.7`

`--dualboot`          Dualboot your iDevice.

`--jail-palera1n`     Use this when you are already jailbroken with semi-tethered palera1n to avoid disk errors. 
   
`--fixHard`           Fixes microphone, girocopes, camera, audio, touch, etc. (the Home button is not fixed yet)

`--help`              Print this help.

`--dfuhelper`         A helper to help you enter DFU if you are struggling to do it manually.

`--boot`              Lets you boot into dualbooted iOS. use this when you are already dualbooted . Usage : ./dualboot.sh --boot

`--dont-create-part`   Skips creating a new disk partition if you have them already, so using this this downloads the boot files. Usage : ./dualboot.sh --dualboot 14.3 --dont-create-part.

`--restorerootfs`     Deletes the dualbooted iOS. (also add --jail-palera1n if you are jailbroken semi-tethered with palera1n)
    
`--recoveryModeAlways`    Fixes the main iOS when it is recovery looping.

`--debug`             Makes the script significantly more verbose. (meaning it will output exactly what command it is running)

`clean`               Deletes the created boot files.

# Dependencies
- A deactivated passcode on A10-A11 
- An .iPSW file for iOS 13.7 
- Around 15 gigabytes of free storage
- A computer with macOS or Linux (if you have neither, you can temporarily "install" a Linux distro to RAM)
# Warnings
- I am **NOT** responsible for any data loss. The user of this program accepts responsibility should something happen to their device.
 **If your device is stuck in recovery, please run one of the following:**
   - futurerestore --exit-recovery
   - irecovery -n
   - ./dualboot.sh --recoveryModeAlways

# Ideal Dualboot Versions and some informations
iOS 13 is working but only 13.6, 13.7. If you want to dualboot iOS 13, use the [ios13](https://github.com/dualra1n/dualra1n/tree/ios13) branch.

- on ios 13 booting take like 15 minutes on a9 devices and probably on a10 as well.

# Common Issues, use --fixHard to fix the most of the firmwares, you can find more information on a full tutorial here below

- A9 : Everything works except touch id.

- A10/11/X: Home button is not working. You can, however, use tweaks like GesturesXV to simulate iPhone X gestures. You can also activate Assistive Touch on the main iOS and have it also enabled on the dualbooted iOS.

- iPads may have issues with "Deep Sleep" (iOS not "waking up" after the display going to sleep). Installing the tweak [Fiona](https://www.ios-repo-updates.com/repository/julioverne-s-repo/package/com.julioverne.fiona/) may fix this.

# How would I dualboot?

- [A full tutorial](https://github.com/dualra1n/dualra1n/blob/main/tutorial.md)

# Credits

<details><summary>Thanks to:</summary>
<p>

- [Edwin](https://github.com/edwin170) owner :)
- [Uckermark](https://github.com/Uckermark/dualra1n-loader) thank you so much for the amazing dualra1n loader app to jailbreak it.
- Edward, my brother, for giving me a Hackintosh to test this on
- [sasa](https://github.com/sasa8810) thank for improve the dfu timing on macos
- [Fatih](https://github.com/swayea) for helping with the readme, testing linux support and being a very good person.
- [plooshi](https://github.com/plooshi) thank you so much for help to fix the home button issue.

   - [azaz0322](https://github.com/m00nl1ghts), [Huy Nguyen](https://github.com/34306), [DarwinUang](https://github.com/DarwinUang) and [aditya11110](https://github.com/aditya11110) for helping with the readme\
</details>
<details><summary>Credits for tools used in dualra1n</summary>

- [Dualboot guide](https://dualbootfun.github.io/) for the guide
- [palera1n](https://github.com/palera1n) for some of the code
- [opa334](https://github.com/opa334/TrollStore) amazing app
- [blacktop](https://github.com/blacktop) for the iPSW downloader
- [Nathan](https://github.com/verygenericname) for the ramdisk
- [Amy](https://github.com/elihwyma) for the [Pogo](https://github.com/elihwyma/Pogo) app
- [Mineek](https://github.com/mineek) thank you for the Kernel15patcher which is a kpf midfied to use with bootx.
- [checkra1n](https://github.com/checkra1n) for the base of the kpf
- [m1sta](https://github.com/m1stadev) for [pyimg4](https://github.com/m1stadev/PyIMG4)
- [tihmstar](https://github.com/tihmstar) for [pzb](https://github.com/tihmstar/partialZipBrowser)/original [iBoot64Patcher](https://github.com/tihmstar/iBoot64Patcher)/original [liboffsetfinder64](https://github.com/tihmstar/liboffsetfinder64)/[img4tool](https://github.com/tihmstar/img4tool)
- [xerub](https://github.com/xerub) for [img4lib](https://github.com/xerub/img4lib) and [restored_external](https://github.com/xerub/sshrd) in the ramdisk
- [libimobiledevice](https://github.com/libimobiledevice) for several tools used in this project (irecovery, ideviceenterrecovery etc), and [nikias](https://github.com/nikias) for keeping it up to date
- [Dora](https://github.com/dora2-iOS) for kpf
- [Sam Bingner](https://github.com/sbingner) for [Substitute](https://github.com/sbingner/substitute)
- [CoolStar](https://github.com/coolstar) for [Libhooker](https://libhooker.com/docs/index.html)
- [Ralp0045](https://github.com/Ralph0045) for [dtree_patcher](https://github.com/Ralph0045/dtree_patcher) and [Kernel64Patcher](https://github.com/Ralph0045/Kernel64Patcher)
- [0x7ff](https://github.com/0x7ff/gaster) thank you so much for the gaster tool.
</details>
</p>
