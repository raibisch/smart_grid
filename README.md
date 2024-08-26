# smart_grid
Ideen rund um Smart-Grid

## Dynamischer Strompreis mit Preisbremse ?

"dynamische Strompreise" ...was ist das ? ...gibt es das auch für mich?  ...will ich das? ... Chancen und Risiken ?

### Was ist das:
Unter dynamischen Strompreisen versteht man einen Strompreis der meist als Stundenpreis am Vortag an der Strombörse EPEX ausgehandelt wird. Deutschland hat bedingt durch  den hohen Anteil an regenerativen Energien  einen sehr volatilen Stunden-Strompreis (inc Netzentgelt und Steuern zwischen 5 und 50cent). Meist liegt der Strompreis auch im Mittel (zwischen 15 und 35cent)  unter den Preisen von Jahresverträgen mit Preisgarantie.

Gibt es das auch für mich:
Ab 2025 müssen die Stromanbieter (auch für private Verbraucher)  mindestens einen dynamischen Stromtarif anbieten. Da dies jedoch einen digitalen "Smart-Meter" (=intelligenten Stromzähler) voraussetzt, werden zunächst nur Haushalte mit mehr als 6000 kW/h Jahresverbrauch und großen PV-Anlagen (> 7kW-peak)  diesen Tarif nutzten können (In der Verordnung steht auch was von Haushalten mit einer "steuerbaren Verbrauchseinrichtungen" (=Wärmepumpe oder Wallbox) ich kenne jedoch noch niemanden mit WP oder WB der automatisch einen anderen Zähler bekommen hat. Ohne diesen "Smart-Meter" kann z.Z. nur der Stromanbieter "Tibber"    für digitaler Stromzähler ohne Netzwerkanbindung (=moderne Meßeinrichtung)  mit Hilfe eines Adapters einen Stundenpreis anbieten, das ist jedoch ehrlicherweise eher was für "Strom-Nerd's".

### Will ich das:
Interessant ist ein dynamischer Tarif für alle, die Ihren Stromverbrauch (zumindest teilweise) in die günstigen Tages und Nachtstunden verschieben können.  In Privathaushalten sind das in erster Linie die Verbraucher Elektroauto und Wärmepumpe. 

### Die Chancen: 
Zunächst profitieren wir alle davon, wenn unser Stromverbrauch den Angebot von erneuerbaren Energien gut angepasst ist (das Netz bleibt stabil und es müssen auch weniger Windräder abgeregelt werden) . 
Das Laden des Elektroautos kann man sehr gut in die günstigen Stunden verschieben (bei 20-40kW pro Tag liegt hier auch ein großes Potential).  Auch die Wärmepumpe kann man - zumindest in Grenzen - so betreiben, dass zumindest die Preisspitzen mit Hilfe der "Smart-ready" Funktion der neueren Wärmepumpen umgangen werden können.

### Die Risiken:
Es gibt keine Preisgarantie oder eine automatische "Preisbremse" für den Stundenpreis !... und Vorhersagen - besonders wenn sie in der Zukunft liegen - sind immer schwierig ;-)
EPEX-Panne: Am 26. Juni 2024 erlebten Stromkunden mit dynamischen Tarifen den Strompreis-Super-GAU: Zwischen 6:00 und 7:00  Uhr morgens schnellten die Preise für eine kWh auf rund 2,30 Euro hoch (bei einer Stunde an der  22kW Wallbox sind das rund 50€). 
Grund war ein "Software-Fehler" der Strombörse EPEX. Bis heute gibt es weder eine Entschädigung hierfür, noch  sind Maßnahmen angekündigt worden, die den Verbraucher in Zukunft vor solchen Fehlern schützen.

### Machen oder sein lassen ?
Es wäre doch schön wenn, man vorab schon mal aufgrund des Verbrauchsprofils  die Kosten vorab "virtuell" mit einer Simulation ermitteln könnte (und dann eine sinnvolle und faktenbasierende Entscheidung treffen kann)
Wenn man das schließlich nutzen will, wäre eine eingebaute "Preisbremse" (siehe EPEX-Panne) wünschenswert, die Wallbox und Wärmepumpe bei sehr hohen Strompreisen runter regelt.
Noch schöner wäre natürlich eine Optimierung des Verbrauchs von Wallbox und Wärmepumpe je nach Strompreis und evt. noch die Einbeziehung einer PV-Anlage.

### ...zuviel gewünscht ?
Ich habe jetzt mal den Anfang gemacht und für alle Software- und Elektronik-Nerds eine 5-10€-Lösung zusammengestellt (die wie immer bei mir als "open-source" offen und frei verfügbar ist)
#### Was schon geht:
- Ermittlung der aktuellen Stundenstrompreise (inc.aller Steuern und Netzentgelte !)
- Anzeige der Daten auf einer Web-App (für alle Mobilgeräte und PC)
- Regelbasierende Auswertung (zur Steuerung von Wärmepumpe oder Wallbox)
- SG-ready Ansteuerung (Relay-Ausgang) für alle SG-ready fähigen  Wärmepumpen
- vieles mehr (Modbus für ext. Stromzähler,  Logging von Daten der AIT-Wärmepumpen)
#### Was bald kommt:
- "virtuelle" Stromrechnung (in Verbindung mit Lesegerät für digitale Stromzähler)
-  Modbus-Ansteuerung  für Wallbox (z.Z. nur für ABL-Wallbox geplant)
#### ... weitere Ideen:
- Vorhersage der PV-Leistung (1-2 Tage)
- Eure Ideen ?

..demnächst auf  https://github.com/raibisch/smart_grid
