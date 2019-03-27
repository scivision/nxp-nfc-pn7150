# NXP NFC PN7150 Makefiles

Makefiles for NXP NFC PN7150 USB board: [MIKROE-2540](https://www.mikroe.com/nfc-usb-dongle).
The documentation recommends the [NXP driver](http://www.nxp.com/documents/software/SW4335.zip) that has Eclipse IDE project files, but no Makefiles.
I didn't want to bother with Eclipse, so I made these non-optimized Makefiles.

## Install

1. Extract SW4335.zip from NXP website
2. Change to the directory for your operating system.

    * Linux: NXP-NCI_Linux_example 
    * MacOS: NXP-NCI_MacOSX_example
    * Windows: NXP-NCI_Windows_example
3. Copy the Makefile appropriate for your operating system to that directory from this repo.


Finally run GNU Make

### Linux

```sh
apt install libhidapi-dev
```

```sh
make -f Makefile.linux
```

### Windows

Need to build [libhidapi](https://github.com/signal11/hidapi) to get libhidapi.dll

```sh
mingw32-make -f Makefile.win
```


## Notes

[NXP's NFC repo](https://github.com/NXPNFCLinux/linux_libnfc-nci/)