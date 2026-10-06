# Third-party software in the MS2net firmware

The MS2net firmware and its configuration page include the software listed below. Each component
keeps its copyright and is used under its own licence; the full licence texts are in the
`licenses/` folder next to this file.

## Firmware

| Component | Copyright | Licence |
|---|---|---|
| RTK firmware for ESP32 (base of the MS2net firmware) | SparkFun Electronics | MIT |
| u-blox GNSS v3 library | SparkFun Electronics | MIT |
| MAX1704x fuel gauge library | SparkFun Electronics | MIT |
| Qwiic OLED library (display driver, fonts) | SparkFun Electronics | MIT |
| LIS2DH12 library | SparkFun Electronics | MIT |
| ArduinoJson | Benoît Blanchon | MIT |
| ESP32 BleSerial | Avinab Malla | MIT |
| ESP32Time | Felix Biego | MIT |
| ESP32-OTA-Pull | Mikal Hart | MIT |
| PubSubClient | Nicholas O'Leary | MIT |
| SdFat | Bill Greiman | MIT |
| CRC-24Q | GPSD project | BSD-2-Clause |
| Certificate bundle verification (esp_crt_bundle) | Espressif Systems | Apache-2.0 |
| ESP-IDF, mbedTLS | Espressif Systems, The Mbed TLS Contributors | Apache-2.0 |
| Arduino core for the ESP32, BluetoothSerial | Espressif Systems and contributors | LGPL-2.1 |
| AsyncTCP 1.1.1 (modified) | Hristo Gochkov | LGPL-3.0 |
| ESPAsyncWebServer 1.2.3 | Hristo Gochkov | LGPL-3.0 |

## Configuration page

| Component | Copyright | Licence |
|---|---|---|
| Bootstrap 4.3.1 and 5.0.2 (with Popper) | The Bootstrap Authors, Twitter Inc. | MIT |
| jQuery 3.6.0 | OpenJS Foundation and contributors | MIT |
| Icon font (glyphs from Font Awesome 4) | Dave Gandy | SIL OFL 1.1 |

## LGPL components

The source code of the LGPL components as used in the firmware, including the changes made to
AsyncTCP, is in the `lgpl-sources/` folder. On request, for at least three years from the release
of each firmware version, the object files of the firmware are provided so that it can be relinked
with a modified version of these components.

Requests: open an issue on this repository.
