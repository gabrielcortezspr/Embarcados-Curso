# 03 · IoT

Exchanging structured data between the ESP32, a computer and the cloud. Choose which sketch to
build in [`platformio.ini`](platformio.ini) (`[activity] file = ...`).

## `atividade_01.cpp`: JSON over serial

Receives and sends JSON with ArduinoJson. Open the serial monitor and send:

```json
{"led_state": true}
```

The LED follows the value and the board replies with the same JSON.

## `atividade_02_mqtt.cpp`: MQTT over Wi-Fi

Connects the ESP32 to Wi-Fi and to the public broker `broker.hivemq.com`, publishing and
subscribing on the topic `curso/embarcados/teste`.

1. Set `ssid` and `password` at the top of the file.
2. Set `file = atividade_02_mqtt.cpp` in `platformio.ini` (PubSubClient is already in
   `lib_deps`).
3. Build and upload: `pio run -e esp32dev -t upload`.
4. Use [MQTTX](https://mqttx.app/) or any MQTT client to publish to and subscribe on the topic.
