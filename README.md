# RemoteIO

Biblioteca para comunicação entre dispositivos [espressif32](https://www.espressif.com/en/products/socs/esp32) e plataforma em nuvem [NodeIoT](https://nodeiot.app.br/).

Possibilita a leitura de sensores e acionamento de atuadores em tempo real, com visualização de dados e ações de comando via dashboards web/mobile.

## Índice
- [RemoteIO](#remoteio)
  - [Índice](#índice)
  - [Requisitos](#requisitos)
  - [Instalação](#instalação)
    - [Usando PlatformIO](#usando-platformio)
    - [Usando Arduino IDE](#usando-arduino-ide)
  - [Primeiro uso](#primeiro-uso)
  - [Passo a passo](#passo-a-passo)


## Requisitos
- Dispositivo [RemoteIO espressif32](link.pra.algum.lugar).
- [PlatformIO](http://platformio.org) ou [Arduino IDE](https://www.arduino.cc/en/software).
- Conta [NodeIoT](https://nodeiot.app.br/register).
- Última versão estável do [esp32 Arduino core](https://github.com/espressif/arduino-esp32) instalada em sua IDE (PlatformIO ou Arduino IDE).

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

# latest stable version
lib_deps = gkraemer-niot@RemoteIO
```
### Usando Arduino IDE

## Primeiro uso

Com os passos abaixo você poderá fazer a primeira interação de um dispositivo RemoteIO com a plataforma [NodeIoT](https://nodeiot.app.br/). Este é um guia para conectar seu dispositivo RemoteIO pela primeira vez e utilizar as funções predefinidas do módulo.

### Passo a passo

- Registre-se na plataforma [NodeIoT](https://nodeiot.app.br/register).
  
![Registro](https://github.com/user-attachments/assets/a476ef09-7335-486a-adc9-a17bc9648d9e)

- Guarde o "Nome da instituição" definido durante seu registro. Ele será necessário para a configuração inicial do dispositivo RemoteIO.
- Conecte a alimentação em seu dispositivo RemoteIO e ligue-o, conforme manual disponibilizado com o produto.
- Em seu computador, verifique os pontos de acesso Wi-Fi disponíveis e conecte em "RemoteIO". Não é necessário senha.

![Rede](https://github.com/user-attachments/assets/b17ac6fe-5324-402e-8c5a-25606d497fc8)

- Após se conectar ao ponto de acesso, abra o browser de sua preferência (ex. Google Chrome, Mozilla Firefox) e acesse a URL: [http://192.168.4.1/]()
- Na tela de configurações, insira as credenciais (nome e senha) da rede Wi-Fi que será utilizada para conexão do dispositivo. Abaixo, informe o "Nome da instituição" definido por você em seu registro [NodeIoT](https://nodeiot.app.br/register). Atente-se para preencher corretamente as informações acima solicitadas. Por último, crie um nome para identificar o dispositivo dentro da plataforma e clique em Salvar.

![Setup](https://github.com/user-attachments/assets/62c7318c-cf3c-4162-b5c6-3c7955591bfd)

- Desconecte-se do ponto de acesso "RemoteIO" e conecte à rede de sua preferência.
- Acesse sua conta [NodeIoT](https://nodeiot.app.br/).
- Faça a autenticação do seu dispositivo, conforme o [tutorial](site.da.node.tutorial).
- Abra o [dashboard](https://nodeiot.app.br/dashboards) do seu dispositivo e utilize os componentes para interagir com o hardware RemoteIO. 

## Documentação

A [documentação RemoteIO](www) apresenta informações mais detalhadas para uso da ferramenta, onde estão disponíveis guias e exemplos para aprender a trabalhar com as entradas e saídas do dispositivo, integrando o meio físico à núvem para construir a solução ideal para seu projeto.

