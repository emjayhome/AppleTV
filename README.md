[![Version](https://img.shields.io/badge/Symcon-PHPModul-red.svg)](https://www.symcon.de/service/dokumentation/entwicklerbereich/sdk-tools/sdk-php/)
![Version](https://img.shields.io/badge/Symcon%20Version-5.1%20%3E-blue.svg)
[![License](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-green.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![Check Style](https://github.com/Schnittcher/AppleTV/workflows/Check%20Style/badge.svg)](https://github.com/Schnittcher/AppleTV/actions)

# AppleTV
   Mit diesem Modul ist es möglich einen Apple TV mithilfe des NodeJS Tool (https://github.com/sebbo2002/atv2mqtt) über MQTT in IP-Symcon zu integrieren.
 
   ## Inhaltverzeichnis
   1. [Voraussetzungen](#1-voraussetzungen)
   2. [Enthaltene Module](#2-enthaltene-module)
   3. [Installation](#3-installation)
   4. [Konfiguration in IP-Symcon](#4-konfiguration-in-ip-symcon)
   5. [Spenden](#5-spenden)
   6. [Sonsriges](#6-sonstiges)
   7. [Lizenz](#7-lizenz)
   
## 1. Voraussetzungen

* mindestens IPS Version 5.1
* ATV2MQTT (https://github.com/sebbo2002/atv2mqtt)
* MQTT Server oder MQTT Client

## 2. Enthaltene Module

* [AppleTV](AppleTV/README.md)

## 3. Installation
Installation über den IP-Symcon Module Store.
Die Installation von ATV2MQTT ist hier beschrieben: https://github.com/sebbo2002/atv2mqtt/blob/master/README.md

## 4. Konfiguration in IP-Symcon
Das Modul kann mit dem internen MQTT Server betrieben werden, oder aber mit einem externen MQTT Broker.
Wenn ein externer MQTT Broker verwendet werden soll, dann muss aus dem Module Store der MQTTClient installiert werden.

Standardmäßig wird der MQTT Server bei den Geräteinstanzen als Parent hinterlegt, wenn aber ein externer Broker verwendet werden soll, muss der MQTT Client per Hand angelegt werden und in der Geräteinstanz unter "Gateway ändern" ausgewählt werden.

Die weitere Dokumentation bitte den einzelnen Modulen entnehmen.

## 5. Spenden

Dieses Modul ist für die nicht kommzerielle Nutzung kostenlos, Schenkungen als Unterstützung für den Autor werden hier akzeptiert:    

<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=EK4JRP87XLSHW" target="_blank"><img src="https://www.paypalobjects.com/de_DE/DE/i/btn/btn_donate_LG.gif" border="0" /></a>

## 6. Sonstiges
Vielen Dank an [sebbo2002](https://github.com/sebbo2002) für das Bereitstelle von [ATV2MQTT](https://github.com/sebbo2002/atv2mqtt)

## 7. Lizenz

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)