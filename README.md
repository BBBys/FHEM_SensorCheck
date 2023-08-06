# FHEM Sensor Check
Kontrolle, ob Sensoren in **FHEM** noch laufen

Programm stellt fest, wann die Sensoren zuletzt Daten geliefert haben

Programm auf 		/usr/local/fhemskripte
Logfiles liegen auf	/opt/FHEM/log

Starten über cron.daily
	#!/bin/sh
	mono /usr/local/fhemskripte/FHEMlogs.exe

