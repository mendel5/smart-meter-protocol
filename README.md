# smart-meter-protocol
Information about smart meters and the protocol they use to transmit information

Smart Meter Language (SML),
Object Identification System (OBIS)

## Tasmota
In der Tasmota-Konsole unter http://192.168.178.xxx/cs? den Befehl "`sensor53 d1`" eingeben um die Rohdaten zu sehen.
## Protocol information

### EMH eHZ Generation P
````
----------------------------------------

010060320101
01 00 60 32 01 01
Hersteller-Kennung

0100600100ff
01 00 60 01 00 ff
Geräte-Identifikation

----------------------------------------
````

Die restlichen Werte sollten identisch sein zum `EMH eHZ Generation K`.

### EMH eHZ Generation K
```
----------------------------------------

77078181c78203ff
77 07 81 81 c7 82 03 ff
Hersteller-Kennung

77070100000009ff
77 07 01 00 00 00 09 ff
Geräte-Identifikation

----------------------------------------

77070100010800ff
77 07 01 00 01 08 00 ff
Zählwerk, positive Wirkenergie, tariflos
Total consumption

77070100010801ff
77 07 01 00 01 08 01 ff
Zählwerk, positive Wirkenergie, Tarif 1
Total consumption, tariff 1

77070100010802ff
77 07 01 00 01 08 02 ff
Zählwerk, positive Wirkenergie, Tarif 2
Total consumption, tariff 2

----------------------------------------

77070100020800ff
77 07 01 00 02 08 00 ff
Zählwerk, negative Wirkenergie, tariflos
Total feed-in

77070100020801ff
77 07 01 00 02 08 01 ff
Zählwerk, negative Wirkenergie, Tarif 1
Total feed-in, tariff 1

77070100020802ff
77 07 01 00 02 08 02 ff
Zählwerk, negative Wirkenergie, Tarif 2
Total feed-in, tariff 2

----------------------------------------

77070100100700ff
77 07 01 00 10 07 00 ff
Aktuelle positive Wirkleistung / Aktuelle Momentanwirkleistung
(wird eventuell nur beim vollständigen Datensatz angezeigt)
Power

----------------------------------------

77078181c78205ff
77 07 81 81 c7 82 05 ff
Public Key

----------------------------------------
```

### Apator
```
----------------------------------------

77070100240700ff, 77 07 01 00 24 07 00 ff, Power L1
77070100380700ff, 77 07 01 00 38 07 00 ff, Power L2
770701004c0700ff, 77 07 01 00 4c 07 00 ff, Power L3

----------------------------------------

77070100200700ff, 77 07 01 00 20 07 00 ff, Voltage L1, Volt
77070100340700ff, 77 07 01 00 34 07 00 ff, Voltage L2, Volt
77070100480700ff, 77 07 01 00 48 07 00 ff, Voltage L3, Volt

----------------------------------------

770701001f0700ff, 77 07 01 00 1f 07 00 ff, Current L1, Ampere
77070100330700ff, 77 07 01 00 33 07 00 ff, Current L2, Ampere
77070100470700ff, 77 07 01 00 47 07 00 ff, Current L3, Ampere

----------------------------------------

770701000e0700ff, 77 07 01 00 0e 07 00 ff, Frequency, Hz

----------------------------------------
```

## Links
- https://hessburg.de/tasmota-wifi-smartmeter-konfigurieren/
- https://hessburg.de/tasmota-smartmeter-faq/
- https://www.msxfaq.de/sonst/bastelbude/smartmeter_d0_sml_protokoll.htm
- https://www.msxfaq.de/sonst/bastelbude/smartmeter_d0_sml.htm
- https://de.wikipedia.org/wiki/OBIS-Kennzahlen
- https://github.com/tasmota/docs/blob/master/docs/Smart-Meter-Interface.md
- https://tasmota.github.io/docs/Smart-Meter-Interface/
