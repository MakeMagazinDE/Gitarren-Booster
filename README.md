![GitHub Logo](http://www.heise.de/make/icons/make_logo.png)

Maker Media GmbH

***

![Picture](https://github.com/MakeMagazinDE/Gitarren-Booster/blob/main/aufm_gh.JPG) 

# Gitarren-Booster

### Stompbox für Pegelanpassung im Effekte-Rig

Der Gitarrist mag Booster. Das sind Vorverstärker, mit denen er seinem Verstärker Dampf machen kann, dass die Röhren röhren! Aber ein Booster vermag auch einfach nur unterschiedliche Gitarren- oder Effektgerätepegel auszugleichen. Unser Bauvorschlag kann über ein einziges Poti als Bedienelement sowohl verstärken als auch abschwächen.

### Dateien:

* booster_03.zip - Gerber-Dateien für Platinenfertigung
* booster_03 - Schematic.pdf - Aktualisierter Schaltplan
* booster_03 - PCB.pdf - Aktualisierter Bestückungsplan

### Stückliste
```
U1 - TL072, OPA2134, TS912, LF412 oder ähnlich
D1 - 1N4004 oder 1N4007
C1, C4 - 100n     
C2, C3-100µ 16V         
C5 - 220p       
C6 - 22n 63V (Folie)      
C7 - 470n 63V (Folie)      
C8 - 47p       
R1 - 100R       
R2, R3 - 47k       
R4- -1M       
R5 - 10k       
R6, R7, R9 - 100k      
R8 - 100k Poti lin.
R10 - 220R      
R11 - 2M2      
R12, R13 - 10k       
``` 
Alle Widerstände 1/4W Metallfilm

### Messwerte

Ermittelt mit Rohde&Schwarz Audio Analyzer UPL. Max. Ausgangsspannung Vpp Spitze-Spitze, Verzerrungen in Prozent, Rauschabstand S/N A-bewertet, Stromaufnahme Ibat bei Vollaussteuerung

OpAmp | Vpp | Dist. | S/N | Ibat
-----|-----|-----|-----|-----
TL072 | 5,5 | 0,004% | 85,5dB | 3,3mA
LF412 | 5,6 | 0,003% | 85dB | 3,9mA
OPA2134 | 6,4 | 0,004% | 86,5dB | 8,2mA
OPA2604 | 2,7 | 0,008% | 86dB | 9,5mA

Den besten Kompromiss aus Messdaten und Stromaufnahme bieten die preiswerten Typen TL072 und LF412. Der OPA2134 liefert weniger Rauschen, ist aber deutlich teurer und nimmt relativ viel Strom auf. Der OPA2604 verbietet sich wegen der zu niedrigen möglichen Ausgangsspannung. Bipolare Typen (LM833, NE5532 usw.) sind wegen ihres hohen Eingangsstroms und der daraus resultierenden hohen Offset-Spannung nicht geeignet.
