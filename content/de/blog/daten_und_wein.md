---
author: "Sören Etler"
title: "Daten und Wein"
date: 2024-06-27
description: "Eine Reise durch die Weinregionen Baden-Württembergs basierend auf einer Datenanalyse der touristischen Landesdatenbank."
tags: ["Datenanalyse", "Tourismus", "Open Data"]
thumbnail: /daten_und_wein.png
---

Was gibt es besseres als Daten und Wein? Ich muss zugeben, ich bin kein ausgewiesener Weinkenner und nach Riesling, Chardonnay und Grauburgunder hört mein Wissen zu Weinsorten schnell auf.
Umso spannender für mich, als ich die Möglichkeit hatte mir die Daten rund um Weinorte, Weinlagen und Weinregionen in der touristischen Landesdatenbank der TMBW (Tourismus Marketing GmbH Baden-Württemberg) genauer anzusehen und für den Knowledge Day der Deutsche Zentrale für Tourismus in wenigen Grafiken aufzubereiten.

## Kann Excel auch Karten?
Gestartet habe ich diese Datenanalyse mit einem kleinen Experiment: Ich wollte gucken, wie weit ich mit einer Analyse der Daten in Excel komme. Und was soll ich sagen: nicht weit! Excel kann zwar auch Karten als Diagrammtyp erstellen, diese sind aber sehr eingeschränkt in der Nutzung. Es können nur Regionen eingefärbt werden und eine Visualisierung von einezelnen Punkten (z.B. PoIs) oder Strecken (z.B. Touren) ist nicht möglich. Auch bei den möglichen Regionen ist man starkt eingeschränkt. Eine Verwendung von eigenen Polygonen (z.B. Reiseregionen) wird nicht unterstützt. Ich habe mich hier also für die Nutzung der Postleitzahlgebeite entschiedenen um die Lage von Weingütern in Baden-Württemberg zu zeigen.

![Excel kann auch Karten!](/weingüter_in_excel.png)

Meine Erfahrungen bei der Erstellung von Karten in Excel habe ich auch in diesem [LinkedIn-Post]( https://www.linkedin.com/posts/soeren-etler_diese-karte-habe-ich-in-excel-erstellt-activity-7200843206261960704-DdtH) zusammengefassst.

## Wo liegen die Weingüter?
Die kurze Antwort ist: In den beiden großen Weinregione Baden-Württembergs - Baden und Württemberg.

Die lange Antwort zeigt sich in dieser Grafik. Die roten Punkte zeigen die Weingüter, die in der touristischen Landesdatenbank als PoIs hinterlegt sind. Die helleren Punke - in der Weinsprache würde man vielleicht von Rosé-farbenden Punkten sprechen - zeigen Andere PoIs, die etwas mit Wein zu tun haben. Von Weinlehrpfaden zu Weinbars ist hier alles dabei. Es mag nicht verwunderlich sein, dass sich wieder deutlich die Weinregionen zeigen, trotzdem erfreut es mich immer wieder, wenn sich reale Gegebenheiten so in den Daten wiederspiegeln.

![Wein in Baden-Württemberg](/wein_in_bw.png)

Eine Besonderheit zeigt sich im äußersten Süden: Am Bodesee gehören die Weinlagen im westlichen Teil zwischen Hegau und Meersburg zu Baden und im östlichen Teil um Kressbronn zum Württembergischen Bodensee. Insgesamt gibt es 7 verschiedene Weinanbaugebiete am Bodensee. Der Würrtembergische Bodensee bildet mit dem Bayrischen Bodensse ein Weinanbaugebiet.

Zusätzlich gibt es noch ein österreichisches, zwei schweizer und ein liechtensteiner Weinanbaugebiete:
- Vorarlberg
- Das Rheintal
- Thurgau
- Schaffhausen Blauburgunderland / Klettgau
- Fürstentum Liechtenstein

Durch die Spiegelung der Sonne im Bodensee, die besondere Ausrichtung der Hänge und die unterscheidlichen Böden unterscheiden sich diese Regionen - und auch die angebauten Weine.

## Welcher Wein ist wo?
Die Weinanbaugebiete lassen sich auch gut nach den angebauten Weinsorten unterscheiden. die folgenden Visualisierungen zeigen die Verbreitung von verschiedenen Weinsoten in Baden-Württemberg. In diesem Fall hatte ich keine genauen Daten und habe daher das Vorkommen der Weinsorten in den Beschreibungstexten von Weingütern in der touristischen Landesdatenbank als Näherung benutzt. Das hat super funktioniert und man kann direkt erkennen, welche Sorten flächendeckend vorhanden sind und welche sehr speziell für eine Region sind.

<link rel="stylesheet" href="/gallery.css">
<script src="/gallery.js"

<!-- The grid: four columns -->
<div class="row">
  <div class="column">
    <img src="/weinsorten.png" alt="Weinsorten Übersicht" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Grauburgunder.png" alt="Grauburgunder" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Gutedel.png" alt="Gutedel" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Kerner.png" alt="Kerner" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Lemberger.png" alt="Lemberger" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Müller-Thurgau.png" alt="Müller-Thurgau" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Riesling.png" alt="Riesling" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Schwarzriesling.png" alt="Schwarzriesling" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Silvaner.png" alt="Silvaner" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Spätburgunder.png" alt="Spätburgunder" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="wein/Trollinger.png" alt="Trollinger" onclick="myFunction(this);">
  </div>
</div>

<!-- The expanding image container -->
<div class="container">
  <!-- Close the image -->
  <span onclick="this.parentElement.style.display='none'" class="closebtn">&times;</span>

  <!-- Expanded image -->
  <img id="expandedImg" style="width:100%">

  <!-- Image text -->
  <div id="imgtext"></div>
</div>

## Und wie kann man Wein beschreiben?
In meiner letzten Auswertung möchte ich nicht nur auf die Geodaten und die Verbreitung von Weinen schauen, sondern einen größeren Fokus auf die Beschreibungstexte legen. Ich wollte wissen mit welchen Adjektiven das Wort "Wein" in den Texten beschrieben wird. Von den XXX Vorkommnissen von dem Wort "Wein", wird das Nomen in XXX Fällen von einem oder mehreren Adjektiven begleitet.

Diese Wortwolke zeigt die häufigsten Adjektive, die Wein beschreiben.

![Wortwolek Adjektive zu Wein](/wortwolke_wein.png)

Im nächsten Schritt interessiert mich, wie eine Generalisierung von so einer Analyse aussehen kann. In zwei Richtungen kann ich mir dies gut vorstellen.

1. Welche Adjektive beschreiben ein bestimmtes Nomen? (so wie ich es auch bei der Analyse zu "Wein" gemacht habe.)
2. Welche Nomen werden von einem bestimmten Adjektiv beschrieben?  (Welche anderen Nomen werden noch als "regional" beschrieben?)
