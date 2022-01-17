# buildroot-external-tree For RISC-V 
DongshanNezhaSTU For RISCV64d for aw-ol d1/d1s.

## SourceCode 
* Toolchain  https://gitlab.com/weidongshan/Toolchain/-/raw/master/riscv64-glibc-gcc-thead_20200702.tar.xz
* opensbi  https://github.com/DongshanPI/DongshanNezhaSTU-opensbi.git
* u-boot2018 https://github.com/DongshanPI/DongshanNezhaSTU-u-boot.git
* kernel https://github.com/DongshanPI/DongshanNezhaSTU-Kernel.git

## Compile & Flash
* dongshannezhaSTU-core_defconfig  mini core system.

### Support Config

### Compile
``` shell
git clone https://github.com/100askTeam/buildroot_aw-ol.git buildroot
```
``` shell
git clone  https://github.com/DongshanPI/buildroot-external-DongshanNezhaSTU 
```
``` shell
cd buildroot
```
``` shell
make BR2_EXTERNAL=../buildroot-external-DongshanNezhaSTU/ dongshannezhaSTU-core_defconfig
```

### Flash
image output `buildroot/output/images/sdcard.img`  
use dd if or  wind32diskimage flash .
