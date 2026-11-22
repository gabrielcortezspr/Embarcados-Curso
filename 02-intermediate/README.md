# 02 · Intermediate

Non-blocking timing, data structures, JSON, low-power modes and hardware interrupts. Each file
is a standalone sketch; choose which one to build in [`platformio.ini`](platformio.ini)
(`[activity] file = ...`).

| Sketch | Board | What it shows |
|---|---|---|
| `atividade_01.cpp` | any | Average of 5 numbers read from serial (accumulator pattern) |
| `atividade_02.cpp` | ESP32 | Average of N numbers stored in a `std::vector` |
| `atividade_03.cpp` | any | Mapping a value between two ranges (sensor scaling) |
| `atividade_04.cpp` | any | `ON`/`OFF` text commands over serial |
| `atividade_05.cpp` | any | Blink with `millis()` instead of `delay()` (non-blocking) |
| `atividade_06.cpp` | ESP32 | Receive and send JSON over serial with ArduinoJson |
| `atividade_07.cpp` | any | Numeric serial commands with `switch` |
| `atividade_08.cpp` | ESP32 | Blink 5 times with `do…while`, then **deep sleep** |
| `atividade_09.cpp` | ESP32 | Deep sleep plus reading the **wake-up cause** |
| `atividade_10.cpp` | UNO | **External interrupt**: button on pin 3 toggles an LED |
| `atividade_11.cpp` | UNO | **Timer interrupt** configured through AVR registers |

```bash
pio run -e uno -t upload        # or -e esp32dev
pio device monitor
```
