# 01 · Basics

First steps with Arduino and ESP32: GPIO, the built-in LED, `delay`, serial input/output and
basic control flow. Each file is a standalone sketch; choose which one to build in
[`platformio.ini`](platformio.ini) (`[activity] file = ...`).

| Sketch | Board | What it shows |
|---|---|---|
| `atividade_01.cpp` | UNO | Blink the built-in LED |
| `atividade_02.cpp` | ESP32 | Blink on the ESP32 (LED on GPIO 2) |
| `atividade_03.cpp` | any | Read numbers from serial and do basic arithmetic |
| `atividade_04.cpp` | any | Echo a received character in hexadecimal |
| `atividade_05.cpp` | any | Blink with the interval in a variable |
| `atividade_06.cpp` | any | Blink 10 times with `for` and `while` |
| `atividade_07.cpp` | any | Print a sentence 10 times with `for` and `while` |
| `atividade_08.cpp` | any | Change the blink interval from the serial monitor |
| `atividade_09.cpp` | any | Echo back half of the received string |
| `atividade_10.cpp` | any | Control the LED with serial commands and `switch` |

```bash
pio run -e uno -t upload        # or -e esp32dev
pio device monitor
```
