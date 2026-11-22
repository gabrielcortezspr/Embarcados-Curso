# Embedded Systems Course: ESP32 & Arduino

![C++](https://img.shields.io/badge/C%2B%2B-Arduino-00979D?logo=arduino&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-Espressif-E7352C?logo=espressif&logoColor=white)
![PlatformIO](https://img.shields.io/badge/PlatformIO-build-F5822A?logo=platformio&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green)

Hands-on material for an introductory embedded systems course I put together: **23 commented
sketches** for Arduino UNO and ESP32, going from blinking an LED to interrupts, deep sleep,
JSON and MQTT.

| Module | Sketches | Topics |
|---|---|---|
| [`01-basics`](01-basics) | 10 | GPIO, `delay`, serial I/O, loops, `switch` |
| [`02-intermediate`](02-intermediate) | 11 | `millis()` non-blocking timing, `std::vector`, value mapping, ArduinoJson, ESP32 deep sleep and wake-up causes, external and timer interrupts (AVR registers) |
| [`03-iot`](03-iot) | 2 | JSON over serial, MQTT over Wi-Fi with PubSubClient |

Code comments are in Portuguese, written for students.

## Getting started

Each module is a [PlatformIO](https://platformio.org/) project with `uno` and/or `esp32dev`
environments. Every file in `src/` is a standalone sketch, so the project compiles one at a
time; choose it in the module's `platformio.ini`:

```ini
[activity]
file = atividade_05.cpp
```

Then build, upload and open the serial monitor (or use the PlatformIO buttons in VS Code):

```bash
cd 02-intermediate
pio run -e esp32dev -t upload
pio device monitor
```

No hardware? Most sketches run in the [Wokwi](https://wokwi.com/) simulator.

## Recommended tools

| Tool | Use |
|---|---|
| [VS Code](https://code.visualstudio.com/) + [PlatformIO IDE](https://platformio.org/install/ide?install=vscode) | Editor, build and upload |
| [Wokwi](https://wokwi.com/) / [Tinkercad](https://www.tinkercad.com/) | Online Arduino/ESP32 and circuit simulators |
| [Fritzing](https://fritzing.org/) | Wiring diagrams |
| [MQTTX](https://mqttx.app/) / [Mosquitto](https://mosquitto.org/) | MQTT client and broker |
| [Hercules](https://www.hw-group.com/software/hercules-setup-utility) | Serial and TCP/UDP terminal |
| [Insomnia](https://insomnia.rest/download) | REST API testing |
| [Serial Bluetooth Terminal](https://play.google.com/store/apps/details?id=de.kai_morich.serial_bluetooth_terminal) / [BLE Scanner](https://play.google.com/store/apps/details?id=com.macdom.ble.blescanner) | Bluetooth and BLE from an Android phone |

## License

[MIT](LICENSE)
