# Telegram COVID-19 Bot
Dies ist ein Telegrambot, der aktuelle COVID-19 Zahlen für verschiedene Orte bereitstellt.
Es können mehrere Orte und Bundesländer abonniert werden können, sodass bei neuen Zahlen des Robert-Koch-Instituts (RKI) eine Zusammenfassung mit den relevanten Orten bereitgestellt wird.
Der aktuelle Prototyp läuft unter [@CovidInzidenzBot](https://t.me/CovidInzidenzBot) und ist Work in Progress.

## Features
Du kannst einfach eine Nachricht mit dem Stadt-/Landkreis, Bundesland oder einem Standort an den Bot senden.
Dann erhälst du eine Liste mit möglichen Orten oder Aktionen, bspw. "Bericht" für die aktuellen Daten oder "Starte Abo" um diesen zu abonnieren.

Außerdem gibt es diese Befehle:
* `/hilfe` bzw. `/start`: Überblick über die Befehle
* `/ort $1`: Aktuelle Daten für `$1`
* `/abo $1`: Abonniere tägliche Daten für `$1`
* `/beende $1`: Beende Abonnement für `$1`
* `/bericht`: Zeige den aktuellen Bericht mit der Coronainzidenz
* `/statistik`: Nutzungsstatistik
* `/datenschutz`: Datenschutzerklärung
* `/loeschmich`: Lösche alle Daten


## Installation
Die aktuelle Version kann man unter [@CovidInzidenzBot](https://t.me/CovidInzidenzBot) benutzen.

Für einen eigenen Telegrambot muss die Konfiguration von `resources/config.default.ini` nach `config.ini` kopiert und ausgefüllt werden.
Danach kann er über `python3 -m covidbot` gestartet werden.

## Credits
Die Informationen über die Corona-Infektionen werden von der offiziellen Schnittstelle des RKI für [Landkreise](https://hub.arcgis.com/datasets/917fc37a709542548cc3be077a786c17_0) und [Bundesländer](https://npgeo-corona-npgeo-de.hub.arcgis.com/datasets/ef4b445a53c1406892257fe63129a8ea_0) abgerufen und stehen unter der Open Data Datenlizenz Deutschland – Namensnennung – Version 2.0.
Weitere Informationen sind auch im [Dashboard des RKI](https://corona.rki.de/) sowie dem [NPGEO Corona Hub 2020](https://npgeo-corona-npgeo-de.hub.arcgis.com/) zu finden.

Welche Bibliotheken und andere Dienste wir noch verwenden, kannst Du unter [Credits](https://github.com/eknoes/covid-bot/wiki/Credits) im Wiki einsehen.

[Datenschutzerklärung](https://github.com/eknoes/covid-bot/wiki/Datenschutz) | [Impressum](https://github.com/eknoes/covid-bot/wiki/Impressum)
