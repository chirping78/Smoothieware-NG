# Smoothieware-NG

This project supports two mbed offline development environments: mbed cli and gcc4mbed.

## Build with gcc4mbed

```
git clone https://github.com/chirping78/Smoothieware-NG
cd Smoothieware-NG
git submodule init
git submodule update

cd gcc4mbed/
./linux_install
cd ..

cd src
make NUCLEO_F401RE
```

## Build with mbed cli

Please install [mbed CLI](https://github.com/ARMmbed/mbed-cli#installing-mbed-cli).

Use mbed cli to download the code and compile:
```
mbed import https://github.com/chirping78/Smoothieware-NG
cd Smoothieware-NG
mbed compile -m NUCLEO_F401RE -t GCC_ARM
```

Or clone the code by yourself and compile by mbed cli:
```
git clone https://github.com/chirping78/Smoothieware-NG
cd Smoothieware-NG
mbed update
mbed compile -m NUCLEO_F401RE -t GCC_ARM
```
