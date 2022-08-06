# Common API

## Objective

The objective is to define a common set of APIs for ESP32 chips.

## Which platforms are taken into account for comparison?

- Arduino
- Rust (Embedded Hell)
- NuttX
- Zephyr
- MicroPython
- CircuitPython
- NanoFramework (https://docs.nanoframework.net/api/index.html)
- Toit
- NodeMCU
- ESP C++ API

## What APIs are covered by WASI?

    https://wasi.dev


    - APIs for host filesystems, network stacks, and other resources.
    - APIs for graphics, audio, input devices
    - APIs for encryption, format conversion, and other transformations (particularly where hardware acceleration may be available on some platforms)


## API Comparison


|Group                                                 |Original C                                 |XX|XX|XX|
|------------------------------------------------------|-------------------------------------------|--|--|--|
|**Application Protocols**                             |                                           |  |  |  |
|ASIO port                                             |                                           |  |  |  |
|ESP-Modbus                                            |                                           |  |  |  |
|ESP-MQTT                                              |                                           |  |  |  |
|ESP-TLS                                               |                                           |  |  |  |
|ESP HTTP Client                                       |                                           |  |  |  |
|ESP Local Control                                     |                                           |  |  |  |
|ESP Serial Slave Link                                 |                                           |  |  |  |
|ESP x509 Certificate Bundle                           |                                           |  |  |  |
|HTTP Server                                           |                                           |  |  |  |
|HTTPS server                                          |                                           |  |  |  |
|ICMP Echo                                             |                                           |  |  |  |
|mDNS Service                                          |                                           |  |  |  |
|Mbed TLS                                              |                                           |  |  |  |
|IP Network Layer                                      |                                           |  |  |  |
|                                                      |                                           |  |  |  |
|**Bluetooth API**                                     |                                           |  |  |  |
|BT COMMON                                             |                                           |  |  |  |
|BT LE                                                 |                                           |  |  |  |
|CLASSIC BT                                            |                                           |  |  |  |
|Controller && VHCI                                    |                                           |  |  |  |
|ESP-BLE-MESH                                          |                                           |  |  |  |
|NimBLE-based host APIs                                |                                           |  |  |  |
|                                                      |                                           |  |  |  |
|**Error Codes Reference**                             |                                           |  |  |  |
|                                                      |                                           |  |  |  |
|**Networking APIs**                                   |                                           |  |  |  |
|Wi-Fi                                                 |                                           |  |  |  |
|Ethernet                                              |                                           |  |  |  |
|Thread                                                |                                           |  |  |  |
|ESP-NETIF                                             |                                           |  |  |  |
|IP Network Layer                                      |                                           |  |  |  |
|Application Layer                                     |                                           |  |  |  |
|                                                      |                                           |  |  |  |
|**Peripherals API**|                                  |                                           |  |  |  |
|Analog to Digital Converter (ADC)                     |                                           |  |  |  |
|Digital To Analog Converter (DAC)                     |                                           |  |  |  |
|GPIO & RTC GPIO                                       |                                           |  |  |  |
|General Purpose Timer (GPTimer)                       |                                           |  |  |  |
|Inter-Integrated Circuit (I2C)                        |                                           |  |  |  |
|Inter-IC Sound (I2S)                                  |                                           |  |  |  |
|LCD                                                   |                                           |  |  |  |
|LED Control (LEDC)                                    |                                           |  |  |  |
|Motor Control Pulse Width Modulator (MCPWM)           |                                           |  |  |  |
|Pulse Counter (PCNT)                                  |                                           |  |  |  |
|Remote Control (RMT)                                  |                                           |  |  |  |
|SD Pull-up Requirements                               |                                           |  |  |  |
|SDMMC Host Driver                                     |                                           |  |  |  |
|SD SPI Host Driver                                    |                                           |  |  |  |
|SDIO Card Slave Driver                                |                                           |  |  |  |
|Sigma-delta Modulation                                |                                           |  |  |  |
|SPI Master Driver                                     |                                           |  |  |  |
|SPI Slave Driver                                      |                                           |  |  |  |
|ESP32-WROOM-32SE (Secure Element)                     |                                           |  |  |  |
|Touch Sensor                                          |                                           |  |  |  |
|Two-Wire Automotive Interface (TWAI)                  |                                           |  |  |  |
|Universal Asynchronous Receiver/Transmitter (UART)    |                                           |  |  |  |
|                                                      |                                           |  |  |  |
|**Project Configuration**                             |                                           |  |  |  |
|Introduction                                          |                                           |  |  |  |
|Project Configuration Menu                            |                                           |  |  |  |
|Using sdkconfig.defaults                              |                                           |  |  |  |
|Kconfig Formatting Rules                              |                                           |  |  |  |
|Backward Compatibility of Kconfig Options             |                                           |  |  |  |
|Configuration Options Reference                       |                                           |  |  |  |
|                                                      |                                           |  |  |  |
|**Provisioning API**                                  |                                           |  |  |  |
|Protocol Communication                                |                                           |  |  |  |
|Unified Provisioning                                  |                                           |  |  |  |
|Wi-Fi Provisioning                                    |                                           |  |  |  |
|SmartConfig                                           |                                           |  |  |  |
|Wi-Fi Easy ConnectTM (DPP)                            |                                           |  |  |  |
|                                                      |                                           |  |  |  |
|**Storage API**                                       |                                           |  |  |  |
|FAT Filesystem Support                                |                                           |  |  |  |
|Manufacturing Utility                                 |                                           |  |  |  |
|Non-volatile storage library                          |                                           |  |  |  |
|NVS Partition Generator Utility                       |                                           |  |  |  |
|SD/SDIO/MMC Driver                                    |                                           |  |  |  |
|SPI Flash API                                         |                                           |  |  |  |
|SPIFFS Filesystem                                     |                                           |  |  |  |
|Virtual filesystem component                          |                                           |  |  |  |
|Wear Levelling API                                    |                                           |  |  |  |
|                                                      |                                           |  |  |  |
|**System API**                                        |                                           |  |  |  |
|App Image Format                                      |                                           |  |  |  |
|Application Level Tracing                             |                                           |  |  |  |
|Call function with external stack                     |                                           |  |  |  |
|Console                                               |                                           |  |  |  |
|eFuse Manager                                         |                                           |  |  |  |
|Error Codes and Helper Functions                      |                                           |  |  |  |
|ESP HTTPS OTA                                         |                                           |  |  |  |
|Event Loop Library                                    |                                           |  |  |  |
|FreeRTOS                                              |                                           |  |  |  |
|FreeRTOS Supplemental Features                        |                                           |  |  |  |
|Heap Memory Allocation                                |                                           |  |  |  |
|Heap Memory Debugging                                 |                                           |  |  |  |
|High Resolution Timer                                 |                                           |  |  |  |
|Internal and Unstable APIs                            |                                           |  |  |  |
|Inter-Processor Call                                  |                                           |  |  |  |
|Interrupt allocation                                  |                                           |  |  |  |
|Logging library                                       |                                           |  |  |  |
|Miscellaneous System APIs                             |                                           |  |  |  |
|Over The Air Updates (OTA)                            |                                           |  |  |  |
|Performance Monitor                                   |                                           |  |  |  |
|Power Management                                      |                                           |  |  |  |
|POSIX Threads Support                                 |                                           |  |  |  |
|Random Number Generation                              |                                           |  |  |  |
|Sleep Modes                                           |                                           |  |  |  |
|SoC Capabilities                                      |                                           |  |  |  |
|System Time                                           |                                           |  |  |  |
|The himem allocation API                              |                                           |  |  |  |
|ULP Coprocessor programming                           |                                           |  |  |  |
|Watchdogs                                             |                                           |  |  |  |


# References

## Arduino

https://www.arduino.cc/reference/en/

https://docs.espressif.com/projects/arduino-esp32/en/latest/libraries.html


## Zephyr

https://github.com/zephyrproject-rtos/zephyr/issues/29394

