# AppleTV
Mit diesem Modul ist es möglich einen Apple TV mithilfen des NodeJS Tool (https://github.com/sebbo2002/atv2mqtt) über MQTT in IP-Symcon zu integrieren.

### Inhaltsverzeichnis

1. [Funktionsumfang](#1-funktionsumfang)
2. [Voraussetzungen](#2-voraussetzungen)
3. [Einrichten der Instanzen in IP-Symcon](#4-einrichten-der-instanzen-in-ip-symcon)
4. [Statusvariablen und Profile](#5-statusvariablen-und-profile)
5. [WebFront](#6-webfront)
6. [PHP-Befehlsreferenz](#7-php-befehlsreferenz)

### 1. Funktionsumfang

* Status aktueller Wiedergabe
* Steuerung des Apple TV

### 2. Vorraussetzungen

- IP-Symcon ab Version 5.1

### 3. Einrichten der Instanzen in IP-Symcon

 Unter 'Instanz hinzufügen' ist das 'AppleTV'-Modul unter dem Hersteller 'Apple' aufgeführt.

__Konfigurationsseite__:

Name     | Beschreibung
-------- | ------------------
MQTT Topic | Topic des ATV2MQTT Moduls, in der Konfigurations Datei von ATV2MQTT zu finden

### 4. Statusvariablen und Profile

Die Statusvariablen/Kategorien werden automatisch angelegt. Das Löschen einzelner kann zu Fehlfunktionen führen.

#### Statusvariablen

Name   | Typ     | Beschreibung
------ | ------- | ------------
Name|String| Name des Apple TVs
IP-Adresse|String| IP-Adresse des Apple TVs
Status|String| Aktueller Status Apple TVs
Steuerung|Integer| Variable zum bedienen des Apple TVs
Dauer|Integer| Dauer der aktuellen Wiedergabe
Verstrichene Zeit|Integer| Verstrichene Zeit der aktuellen Wiedergabe
Artist|String| Aktueller Künstler der Wiedergabe
Titel|String| Aktueller Title der Wiedergabe
Album|String| Aktuelles Album der Wiedergabe
App|String| Aktuelle App
AppBundleIdentifier|String| AppBundleIdentifier
Timestamp|Integer|Aktueller Timestamp

#### Profile

Name   | Typ
------ | -------
ATV.Controls|Integer

### 5. WebFront

Anzeige und Steuerung des Apple TVs.

### 6. PHP-Befehlsreferenz

`RequestAction(integer $VariablenID, $Value);`
Schalten der Variable.

Beispiel:
 Variable Steuerung = 12345
 AppleTV in Standby versetzen
`RequestAction(12345, 10);`