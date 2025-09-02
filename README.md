<div align="center">
	<h1>Curso de Embarcados: ESP32 & Arduino</h1>
	<img src="https://platformio.org/images/platformio-logo.svg" alt="PlatformIO" width="120"/>
	<br/>
	<b>Repositório oficial do curso de embarcados para iniciantes e intermediários</b>
</div>

---

## Como criar seu próprio projeto no PlatformIO (VS Code)

1. Instale o [VS Code](https://code.visualstudio.com/) e a extensão [PlatformIO IDE](https://platformio.org/install/ide?install=vscode)
2. Abra o VS Code e clique no ícone do PlatformIO (formato de formiga) na barra lateral
3. Clique em "New Project"
4. Dê um nome ao projeto, escolha a placa (ex: Arduino Uno, ESP32 DevKit, etc) e o framework (Arduino)
5. Clique em "Finish" e aguarde a criação do projeto
6. Coloque seus códigos na pasta `src/` do projeto criado
7. Para compilar e enviar para a placa, use os botões de "Build" (martelo) e "Upload" (seta para a direita) na barra inferior do PlatformIO
8. As Dependências dos códigos devem ser instaladas pelo próprio PlatformIO

---

## Sobre este repositório

Aqui você encontra três projetos independentes, cada um com vários exemplos práticos:

- **basico/** — Exemplos para quem está começando: piscar LED, leitura serial, lógica básica, laços, etc.
- **intermediario/** — Exercícios com lógica mais avançada, uso de funções, comunicação serial, interrupções, timers, etc.
- **iot/** — Exemplos de comunicação, IoT, uso de JSON, integração com brokers, etc.

Cada pasta é um projeto PlatformIO pronto para abrir no VS Code. Basta abrir a pasta desejada, selecionar o ambiente correto no `platformio.ini` e compilar qualquer arquivo da pasta `src/`.

Todos os códigos estão comentados por blocos para facilitar o entendimento.

---

## Ferramentas recomendadas

- [WOKWi](https://wokwi.com/) — Simulador online de Arduino e ESP32
- [TINKERCAD](https://www.tinkercad.com/) — Simulador de circuitos e prototipagem
- [VS Code](https://code.visualstudio.com/) — Editor de código recomendado
- [PlatformIO](https://platformio.org/) — Ambiente de desenvolvimento para embarcados
- [Fritzing](https://fritzing.org/) — Criação de diagramas eletrônicos
- [MQTTX](https://mqttx.app/) — Cliente MQTT para testes de IoT
- [Hercules](https://www.hw-group.com/software/hercules-setup-utility) — Terminal serial e TCP/UDP
- [Bluetooth Terminal](https://play.google.com/store/apps/details?id=de.kai_morich.serial_bluetooth_terminal&hl=pt_BR) — App Android para comunicação Bluetooth
- [ScannerBLE (Conectar&Notificar)](https://play.google.com/store/apps/details?id=com.macdom.ble.blescanner&hl=pt_BR) — App Android para BLE
- [Insomnia](https://insomnia.rest/download) — Testes de APIs REST
- [Mosquitto Broker](https://mosquitto.org/) — Broker MQTT open source

---

## Dúvidas ou sugestões?

Abra uma issue ou envie um pull request!
