---
author: "Sören Etler"
title: "Wie heißen Orte in Brandenburg?"
date: 2022-06-20
description: "Was heißt das für einen Ortsnamen „brandenburgisch“ zu klingen? Ist es möglich neue brandenburger Ortsnamen zu generieren, die so klingen, als könnten sie echt sein?"
tags: ["Brandenburg", "Dorf"]
thumbnail: /thumbnail_brandenburger_orte.png
---

 Ich weiß nicht, ob diese Entwicklung nützlich ist – aber spannend ist sie auf jeden Fall. In vielen Projekten in Brandenburg bin ich mit unterschiedlichen Städten und Dörfern in Kontakt gekommen. Bei einigen merkt man sofort, dass sie hierhergehören - sie klingen brandenburgisch.

 - Aber was heißt das für einen Ortsnamen „brandenburgisch“ zu klingen?
 - Ist es möglich neue brandenburger Ortsnamen zu generieren, die so klingen, als könnten sie echt sein?

# Gucken wir uns die Ortsnamen aus Brandenburg etwas genauer an –ow

In Brandenburg gibt es 413 politisch selbstständigen Städten und Gemeinden (so sagt es zumindest Wikipedia). Wichtig ist mir aber auch die 1.776 Ortsteile zu berücksichtigen. Nützlicherweise veröffentlich das Land Brandenburg ein Gemeinde- und Ortsteilverzeichnis mit mehr als 5.000 Namen. Hierzu gehören neben kreisfreien Städten und Gemeinden auch Ortsteile, Gemeindeteile und sonstigen Wohnplätzen bzw. Siedlungsnamen.

![Diagram über die Länge der Ortsnamen](/wortlaenge_orte_brandenburg.png)

Der kürzeste Ortname ist der Ortsteil Lug in der Gemeinde Bronkow im Kreis Oberspreewald-Lausitz. Weitere Namen mit drei Buchstaben sind Amt, Dom und Aue. Diese sind jedoch nur als Gemeindeteile bzw. Wohnplatz gelistet.

Den längsten Namen hat die Gemeinde Groß Schacksdorf-Simmersdorf mit 28 Zeichen. Länger sind nur die Bungalowsiedlung Carwitzer See, Forsthaus Oppelhainer Pechhütte und Hartmannsdorf-Neu Hartmannsdorf, die aber ebenfalls nur als Gemeindeteile oder Wohnplätze aufgeführt sind.

Die meisten Namen fangen mit S, B oder K an. A ist auf Platz 9 der erste Vokal. Nur Wohnplätze haben einen Umlaut an erster Stelle. Es sind drei: Ölschlägers Mühle, Üderheide und Ützdorf. Und, es gibt mehr brandenburger Ortsnamen, die mit Q (10) anfangen als mit I (8). Nur bei X, Y und Ä könnt ihr bei Stadt, Land, Fluss in der Kategorie Ortsnamen in Brandenburg passen – es gibt keine!

Noch ein kurzer Blick ans Wortende, bevor wir anfangen Namen zu generieren. 8% der Namen enden auf -ow. Es gibt sowohl ein Lunow als auch ein Lünow. Nur 2% enden auf -in: Menkin, Mescherin.

# So jetzt geht es mit dem Generieren los!

Ich habe die Namen zeichenweise generiert. Es wird also immer ein Buchstabe nach dem anderen hinzugefügt. Daher fängt der Prozess auch mit dem Aufsplitten der Namen in die einzelnen Zeichen an. In der Liste von brandenburger Ortsnamen gibt es 67 verschiedene Buchstaben und Zeichen. Neben dem Alphabet (in Groß- und Kleinschreibung) und Umlauten, sind dies auch Leerzeichen und Sonderzeichen (wie Bindestich, Klammern und Punkt).

Jedes Zeichen wird als 16-dimensionaler Vektor dargestellt. So können Ähnlichkeiten zwischen ihnen besser berücksichtigt werden. Bestimmte Konsonantengruppen sind vielleicht ähnlicher zueinander als andere. Ein „T“ ist möglicherweise näher an einem „D“ als an einem „R“.

Im Herzen des Systems ist ein Recurrent Neural Network. Dieses nutzt die kombinierten Informationen aus den vorherigen Buchstaben und dem Vektor des jetzigen Buchstabens, um eine Wahrscheinlichkeitsverteilung über den nächsten Buchstaben zu generieren. Dieser Vorgang wird wiederholt. Aus allen möglichen Buchstaben wird dann basierend auf ihrer Wahrscheinlichkeit ein Buchstabe (nicht zwingend der mit der höchsten Wahrscheinlichkeit) ausgewählt.

So werden Buchstabe für Buchstabe neue Ortsnamen generierten, die so klingen, als würden sie aus Brandenburg kommen.

Beispiel:
- Gerkbecke
- Driest
- Wallshag
- Kapplow
- Kabewitz/Hark
- Silkow-Hollenberg
- Alte Grüne
- Friesnig
- Sieblung Grießbendee
- Stötzen
- Brückel
- Birchhof
- Malzheusen
- Grossdorf
- Brömnitz
- Pelzik
- Rohlenkshorfn

Im nächsten Schritt wäre auch eine Gliederung auf Kreisebene denkbar: Märkisch-Oderland klingt sicherlich anders als die Prignitz oder der Fläming. Vielleicht wird daraus mal ein Spiel – „Welchen dieser Orte gibt es nicht?“ oder eine größere Auswertung. Bei mir bleiben noch viele Fragen offen: Woher stammen die Ortsnamen? Heißen große Städte anders als kleine Dörfer? Vielleicht können diese Auswertungen dabei helfen, die Geheimnisse von Brandenburgs Dörfern zu verstehen.

Falls Sie Ideen für spannende Open Data Projekte haben oder noch mehr Details über dieses erfahren wollen, können Sie mir gerne eine Nachricht schreiben. Ich bin gespannt auf Feedback, Ideen und weitere Vorschläge.


# Quellen
 - Daten: https://geobasis-bb.de/lgb/de/geodaten/weitere-digitale-produkte/gemeinde--ortsteilverzeichnis/# © GeoBasis-DE/LGB, dl-de/by-2-0
 - Code basierend auf https://www.tensorflow.org/text/tutorials/text_generation