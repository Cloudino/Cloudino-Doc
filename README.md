Welcome to Cloudino Documentation!
===================

<img src="https://github.com/Cloudino/Cloudino-Doc/raw/master/Cloudino_logo.png" width="300" align="left">

Cloudino is a Full Stack Internet of Things Platform, Open Source and Open Hardware, that allows the development and instrumentation of Internet of the Things Solutions in a Simple and Transparent way.

The Cloudino Platform was designed thinking in 4 main characteristics: small size, easy to use, low cost hardware and modularity. And with these characteristics, that the Cloudino platform allows to everyone the possibility to incorporate IoT technologies in their projects without any technical or economical limitations.

![Cloudino Characteristics](https://github.com/Cloudino/Cloudino-Doc/raw/master/Cloudino_characteristics.png)

Cloudino is developed and maintained by INFOTEC (Public Research Center of CONACYT) as a Open Source and Open Hardware Platform

## Cloudino Architecture

The Cloudino Platform proposes to add a new IoT Chip (Cloudino WiFi Connector) that works like a configurable Network Layer between the sensors, actuators or existent hardware solutions like Arduino and the Cloud Services, for a simple and fast start to IoT World.

![Cloudino Architecture](https://github.com/Cloudino/Cloudino-Doc/raw/master/Cloudino_Achitecture.png)

You can find more information about Cloudino Architecture [here](https://github.com/Cloudino/Cloudino-Doc/wiki/Cloudino-Arquitecture)

## Cloudino WiFi Connector

The **Cloudino WiFi Connector**, which is a little, inexpensive and powerful IoT Chip, that **has preprogrammed** the most common IoT protocols like a **MQTT** or the **NGSI** for the Orion Context Broker, that allows everyone to start sending information to the Cloud without any additional programming effort.

![Cloudino WCC](https://github.com/Cloudino/Cloudino-Doc/raw/master/Cloudino.png)

### Technical Specifications
Microcontroller |	ESP8266
Operating Voltage |	4V - 12V
Digital I/O Pins |	11
Analog Input Pins |	1 (Max input: 1V)
Clock Speed |	80MHz/160MHz
Flash |	4M bytes
Length | 25mm
Width |	25.6mm
Weight | 3g

### Pins

CWC Pin | Function | | CWC Pin | Function
--- | --- | --- | --- | ---
VCC | OUT 3.3V | | GPIO13 | IO, MOSI
RST	| Reset | | GPIO12 | IO, MISO
GND | Ground | | GPIO14 | IO, SCK
GND | Ground | | GPIO16 | IO
VIN	| IN 4V - 12V | | ADC | 10-bit Analog Input, Max 1V Input
TXD	| TXD | | GPIO2	| IO, 10k Pull-Up, BUILTIN_LED
RXD	| RXD | | GPIO0	| IO, 10k Pull-Up
GPIO5	| IO, SCL | | GPIO4	| IO, SDA

We can see the **Cloudino WiFi Connector** as an **IoT Router**, where let us configure using a simple web browser, the internet settings as well as the IoT protocol that the chip will use.

An other important characteristic of the **Cloudino WiFi Connector** is that can **working in parallel with the Arduino**, the WCC can be used as an **Cloudino WiFi Connector**, I mean, we can reprogram the Arduino via Cloud.

The **Cloudino WiFi Connector** working with Arduino is not like an Arduino shield, is an other processor working in parallel dedicated only to the network layer including the IoT protocols, leaving the Arduino dedicated to the connectivity with the sensors and actuators, while allowing reprogramming Arduino via WiFi or Cloud.

The **Cloudino WiFi Connector** can be used as we mention as an **additional microcontroller dedicated to the network layer, working in parallel with actual microcontroller solutions like arduino**. But also can be used as a **Standalone device** for directly communicate the real-life objects to the internet.  

You can find more information about Cloudino Wifi Connector [here](https://github.com/Cloudino/Cloudino-Doc/wiki/Cloudino-WiFi-Connector)

If you want to make your own Cloudino Module you can start with:
* [Cloudino Connector Squema](https://github.com/Cloudino/Cloudino-Doc/wiki/Cloudino-WiFI-Connector-Schema)
* [Make your first Cloudino](https://github.com/Cloudino/Cloudino-Doc/wiki/Make-your-first-Cloudino)

## Cloudino Standalone

To start with the WiFi Cloud connector in Standalone mode you only need to connect it to a power supply between 4v and 15v.

![Cloudino SA](https://github.com/Cloudino/Cloudino-Doc/raw/master/Squema_Cloudino_SA_9V.png)

The WiFi Cloud Connector sets up a network of its own, allowing the user to connect directly to it for an easy and fast configuration through a web browser [http://192.168.4.1](http://192.168.4.1)

![Cloudino WCC](https://github.com/Cloudino/Cloudino-Doc/raw/master/Cloudino_WCC_Config_2.png)

You can find more information about Cloudino WiFi Connector Configuration [here](https://github.com/Cloudino/Cloudino-Doc/wiki/Cloudino-WiFi-Connector-Configuration)

## Cloudino with Arduino

**Cloudino** can be work in **parallel with Arduino** using it like an **Arduino Cloud Programmer**.

For this you only need to use tree ping from the Arduino (TX, TX , RST) and the additional (5V, GND)

![Arduino_connection](https://github.com/Cloudino/Cloudino-Doc/raw/master/Squema_Cloudino_Ard_V2.png)

You can find more information about Arduino Connection Squema [here](https://github.com/Cloudino/Cloudino-Doc/wiki/Cloudino-with-Arduino-Connection-Squema)

### Supported Devices
* The Arduino Uno
* Arduino Duemilanove or Diecimila
* Arduino Nano
* ATmega1280
* Arduino Mini
* Arduino Fio
* Arduino BT
* LilyPad Arduino
* Arduino Pro or Pro Mini
* Arduino NG or older

### Arduino library

* [Cloudino Library for Arduino](https://github.com/Cloudino/Cloudino-Doc/wiki/Cloudino-Library-for-Arduino)
* [Github Arduino Library](https://github.com/Cloudino/Cloudino-ArduinoLib)

## Cloudino with Javascript
CloudinoJS is a JavaScript implementation por Cloudino Platform

* [CloudinoJS Examples](https://github.com/Cloudino/Cloudino-Doc/wiki/CloudinoJS-Examples)
* [CloudinoJS Language Reference](https://github.com/Cloudino/Cloudino-Doc/wiki/CloudinoJS-Language-Reference)

## Cloudino Server

The use of the Cloudino Server is optional, however, it has many advantages over existing services, such as: Devices, Rules and User Contexts Manages, and Stream Data Storage.

The Cloudino Server includes also Web IDE that allows devices to be programmed and debugged via Cloud and it also includes an easy "Blocks programming interface" for non-experimented programmers.

![Cloudino Server](https://github.com/Cloudino/Cloudino-Doc/raw/master/Cloudino_Server.png)

For start using the Cloudino Server visit [http://cloudino.io/panel](http://cloudino.io/panel)



