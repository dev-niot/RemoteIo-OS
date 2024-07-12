# RemoteIO

Biblioteca para comunicação entre dispositivos espressif32 e plataforma em nuvem [NodeIoT](https://nodeiot.app.br/).

Possibilita a leitura de sensores e acionamento de atuadores em tempo real, com visualização de dados e ações de comando via dashboards web ou mobile.

Requer [ArduinoJson@^7.1.0](https://github.com/bblanchon/ArduinoJson), [WebSockets@^2.4.2](https://github.com/Links2004/arduinoWebSockets) e [ESPAsyncWebServer@^1.2.4](https://github.com/me-no-dev/ESPAsyncWebServer) para funcionar.

Para usar a biblioteca você pode pode precisar, também, da última versão do [ESP32](https://github.com/espressif/arduino-esp32) Arduino Core.

## Índice
- [RemoteIO](#remoteio)
  - [Índice](#índice)
  - [Instalação](#instalação)
    - [Usando PlatformIO](#usando-platformio)
  - [Princípio de operação](#princípio-de-operação)
    - [Classe RemoteIO](#classe-remoteio)
  - [Atributos](#atributos)
  - [Métodos](#métodos)
  - [Primeiro uso](#primeiro-uso)
  - [Passo a passo resumido](#passo-a-passo-resumido)
  - [Passo a passo detalhado](#passo-a-passo-detalhado)

## Instalação

### Usando PlatformIO

[PlatformIO](http://platformio.org) é um ecossistema de código aberto para o desenvolvimento de IoT com sistema de construção multiplataforma, gerenciador de bibliotecas e suporte completo para o desenvolvimento utilizando Espressif ESP8266/ESP32. Funciona nos sistemas operacionais populares: Mac OS X, Windows, Linux 32/64, Linux ARM (como Raspberry Pi, BeagleBone, CubieBoard).

1. Instale o [PlatformIO IDE](http://platformio.org/platformio-ide).
2. Crie um novo projeto usando "PlatformIO Home > New Project".
3. Adicione "RemoteIO" ao projeto usando o [Project Configuration File `platformio.ini`](http://docs.platformio.org/page/projectconf.html) e o parâmetro [lib_deps](http://docs.platformio.org/page/projectconf/section_env_library.html#lib-deps):

```ini
[env:myboard]
platform = espressif32
board = ...
framework = arduino

lib_deps = gkraemer-niot@RemoteIO
```
## Princípio de operação

### Classe RemoteIO

Possibilita a conexão do hardware espressif32 à plataforma [NodeIoT](https://nodeiot.app.br/), associando-o a um dispositivo virtual criado previamente no ecossistema em nuvem. Para isso, a classe RemoteIO abre um ponto de acesso Wi-Fi no dispositivo, ao qual o usuário deve se conectar para acessar a página de configurações e informar a conta e dispositivo NodeIoT, bem como a rede Wi-Fi em que o hardware irá se conectar.

## Atributos
- blahblah : serve pra tal coisa
- pipipi : .....

## Métodos
- fazAlgo() : faz isso isso isso
- desfazAlgo() : ........

## Primeiro uso

Abaixo disponibilizamos em duas versões, uma resumida e outra detalhada em documentação, um exemplo básico para o primeiro contato com a ferramenta [NodeIoT](https://nodeiot.app.br/) utilizando a biblioteca [RemoteIO](link.com.....).

### Passo a passo resumido
- faz isso
- faz aquilo
- cria conta na node
- like no insta
- faz assado

### Passo a passo detalhado
- link pra documentação detalhada com imagens...

