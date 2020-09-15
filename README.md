# Vorlage
## Inhaltsverzeichnis
1. [x] [Inhaltsverzeichnis](#Inhaltsverzeichnis)
1. [ ] [Beschreibung](#Beschreibung)
   1. [ ] [Leitungen](#Leitungen)
1. [ ] [Hardware](#Hardware)
   1. [ ] [Technische Daten](#technische-daten)
   1. [ ] [Datasheet](#datasheet)
   1. [ ] [PCB](#PCB)
1. [ ] [Software](#Software)
1. [ ] [3D](#3D)
1. [ ] [Where to buy](#Where-to-buy)
1. [ ] [Abbildungen](#Abbildungen)
1. [x] [Credits](#Credits)

## Beschreibung
IC zur Umwandlung von seriellen Signalen zu USB. 
* Kompatibel mit 5V- und 3,3V-Systemen. 
* 2.0 Full-speed device
* Geschwindigkeit 50bps .. 2Mbps
* integrierter 12MHz crystal, kein externer benötigt
* USB-Vendor-class

http://www.wch-ic.com/products/CH340.html
http://www.wch-ic.com/search?q=CH340&t=downloads

### Leitungen
###### Standard für Arduinos
PIN | Name | Beschreibung | TYP
------------ | ------------- | ------------- | -------------
RX | Receive Data | Leitung für eingehende (von DTE zu empfangende) Daten (negative Logik) | I
TX | Transmit Data | Leitung für ausgehende (von DTE gesendete) Daten ([negative Logik](https://de.wikipedia.org/wiki/Negative_Logik)) | O
DTR | Data Terminal Ready | Mit einem High-Pegel an diesem Ausgang signalisiert DTE seine Betriebsbereitschaft an die Gegenstelle. Damit kann die Gegenstelle, z. B. ein Modem, aktiviert oder auch zurückgesetzt werden. Üblicherweise antwortet die Gegenstelle mit einem High-Pegel auf DSR | O

###### Weitere für RS-232
PIN | Name | Beschreibung | TYP
------------ | ------------- | ------------- | -------------
CTS | Clear to Send | Hardware-Handshake, „Sendeerlaubnis“; Ein High-Pegel an diesem Eingang ist ein Signal der Gegenstelle, dass sie Daten von DTE entgegennehmen kann | I
RTS | Request to Send | Hardware-Handshake, „Sendeanforderung“; ein High-Pegel an diesem Ausgang signalisiert, dass DTE Daten senden möchte | O
RTR (n.v.) | Request to Receive | „Empfangsstatus“; ein High-Pegel an diesem Ausgang signalisiert der Gegenstelle, dass DTE bereit ist, Daten zu empfangen | O
DSR | Data Set Ready | Ein High-Pegel an diesem Eingang ist ein Signal der Gegenstelle, dass sie im Prinzip einsatzbereit ist (aber nicht notwendigerweise auch empfangsbereit, siehe CTS) | I
RI | Ring Indicator | Ein High-Pegel an diesem Eingang signalisiert dem DTE-Gerät, dass ein Anruf ankommt, d. h., dass jemand eine Datenverbindung aufbauen will („ring“ ist engl. für „klingeln“; besonders bei Telefonen und im übertragenen Sinne auch bei Modems). Siehe auch [Rufspannung](https://de.wikipedia.org/wiki/Rufspannung). | I
DCD | Data Carrier Detected | Mit einem High-Pegel an diesem Eingang signalisiert die Gegenstelle, dass sie einlaufende Daten auf der Leitung erkennt (dem Namen nach ist das die [Modulationsträger](https://de.wikipedia.org/wiki/Tr%C3%A4ger_(Nachrichtentechnik)-Erkennung) und an DTE weitergeben möchte | I


## Hardware
### Technische Daten
* Modell:Multiplexer/Demultiplexer
* Typ:74HC 4067
* Temperaturbereich:-40 ... +85 °C
* Versorgungsspannung:2,0 ... 10,0 VDC
* Leistung:500 mW
* LCSC Part #: C6525 / C424181 / [C98457](https://lcsc.com/product-detail/Analog-Switches_TI_CD74HC4067SM96_CD74HC4067SM96_C98457.html/?href=jlc-SMT)
* EAN / GTIN: 9900001079047

### Datasheet
* [TI.com datasheet](https://www.ti.com/lit/ds/symlink/cd74hc4067.pdf)
* [snapshot](datasheet/xyz.pdf)
### PCB
## Software
## 3D

## Where to buy
~ 6 EUR for 10pcs: [AliExpress](https://www.aliexpress.com/item/32821800330.html)

## Abbildungen
![Front](images/front.png)
![Back](images/back.png)

## Credits
* :+1: [arduino](https://github.com/arduino)
* :+1: [adafruit](https://github.com/adafruit)
* :+1: [sparkfun](https://github.com/sparkfun)
* :+1: [Watterott](https://github.com/watterott) and @awatterott for great SW, HW and products
* :+1: [atom](https://github.com/atom) 
* :+1: @ikatyang for the [emoji-cheat-sheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)
