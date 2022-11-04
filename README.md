
[![Arduino CI](https://github.com/RobTillaart/FastShiftInOut/workflows/Arduino%20CI/badge.svg)](https://github.com/marketplace/actions/arduino_ci)
[![Arduino-lint](https://github.com/RobTillaart/FastShiftInOut/actions/workflows/arduino-lint.yml/badge.svg)](https://github.com/RobTillaart/FastShiftInOut/actions/workflows/arduino-lint.yml)
[![JSON check](https://github.com/RobTillaart/FastShiftInOut/actions/workflows/jsoncheck.yml/badge.svg)](https://github.com/RobTillaart/FastShiftInOut/actions/workflows/jsoncheck.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/RobTillaart/FastShiftInOut/blob/master/LICENSE)
[![GitHub release](https://img.shields.io/github/release/RobTillaart/FastShiftInOut.svg?maxAge=3600)](https://github.com/RobTillaart/FastShiftInOut/releases)


# FastShiftInOut

Arduino library for (AVR) optimized shiftInOut (simultaneously).

A library for FastShiftIn only - https://github.com/RobTillaart/FastShiftIn
A library for FastShiftOut only - https://github.com/RobTillaart/FastShiftOut


## Description

FastShiftInOut is a class that can send and receive bytes simultaneously.
In that sense it mimics a SPI bus.

VERY experimental.


## Performance

TODO


## Interface

 //  bitOrder = { LSBFIRST, MSBFIRST };
- **FastShiftInOut(uint8_t dataIn, uint8_t dataOut, uint8_t clockPin, uint8_t bitOrder = LSBFIRST)**
- **uint8_t write(uint8_t data)** reads and writes simultaneously.
- **uint8_t lastWritten(void)** returns last written value.
- **bool setBitOrder(uint8_t bitOrder)** idem.
- **uint8_t getBitOrder(void)** idem.
- **uint8_t writeLSBFIRST(uint8_t data)** slightly optimized version.
- **uint8_t writeMSBFIRST(uint8_t data)**


## Notes



## Operation

See examples


## Future

#### must
- documentation
- get functional complete

#### should
- performance measurements
- optimize for AVR

#### could
- **void ignoreRead()**
- add Print interface?


