---
author: "Sören Etler"
title: "Domblicke: Von wo sieht man den Dom?"
date: 2025-05-15
description: "Der Magdeburger Dom prägt die Silhouette der Stadt wie kein anderes Bauwerk. Aber von welchen Orten aus ist er eigentlich sichtbar? "
tags: ["Datenanalyse", "Tourismus", "Open Data"]
thumbnail: /domblicke.png
---

**Der Magdeburger Dom prägt die Silhouette der Stadt wie kein anderes Bauwerk. Aber von welchen Orten aus ist er eigentlich sichtbar? Mit meinem Projekt Domblicke gehe ich dieser Frage nach. Auf einer interaktiven Karte zeige ich, von welchen Punkten im Stadtgebiet aus man den Dom sehen kann – und von welchen nicht.**

## Sichtbarkeit als digitales Erlebnis

Die Idee für dieses Projekt entstand nach dem Ansehen eines YouTube-Videos von Adam Cole und Joss Fong, in dem sie das Projekt shademap.app vorstellen. Dort wird visualisiert, wann Orte auf der Erde im Schatten liegen. Inspiriert davon habe ich mithilfe eines Tutorials von Helen Makes Maps die Technik auf Magdeburg angewendet.

Ich nutze die Open-Source-Software QGIS. Das Verfahren basiert auf einer Viewshed-Analyse: Man wählt einen Beobachtungspunkt – in meinem Fall die Türme des Magdeburger Doms –, lädt ein Höhenmodell der Umgebung und berechnet, welche Flächen auf Basis von Gelände und Bebauung sichtbar sind.

Berechnet habe ich die Karten mit dem Oberflächenmodell (DOM) und dem Geländemodell (DGM) des Landesamts für Vermessung und Geoinformation Sachsen-Anhalt (LVermGeo). Beide Modelle sind offen verfügbar und bieten eine hohe Auflösung von 1 Meter.

Für die Webkarte habe ich nur die sichtbaren Flächen markiert, die nicht bebaut sind – denn eine Sicht vom Hausdach ist für die meisten Menschen weniger hilfreich. Die berechneten Kacheln habe ich in eine interaktive Leaflet-Karte überführt:

👉 domblicke.soerenetler.de

## Anwendungsfälle im Tourismus

Solche Sichtbarkeitsanalysen bieten spannende Perspektiven für den Tourismus. Statt nur statisch auf Sehenswürdigkeiten hinzuweisen, lassen sich neue Fragen stellen:

- Wo lohnt sich ein Aussichtspunkt wirklich? Man kann prüfen, welche Wahrzeichen von dort aus sichtbar sind.

- Welche Orte bieten Fernblick auf den Kirchturm oder ein Schloss? Das ist besonders für Panoramawege oder Radstrecken interessant.

- Wie lassen sich Sichtachsen in digitale Entdeckertouren integrieren? Zum Beispiel mit dem Motto: "Folge dem Blick auf den Dom".

Ein konkreter Anwendungsfall: Ein Tourismusverband könnte mit solchen Analysen neue Aussichtspunkte erschließen und beschildern – inklusive QR-Codes zur Domblicke-Karte.

## Ideen für die Weiterentwicklung

Das Thema Sichtbarkeit lässt sich auch spielerisch oder historisch denken:

- **Gamification**: Wer findet die meisten Domblicke im Alltag? Eine App mit Foto-Upload und Rangliste könnte daraus ein Spiel machen.

- **Historische Perspektiven**: Wie haben sich die Sichtachsen auf den Dom durch Neubauten verändert?

## Karte entdecken

Die interaktive Karte findest du unter domblicke.soerenetler.de. Viel Spaß beim Erkunden der Domblicke! Ich freue mich über Fotos vom Dom aus den unterschiedlichsten Ecken Magdeburgs.



## Quellen der Inspiration:

- Video von Adam Cole & Joss Fong: YouTube-Link
- Tutorial von Helen Makes Maps: Zur Anleitung

