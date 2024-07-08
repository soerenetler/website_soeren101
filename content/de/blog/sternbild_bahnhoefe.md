---
author: "Sören Etler"
title: "Das Sternbild der Bahnhöfe"
date: 2024-07-08
description: "Eine Darstellung der Bahnhöfe in Deutschland als Sternbilder basierend auf offenen Daten "
tags: ["Datenanalyse", "Tourismus", "Open Data"]
thumbnail: /bahnhof_sternbild.png
---

Für eine aktuelle Analyse wollte ich wissen, in welchen Gemeinden es einen Bahnhof gibt. Als kleines Nebenprodukt entstand diese schöne Karte der Bahnhöfe zwischen Wolfsburg, Berlin und Leipzig.

Ich finde es schön zu sehen, wie sich die Bahnlinien wie Lebensadern durch das Land ziehen - und wie viele ich schon bereist habe und mit den Orten eine kleine Geschichte verbinde.

<div id="map", style="height: 600px; width: 100%"></div>

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.3/dist/leaflet.css"
integrity="sha384-o/2yZuJZWGJ4s/adjxVW71R+EO/LyCwdQfP5UWSgX/w87iiTXuvDZaejd3TsN7mf"
crossorigin=""/>
<script src="https://unpkg.com/leaflet@1.9.3/dist/leaflet.js"
integrity="sha384-okbbMvvx/qfQkmiQKfd5VifbKZ/W8p1qIsWvE1ROPUfHWsDcC8/BnHohF7vPg2T6"
crossorigin=""></script>
<script>
    var map = L.map('map', { attributionControl: false } ).setView([51.15287186285573, 10.100505460342438], 8.0);
    L.control.attribution( { prefix: false } ).addTo( map );
    var tilesource_layer = L.tileLayer('/bahnhof_karte/{z}/{x}/{y}.png', {
    minZoom: 6,
    maxZoom: 10,
    tms: false,
    attribution: 'Mit QGIS erstellt; Datenquellen: Deutschen Bahn AG & DELFI e.V.'
    }).addTo(map);
</script>

Ich habe die Station Data API der Deutschen Bahn verwendet. Hier werden alle Bahnhöfe mit vielen Zusatzinformationen zur Verfügung gestellt - als Open Data unter einer cc-by-Lizenz. Die Daten für die Haltestellen stammen aus dem zentralen Haltestellenverzeichnis von DELFI - ebenfalls unter cc-by Lizenz veröffentlicht.

Die Unterscheidung zwischen Knotenbahnhöfen (gelbe Punkte) und Zubringerbahnhöfen (orange Punkte) war für mich besonders hilfreich und macht die Karte deutlich übersichtlicher. Die Knotenbahnhöfe sind so etwas wie die hellen Sterne am Himmel, die bei der Orientierung helfen. Und dazwischen gibt es viele kleine Zubringerbahnhöfe. Diese Analogie wird noch deutlicher, wenn ich zusätzlich alle Bushaltestellen als schimmernde Punkte im Hintergrund einblende.

🏙️ 400 Kontenbahnhöfe
🚉 4000 Zubringerbahnhöfe
🚏 880.000 Haltestellen
