# Gleichrichter Fernlicht PCB#
Schaltung stammt von hier: https://fahrradzukunft.de/14/mosfet-gleichrichter
Serienkondensator von 390uF antiparallel hat sich als optimum herausgestellt (im Vgl. zu 330uF und 560uF)
Spannungsfestigkeit Kondensator: 35V (Großzügig)

Verwendete Mosfets:
N-Kanal: IRLML 0030
P-Kanal: TSM 3401 -> Kann aber nur max. 12V VGS

Anforderungen Mosfets:
möglichst niedriges RDS_on
30V VDSmax (großzügig)
Am besten möglichst hohes VGS_max -> 20V
Gate-Source sieht immer ca. die Ausgangsspannung -> 12V Reichen locker für 2 LEDs in Reihe mit jew. 6V am Ausgang. Je höhere Ausgangsspannungen auftreten können desto höher muss VGS_max sein.

Zenerdioden Schützen Gate vor zu hohen Spannungen. Aber auch nur kurzfristig, denn die können den Strom nicht ab. Zenerspannungen sollten also unter dem VGS_max sein!

Bei erster Version war Fehler im Layout: Die Pin-Reihenfolge der Standard-Mosfet-Symbole passt nicht zum SOT-23 Gehäuse.
Mosfets mussten daher auf dem Kopf gelötet werden.
Funktioniert so aber gut.

Ist jetzt im Schaltplan korrigiert aber das Layout  noch nicht fertig. (Falls nochmal aufgebaut wird)
