
uuu_1.2.68 / 2019-01-31
=======================

  * Fixed random stop at linux environment

uuu_1.2.66 / 2019-01-25
=======================

  * fixed crash when DONE cmd is not last one
  * fixed #79 all data is zero when file transfer from target to windows PC
  * fix -b qspi failure
  * FB added set_active command
  * Avoid add addition space when convert cmd arg

uuu_1.2.61 / 2019-01-16
=======================

  * Fix 8mq skipspl ivt search problem
  * Old i.MX8MQ SPL bcd use 0x9999
  * fix memory leak
  * fix windows random crash when multi device running
  * remove duplicated SDPV line

uuu_1.2.56 / 2019-01-09
=======================

  * Fix linux build failure
  * fix windows built failure
  * fixed #70 usbfs: process uuu did not claim interface 0 before use
  * Image size need minus IVT offset
  * update default SDPV command option
  * Update built-in script to support SDPV command
  * Support -skipspl option at sdp protocol
  * Change SPPV usb bcd version from 0x500
  * Support Filter a range or BCDVersion number
  * MAC build success
  * Update Readme.md to add pkg-config to linux apt
  * Fix typos in user visible strings
  * fix -Wreturn-type in `runshell`
  * usb bcd distinguish SDPU
  * Only download size that imx8qm and imxqxp's container header indicator
  * Fixed windows build failure
  * add built-in script fat_write

uuu_1.2.39 / 2018-12-13
=======================

  * Update libusb link to folk's link
  * Only show auto complete help message when print help
  * notify.cpp: prevent crash by catching exception
  * doxygen support

uuu_1.2.31 / 2018-11-29
=======================

  * Update Readme for better format
  * Update license info
  * Update appveyor.yml
  * Added static link project for windows

uuu_1.2.26 / 2018-11-28
=======================

  * Fix add quota for FB[-t 1000]: Only filename need quota

uuu_1.2.24 / 2018-11-27
=======================

  * fix built-in script always have quota
  * Support space in Path
  * Fixed uuu "fb[-t 1000]:" ucmd problem
  * fix a2x build problem when wiki include signed off
  * Fix sudo uuu auto complete problem
  * add help -udev option to generate udev rule
  * tell sudo uuu have problem
  * Improve uuu autocomplete txt and put into Microsoft.PowerShell_profile.ps1
  * Add one more new line about autocomplete
  * Fix crash when parameter more than script required
  * fall back to verbose mode if vt mode enable failure
  * improve linux auto complete
  * skip x86 build output file
  * skip debug and x86 build for linux side
  * Add debug version build
  * fix rebase missed e3c4b56 commit change
  * Move auto complete into separate file
  * powershell auto complete basic work
  * Remove VT color code at win7 environment
  * win32 also use static link
  * Fix windows 32bit build problem
  * Update appveyor.yml
  * Update appveyor.yml
  * fix auto complete problem with path
  * Fix windows version build failure
  * fix uboot command in shell mode
  * show help tell user use auto complete
  * linux basic auto complete work
  * linux auto complete basic work
  * just print help if run uuu
  * SPDS support BLOG
  * SPL：added SDPU: done command
  * SDPU fetch log blog command
  * Add timeout support for HID read command
  * EXPERIMENTAL: Added Blog command to capture console log
  * Add a u-boot shell command mode.
  * lookup libbz2 not by filename but by library name
  * flush output after wait for known usb device appear
  * Update Readme add build status-badges

uuu_1.2.0 / 2018-10-31
======================

  * update version number to 1.2.x

uuu_1.1.112 / 2018-10-31
========================

  * update appveyor.xml to add history of uuu.pdf
  * Update README.md
  * Update README.md

uuu_1.1.108 / 2018-10-30
========================

  * update artifacts
  * linux clone mfgtools.wiki.git
  * linux install rename
  * Update appveyor.yml
  * Update appveyor.yml
  * Update appveyor.yml
  * Update appveyor.yml
  * Use static link C library
  * Update appveyor.yml
  * Update appveyor.yml
  * Update appveyor.yml
  * Update README.md

