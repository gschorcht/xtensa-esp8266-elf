# ESP8266 Toolchain for RIOT-OS using the RTOS-SDK

This is a precompiled Xtensa **ESP8266 Toolchain** that was generated with [crosstool-NG](https://github.com/espressif/crosstool-NG.git) and configured for use with _RIOT-OS_ and the _ESP8266-RTOS-SDK v3.x_. In difference to the precompiled toolchain provided by _Espressif_, it has enabled the IOs for C99 formats, long long, floats, and doubles.

**Please note:** This toolchain can only be used for the development version of the [new RIOT-OS port](https://github.com/gschorcht/RIOT-Xtensa-ESP/tree/cpu/esp8266/esp-idf/pr) that uses the _ESP8266 RTOS SDK v3.x_.
It **cannot be used** to compile the [official RIOT-OS port](https://github.com/RIOT-OS/RIOT) that uses the old _ESP8266-NONOS-SDK_. Instead, use the toolchain you can find [here](https://github.com/gschorcht/RIOT-Xtensa-ESP8266-toolchain) for the official RIOT-OS port.

## Installation

To install the toolchain use the following commands:

```
cd /opt/esp
sudo git clone https://github.com/gschorcht/xtensa-lx106-elf
```

After the installation, the components of the toolchain are installed in directory `/opt/esp`. Of course, you can use any other location for the installation, e.g., `/path/to/toolchains` with following commands:

```
cd /path/to/toolchains
sudo git clone https://github.com/gschorcht/xtensa-lx106-elf
```

## Usage

To use the toolchain, you have to add the path of the binaries to your `PATH` variable according to your toolchain location:

```
export PATH=/path/to/toolchains/xtensa-lx106-elf/bin:$PATH
```

For the default installation in `/opt/esp` this would be:

```
export PATH=/opt/esp/xtensa-lx106-elf/bin:$PATH
```

## Copyrights

Please see the given references for the copyrights of the respective owners.

