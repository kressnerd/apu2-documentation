PC Engines APU2 coreboot Release Notes
--------------------------------------

Releases 4.0.x are based on PC Engines 20160304 release

### 4.0.1.1

#### coreboot

  * Reprogram `GPP_CLK3` output (connected to miniPCIe slot 1) to ignore `CLKREQ#`
    input - force it to be always on.

### 4.0.1

#### coreboot

  * introduce versioning
  * obtain `smbios` fields, such as `board serial` and `SKU`
  * reduce log level: display mainboard, DRAM and ECC info only
  * improve SD card performance
  * force to use SD in 2.0 mode
  * nct5104d driver backport
  * check if `git` exists before calling it
  * change git repository in `Makefile`
  * add missing `cbfs_find_string` in `libpayload`
  * add executable bit to `xcompile`

#### SeaBIOS

  * allow for one-time `PXE ` boot with `N` key
  * enable/disable `USB` boot
  * enable/disable `PXE` boot
  * prevent from printing character multiple times

#### Sortbootorder

  * merge all `USB` entries into one
  * add `(disabled)` tag in menu
  * interface modification
  * version bump to v1.3
  * add `PXE` and `USB` enable options in menu
  * add `PXE` to bootorder menu
  * change interface to lower case
  * version bump to v1.2
  * change letter for save and exit to `S`
  * use proper way to access extended SPI registers
  * add support for `yangtzee fch spi controller`
  * user interface improvements
  * add `PC Engines` header
  * add `README` and `Makefile`
  * initial commit based on
    [coreboot_140908](http://pcengines.ch/tmp/coreboot_140908.tar.gz)

#### Memtest86plus

  * add macro `SPD_DISABLED ` for disabling SPD related functionality
  * fix refresh procedure so that full screen content is reprinted on refresh
  * add refresh option label (`l`) to bottom menu
  * enable serial console by default
  * based on [memtest86plus](https://review.coreboot.org/cgit/memtest86plus.git?)

#### iPXE

  * mirror of [iPXE git tree](http://git.ipxe.org/ipxe.git)