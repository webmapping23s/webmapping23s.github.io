# Workload für die Woche vom 4. bis 11. Mai 2023

## Wetterstationen Euregio Beispiel vorbereiten

1. erstellt auf github.com ein neues public Repo `aws-euregio`

2. cloned es lokal und packt das [AWS Euregio Template](https://webmapping.github.io/templates/template_aws-euregio.zip) dort aus

3. implementiert Icons für die Wetterstationen in der asynchronen Funktion `showStations`
    - verwendet das Icon `wifi` der [Map Icons Collection](https://mapicons.mapsmarker.com/)
    - wählt <https://clrs.cc> OLIVE als Icon-Farbe
    - speichert das Icon im `icons` Unterverzeichnis als `icons.png`

4. erstellt auch Popups für die Stationen mit
    - Name der Station und Seehöhe als Überschrift
    - eine ungeordnete Liste mit Werten für:
        - Lufttemperatur (LT) in °C
        - Relative Luftfeuchte (RH) in %
        - Windgeschwindigkeit (WG) in km/h (!)
        - Schneehöhe (HS) in cm
    - Tipp 1: nicht alle Stationen messen alle Werte, verwendet deshalb den Trick für fehlende Werte, den wir bei den Popups der Fußgängerzonen Wiens kennengelernt haben  ...
    - Tipp 2: die Seehöhe der Station verbirgt sich im Array `feature.geometry.coordinates` ...

5. pushed alles zurück zu github.com und macht das Repo über die Settings online verfügbar

Bis spätestens **Donnerstag, den 11. Mai 2023 um 12:00 Uhr mittags** soll das fertige Beispiel unter https://usernmame.github.com/aws-euregio erreichbar sein
