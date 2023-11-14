# smart-meter-protocol
Information about smart meters and the protocol they use to transmit information

Smart Meter Language (SML),
Object Identification System (OBIS)

## Protocol information
In der Tasmota-Konsole unter http://192.168.178.xxx/cs? den Befehl "`sensor53 d1`" eingeben um die Rohdaten zu sehen.

```
77078181c78203ff
77 07 81 81 c7 82 03 ff
Hersteller-Kennung

77070100000009ff
77 07 01 00 00 00 09 ff
Geräte-Identifikation

77070100010800ff
77 07 01 00 01 08 00 ff
Zählwerk, positive Wirkenergie, Tariflos

77070100010801ff
77 07 01 00 01 08 01 ff
Zählwerk, positive Wirkenergie, Tarif 1

77070100010802ff
77 07 01 00 01 08 02 ff
Zählwerk, positive Wirkenergie, Tarif 2

77070100100700ff
77 07 01 00 10 07 00 ff
Aktuelle positive Wirkleistung

77078181c78205ff
77 07 81 81 c7 82 05 ff
Public Key
```

## Links
- https://hessburg.de/tasmota-wifi-smartmeter-konfigurieren/
- https://hessburg.de/tasmota-smartmeter-faq/
- https://www.msxfaq.de/sonst/bastelbude/smartmeter_d0_sml_protokoll.htm
- https://www.msxfaq.de/sonst/bastelbude/smartmeter_d0_sml.htm
- https://de.wikipedia.org/wiki/OBIS-Kennzahlen