uuu_1.1.95 / 2018-10-25
=======================

  * Update README.md
  * Add missed bz2 project file
  * libbz2 have not provide pkg-config
  * add linux build support
  * support decompress bz2 file
  * add bzip2 code
  * Rewrite zip and sdcard fat handle code
  * check original file size to avoid crash when use small image
  * Fix jump command overwrite data that caused security image boot failure
  * Update README.md

uuu_1.1.87 / 2018-10-17
=======================

  * increase qspl write timeout value to 20s
  * Merge pull request #60 from cwald/patch-1
  * Update README.md
  * fix linux build error
  * Move shell mode to low priority
  * windows: using FSCTL_REQUEST_OPLOCK to monitor file change

uuu_1.1.81 / 2018-09-26
=======================

  * Update qspi_burn_loader.lst

uuu_1.1.79 / 2018-09-25
=======================

  * correct fix windows file lock problem
  * Remove debug message
  * In windows system don't buffer memory mapped file because it prevent update target file during daemon mode.

uuu_1.1.76 / 2018-09-25
=======================

  * Fix crash for some imx6/7's image
  * convert uuu.cpp to unix text format
  * fix linux build error and popen fail if mode is "rb" in linux
  * fix linux build failure
  * Add shell command support
  * Merge pull request #56 from angolini/typo2
  * uuu.cpp: Fix Typo
  * Increase max each bulk transfer to 1M
  * Reduce polling to 200ms because libusb_get_device_list take 66ms.
  * Move common command under _ALL: to avoid copy to each protocol

uuu_1.1.61 / 2018-09-13
=======================

  * improve error message for libusb
  * Limited max download size to 16M for sparse file to avoid long timeout
  * Merge pull request #55 from angolini/typo
  * libuuu: Fix typo in error message
  * Merge pull request #53 from nsjodk/cosmetic
  * cosmetic: fix indentation
  * Merge pull request #52 from nsjodk/master
  * cmake: make install, installs uuu in bin
  * Merge pull request #51 from Raphexion/master
  * remove unused (un-read) variable
  * Merge pull request #50 from nsjodk/doc
  * Merge pull request #49 from nsjodk/master
  * README: correct the github path
  * modern cmake: set cxx standard
  * Update README.md
  * Merge pull request #48 from nsjodk/master
  * modern cmake - minimal version 3.4
  * consistent cmake_minimum_required
  * Merge pull request #47 from nsjodk/master
  * config.h: #pragma once before includes
  * Add q\quit to exit shell

uuu_1.1.41 / 2018-08-22
=======================

  * Update qspi erase timeout value to 40s
  * built-in qspi support burn difference image
  * Fastboot add flashing and oem command
  * Update README.md

uuu_1.1.35 / 2018-08-16
=======================

  * add sd_all into default script
  * fix linux build failure
  * optimize version info
  * remove redundant hash value
  * use last tag as build version when build from git

uuu_1.1.29 / 2018-08-15
=======================

  * fix linux build error
  * Fix crash when connect 2 board and load from zip file
  * Async unzip file
  * Notify application when zip file
  * Delay 100ms in case some thread have not exit and send out THREAD_EXIT notify message
  * Remove debug message
  * linux: correct build_ver
  * Remove duplicate build number info
  * Fix windows build problem cause by createversion.bat
  * roll back version number to 1.1.4
  * linux update gen script to recongize appver build number
  * windows recognize appver build number
  * Parse version info from version string
  * Fix open zip file failure
  * FB flash support timeout

uuu_1.1.16 / 2018-08-13
=======================

  * fix mmc emmc partition ack setting
  * built-in emmc_all, sd, spl scripts
  * Improve help message
  * improve cmake clst generate
  * improve error message
  * Fix wrong path handle at failure parser build in command
  * fix linux build
  * Added built-in script support

