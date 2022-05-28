
# a135f-T-u3

1. Edit makefile to 

CROSS_COMPILE= ~/toolchains/aarch64-linux-android-4.9-master/bin/aarch64-linux-android-

CC= ~/toolchains/android_prebuilts_clang_host_linux-x86_clang-5484270-9.0/bin/clang

CLANG_TRIPLE= ~/toolchains/proton-clang-13-clang/bin/aarch64-linux-gnu-

2. Build

make clean && make mrproper
export PLATFORM_VERSION=11
export ANDROID_MAJOR_VERSION=r
export ARCH=arm64
make physwizz_defconfig
make


