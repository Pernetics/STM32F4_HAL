# STM32F4_HAL
STM32F4 Family Hardware Abstraction Layer (HAL) Library

This library is a fork of the ST [STM32CubeF4](http://www.st.com/web/en/catalog/tools/PF259243) v1.3.0 distribution.

The recommended toolchain is: [Linary GNU Tools for ARM Embedded Processors](https://launchpad.net/gcc-arm-embedded)

Build instructions:

```sh
./autogen.sh
mkdir build ; cd build
../configure --host=arm-none-eabi
make
```

The default target processor is the STM32F439xx.  This can be overriden by specifying an alternate TARGET when running the configure script.  For example:

```sh
../configure --host=arm-none-eabi TARGET=STM32F407xx
```

The default high speed external clock source (HSE) is set to 8 MHz.  This can be overriden by specifying an alternalte HSE_VALUE.  For example:

```sh
../configure --host=arm-none-eabi HSE_VALUE=25000000
```