uuu_1.1.7 / 2018-08-10
======================

  * add -offset document
  * imx8mq skip HDMI firmware
  * SDPS add option -offset to skip some header

uuu_1.1.3 / 2018-08-09
======================

  * Fix protocol case sensitive problem in script

uuu_1.1.1 / 2018-08-07
======================

  * Update build number to 1.1.x
  * Fixed miss ":" at parser uuu script
  * Fix [-t 1000] parser problem at uuu script
  * Added Timeout for FB protocol.

uuu_1.0.86 / 2018-08-02
=======================

  * Fine tune help information
  * Fix -v PID\VID miss algined at IMXRT106X

uuu_1.0.84 / 2018-07-31
=======================

  * clean up some warning for windows build
  * Clean up warning
  * clean up some warning
  * Fixed a typo
  * Add -V option to print libusb error and warning information
  * work around libusb 1/10 open device failure at windows platform
  * Merge pull request #44 from eramox/feature/OOT_build
  * Merge pull request #43 from eramox/fix/fix_different_issues
  * Fix trailing whitespace in the project
  * fix checkpatch
  * Fix warning in uuu
  * Support build of the project from a tarball
  * Support Out Of Tree build

uuu_1.0.74 / 2018-07-24
=======================

  * Added MX8QM support
  * Move ROM info to separated file
  * Add i.MX8MQ support
  * Update README.md
  * Update README.md
  * Update README.md
  * Merge pull request #39 from angolini/README_update
  * README: Fix typo and add missing libzip-dev
  * README: Update the formatting of code block

uuu_1.0.59 / 2018-07-11
=======================

  * add delay command
  * fb: avoid a small package after big package
  * Merge pull request #34 from MrVan/opensuse-fix
  * Add appveyor.yml
  * uuu: fix build on openSUSE tumbleweed

uuu_1.0.53 / 2018-07-05
=======================

  * sdpu: use default address
  * Added missed SDPU done command support
  * Enable cursor when exit program
  * fix issue #33 add try sudo uuu
  * fix i.mx7ulp pid number
  * Merge pull request #32 from falstaff84/master
  * avoid warning
  * Support uboot sdpu protocol to continue with SPL
  * Change uuu output to the same folder with libusb

1.0.44 / 2018-06-21
===================

  * Fix build error
  * remove reduntant data in gitsubmodules
  * Dynamic link libusb
  * Add MXRT106X support
  * Added License file
  * Update README.md
  * Test push hook
  * Update README.md
  * using stadic-libstdc++ to reduce dependence

uuu_1.0.35 / 2018-05-25
=======================

  * fb flash always convert to sparse format
  * fix divided by zero problem
  * Fix build warning
  * Merge remote-tracking branch 'github/uuu'
  * Merge pull request #29 from agavemountain/uuu
  * linux mmap work
  * Precode Linux mmap version
  * Using mmap to read files
  * Fixed CMAKE relative path error
  * Add FB flash command description
  * Fix stack overflow when read sdcard image file
  * use back file if filename is ..
  * Don't return error when can't commands for protocol
  * RAW to sparse work.
  * Add usb path filter support
  * fix linux build
  * Add FAT partition file read
  * Every thread have independence command list
  * Capture ctrl_c to show cursor

uuu_1.0.28 / 2018-05-22
=======================

  * unified file path
  * Add timeout to 5s for flash command
  * Fix linux build problem
  * Added miss file
  * Support split android sparse file
  * precode fastboot flash command
  * Add submodule libsparse
  * fix linux build failure
  * Index start from 1
  * Fix line mass up if error happen
  * Optimize output
  * Correct fastboot transfer size notification error.
  * Fix current path set wrong when use uuu xxx.zip
  * Test web trigger
  * Update README.md
  * Update FBK vid pid info
  * Update README.md
  * Update README.md
  * Update README.md