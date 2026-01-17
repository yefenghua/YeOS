# YeOS
Custom linux kernel and operating system

## Build environment

1. install dependencies.
    ```shell
    sudo apt-get install libx11-dev libc6-dev build-essential xorg-dev libgtk2.0-dev libreadline-dev
    ```
2. download [bochs2.7](https://sf-west-interserver-2.dl.sourceforge.net/project/bochs/bochs/2.7/bochs-2.7.tar.gz?viasf=1) and unzip.
3. edit config.
   ```shell
   ./configure --with-x11 --with-x --enable-all-optimizations --enable-readline  --enable-debugger-gui --enable-x86-debugger --enable-a20-pin --enable-fast-function-calls --enable-debugger
   ```
4. compile bochs.
   ```shell
   make -j4
   sudo make install
   ```
5. install qemu.
   ```shell
   sudo apt-get install qemu
   ```