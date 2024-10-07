# FHEM Sensor Check
Check whether sensors in *FHEM* are still running
## Problem
Sensors are integrated into the *FHEM* smart home software to display measured values ​​and use them for control. The measured values ​​are saved in log files.

The **sensors can fail**, e.g. when the battery is empty.
## Solution 
The program reads all available log files and determines when a sensor last delivered data. If this time is too far back, an email will be sent.
## Implementation
* Implementation on the same server running FHEM
* Program on ```/usr/local/fhemScripte```
* Log files on ```/opt/FHEM/log```
* Start via ```cron.daily```
-----
# FHEM Sensorprüfung
Kontrolle, ob Sensoren in *FHEM* noch laufen
## Problem
In der Smart-Home-Software *FHEM* werden Sensoren eingebunden, um gemmessene Werte anzuzeigen under für die Steuerung zu verwenden. Die Messwerte werden in Log-Dateien gespeichert.

Die **Sensoren können ausfallen**, z. B. wenn die Batterie leer ist.
## Lösung
Das Programm liest alle verfügbaren Logfiles und stellt fest, zu welchem Zeitpunkt ein Sensor zuletzt Daten geliefert hat. liegt dieser Zeitpunkt zu weit zurück wird eine Mail gesendet.
## Umsetzung
* Implementierung auf dem gleichen Server, auf dem FHEM läuft
* Programm auf ```/usr/local/fhemskripte```
* Logfiles auf ```/opt/FHEM/log```
* Starten über ```cron.daily```
