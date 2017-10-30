# Nucleo F401RE

Per datasheet of STM32F401xE, the USB pins are

```
PA9  - OTG_FS_VBUS
PA11 - OTG_FS_DM
PA12 - OTG_FS_DP
```

# Backlog

Compiling failed with USB libraries. See this [mbed-os issue](https://github.com/ARMmbed/mbed-os/issues/3335).

```
mbed compile -m NUCLEO_F401RE -t GCC_ARM --source . --source mbed-os/features/unsupported/USBDevice
```
