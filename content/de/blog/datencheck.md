---
author: "Sören Etler"
title: "Datenchecks: Datenqualität messen und verbessern"
date: 2025-07-16
description: "Datenqualität kann nur verbessert werden, wenn sie auch gemessen wird."
tags: ["Datenanalyse", "Tourismus", "Open Data"]
thumbnail: /datencheck/datencheck.png
---

**„Datenqualität kann nur verbessert werden, wenn sie auch gemessen wird.“** Genau hier setzen die Datenchecks an, die ich für Baden‑Württembergs zentrale Datenbank *mein.toubiz* und Sachsens *SaTourN*-Datenbank durchgeführt habe. In diesem Blogpost erkläre ich, was es mit diesen Datenchecks auf sich hat, welche **Qualitätskriterien** geprüft wurden und welchen **Mehrwert** sie bieten – ganz nach dem Prinzip: Ohne Messung keine Verbesserung. Sie erfahren zudem, wie solche Analysen Ihre Organisation motivieren können, **gezielt an besserer Datenqualität zu arbeiten**, und wir geben Anregungen für weiterführende Auswertungen.

## Warum ist Datenqualität im Tourismus wichtig?

In der digitalen Tourismuswelt sind zuverlässige, aktuelle und vollständige Daten Gold wert. Ob es um Beschreibungen von Sehenswürdigkeiten, Veranstaltungsdetails oder Unterkunftsinformationen geht -  **hochwertige Daten** sorgen dafür, dass Gäste die richtigen Infos zur richtigen Zeit am richtigen Ort erhalten. Die landesweiten Daten-Hubs wie *mein.toubiz* in Baden-Württemberg und *SaTourN* (Sachsen Tourismus Netzwerk) in Sachsen bilden die Grundlage dafür, dass diese Inhalte zentral erfasst und über viele Kanäle ausgespielt werden. Entsprechend hat die Qualität dieser Daten **oberste Priorität**: Ungenaue oder fehlende Angaben führen zu unzufriedenen Gästen, während gute Daten zu mehr Sichtbarkeit und besserem Gästeerlebnis beitragen.

Doch wie erkennt man, *wie gut* die Daten sind? Hier kommen die Datenchecks ins Spiel.

## Was wurde geprüft? – Komponenten der Datenqualität

Die durchgeführten Datenchecks analysierten verschiedene **Qualitätskomponenten** in den touristischen Datenbanken *mein.toubiz* (Baden-Württemberg) und *SaTourN* (Vogtland/Sachsen). Die Datenchecks wurden so konzipiert, dass sie **klar und visuell ansprechend** den Status quo der Datenqualität darstellen. Jeder Bericht – ob für eine einzelne Organisation in Baden-Württemberg oder für eine Datenkategorie im Vogtland – ist nach einem ähnlichen Muster aufgebaut:

![Datencheck BaWü](/datencheck/datencheck_bw.png)

*Beispielhafte Auswertung aus dem&#160;**mein.toubiz Datencheck 2024**&#160;für Tourismus Baden-Württemberg: Der Bericht zeigt oben Gesamtzahlen und Lizenzquoten (nur 21 % der Einträge sind Open Data), daneben die Hauptkategorien der Einträge im Vergleich zum Landesdurchschnitt. Unten werden Kennzahlen zu Beschreibungstexten, Kurzbeschreibungen und Bildern dargestellt – z.B. haben 73 % der Einträge einen Beschreibungstext, aber nur 51 % liegen im empfohlenen Längenbereich von 300–1000 Zeichen. Außerdem besitzen 83 % der Einträge mindestens ein Bild.*

GARFIK DATENCHECK Vogtland

*Ausschnitt aus dem&#160;**Datencheck 2025 Vogtland (POI)**: Auch hier die Schlüsselwerte oben (1103 Einträge, 48 Dubletten, 14 % Open Data Quote insgesamt). Die Hauptkategorien der POIs werden mit Prozent und Balken dargestellt – man sieht z.B., dass \~7 % der POIs Geldautomaten sind. Unten: 94 % der POIs haben einen Beschreibungstext, 84 % dieser Texte liegen in empfohlener Länge. 87 % haben eine Kurzbeschreibung, 70 % davon in idealer Länge. 92 % der POIs besitzen Bilder, jedoch sind nur bei 46 % der Einträge die Bilder Open Data (grüner Anteil im Kreisdiagramm).*


- **Übersicht und Kennzahlen:** Am Anfang jeder Auswertung stehen die wichtigsten Kennzahlen auf einen Blick. Dazu zählen die Anzahl der **Einträge** (z.B. alle POIs einer Region), eventuell die Anzahl an **Entwürfen** oder importierten Datensätzen, sowie zentrale Quoten. Im Baden-Württemberg-Check sieht man z.B. wie viele Einträge eine Organisation im System hat und welche **Hauptkategorien** diese Einträge zugeordnet sind. Diese Liste wird immer ins Verhältnis zum Landesdurchschnitt gesetzt („BaWü Ø“). Das schafft Kontext: Wenn z.B. 10 % der eigenen Einträge der Kategorie „Essen & Trinken” zugeordnet sind, entspricht das genau dem Landesdurchschnitt.
- **Lizenzen:** Ein ganz wichtiger Aspekt ist die **Lizenzierung der Inhalte**. Nur wenn Texte und Bilder mit offenen Lizenzen versehen sind, können sie z.B. im Rahmen von Open Data frei von Dritten genutzt werden. Die Datenchecks haben daher festgehalten, welcher Anteil der Einträge mit einer offenen **Creative-Commons-Lizenz (z.B. CC BY-SA)** publiziert wurde und wie viele Einträge noch „Alle Rechte vorbehalten“ haben.
- **Beschreibungstexte:** Ist zu jedem Eintrag (POI, Tour, Event etc.) ein Beschreibungstext vorhanden? Wenn ja, wie **lang** ist er und liegt er im empfohlenen Bereich? Beispielsweise gelten 300–1000 Zeichen als optimale Länge für ausführliche Beschreibungen (Kurzbeschreibungen ca. 250 Zeichen). Der Datencheck wertete aus, welcher Prozentsatz der Einträge überhaupt einen Beschreibungstext hat und wie viele Texte die empfohlene Länge erreichen.
- **Bilder:** Verfügt der Datensatz über mindestens ein Bild? Hier wurde die **Abdeckung mit Bildern** ermittelt (wie viel Prozent der Objekte haben ein oder mehrere Bilder). Außerdem spielt die **Bildqualität** eine Rolle – zwar wurde sie in den Berichten vor allem indirekt behandelt (z.B. ob Bilder ausreichend hochauflösend und im richtigen Seitenverhältnis sind), aber insbesondere wurde geschaut, ob genug Bildmaterial vorhanden ist. Im Vogtland-POI-Datencheck verfügen zwar 92 % der POIs über Bilder, doch nur bei 46 % der Einträge sind die Bilder auch mit offener Lizenz freigegeben. Solche Erkenntnisse motivieren, gezielt die Bildrechte zu prüfen und wo möglich Open-Data-Lizenzen einzuräumen.
- **Mindest-, gute und sehr gute Qualität:** Herzstück des Checks ist die Bewertung, wie viele Einträge gewisse **Qualitätsstufen** erreichen. Dabei wurde mit drei Stufen gearbeitet:
Für jede dieser Stufen wurde berechnet, welcher **Prozentsatz der Einträge** sie erreicht. So erkennt man beispielsweise: Erfüllen bereits viele Objekte die Minimalstandards? Wie groß ist der Sprung zu „guter“ Qualität und wie selten ist „sehr gute“ Qualität bisher? Im Vogtland-Report für Events zeigte sich etwa, dass zwar 63 % der Veranstaltungseinträge die Mindestanforderungen schaffen, aber nur **1 %** die Kriterien für „gute Qualität“ erfüllen – und **0 %** erreichen den sehr guten Bereich. Diese Zahlen waren für alle ein Weckruf.
    - *Minimale Anforderungen:* Dieser Basislevel definiert, was ein Datensatz mindestens haben sollte (z.B. **mindestens 1 Bild, einen Beschreibungstext mit Grundinformationen, eine Kategoriezuordnung**, etc.).
    - *Gute Qualität:* Hier kommen weitere Kriterien hinzu, z.B. **ausführlicherer Text**, mehrere Bilder in hoher Auflösung, ggf. Angaben wie Öffnungszeiten oder Preise – alles, was den Datensatz für Nutzer deutlich informativer macht.
    - *Sehr gute Qualität:* Die Königsklasse – der Datensatz erfüllt **alle** empfohlenen Kriterien. Dazu könnte zählen, dass der Eintrag **vollständig** ist (alle Felder ausgefüllt), **mit hochwertigen Bildern** ausgestattet ist und *alle Inhalte offen lizenziert* sind (was den Eintrag besonders wertvoll für die Weiterverwendung macht).

Je nach Datentyp wurden noch zusätzliche Punkte geprüft. Auch bestimmte Pflichtfelder (wie Geodaten, Kategorien oder Öffnungszeiten) flossen in die Bewertung der *Mindestanforderungen* ein. All diese Aspekte zusammen ergeben ein umfassendes Bild der Datenqualität.

## Wie sind die Datenchecks aufgebaut?




**Individualisierte Berichte:** Das TMBW-Projekt hat für **jede einzelne mein.toubiz-Mandanten** (alle Destinationen in Baden-Württemberg, die mit dem System arbeiten) einen eigenen PDF-Datencheck erstellt. Jede Organisation – sei es eine Stadt, ein Landkreis oder eine Tourismusregion – konnte so **ihren persönlichen Datenqualitätsbericht** in Händen halten. Darin waren die eigenen Kennzahlen stets dem Landesdurchschnitt gegenübergestellt, was einen gewissen **Benchmarking-Effekt** hat. Eine kleine Gemeinde sieht zum Beispiel, dass landesweit 53 % aller POIs mit Bildern versehen sind, man selbst aber vielleicht nur 40 % geschafft hat – eine wertvolle Info, um intern zu argumentieren, wo man aufholen sollte. Gleichzeitig wurden positive Ausreißer sichtbar: Manche Regionen hatten überdurchschnittlich lange Beschreibungstexte oder einen hohen Open-Data-Anteil. So etwas kann intern als **Best Practice** hervorgehoben werden („Schaut her, wir liegen über dem Schnitt!“) und andere motivieren**.**

**Vergleich nach Datentypen:** Für das Vogtland (Sachsen) wurde ein etwas anderer Ansatz gewählt. Hier wurde die Analyse **differenziert nach Datentypen** durchgeführt. Anstatt Berichte pro Organisation (das Vogtland ist als Region an sich schon eine Organisation) gab es separate Auswertungen für **POIs**, **Touren**, **Events**, **Gastronomie** und **Unterkünfte (Hotels)**. Diese Aufteilung ergab Sinn, weil die Datenqualität stark vom Typ abhängen kann – z.B. haben Veranstaltungen andere Anforderungen (Aktualität der Termine, regelmäßige Änderungen) als Dauer-POIs. Die Ergebnisse zeigten tatsächlich deutliche Unterschiede: So waren im Vogtland die **Hotel-Daten schon sehr gut gepflegt**, während bei **Events deutlicher Nachholbedarf** bestand. Durch die getrennte Betrachtung konnte die TMGS für jede Datenkategorie spezifische Handlungsempfehlungen ableiten.

## Wie motivieren die Ergebnisse zu Verbesserungen?

Vielleicht fragen Sie sich: Bleibt so ein Bericht nicht einfach in der Schublade liegen? Unsere Erfahrung aus Baden-Württemberg und Sachsen zeigt das Gegenteil. Durch die anschauliche Darstellung und den direkten Vergleich (intern wie extern) entwickelten viele Organisationen *Ehrgeiz*, ihre Zahlen beim nächsten Mal besser aussehen zu lassen. Jeder Beteiligte – vom Datenmanager bis zur/dem Geschäftsführer:in – konnte erstmals objektiv sehen, **wie es um die eigenen Daten bestellt ist**. Das war nicht immer bequem (schwache Stellen wurden schonungslos aufgezeigt), aber absolut notwendig für einen konstruktiven Verbesserungsprozess.

Ein paar **Beobachtungen zur Motivation**:

Viele Touristiker lieben den „sanften Wettbewerb“. Wenn Region A sieht, dass Region B eine höhere Datenqualität in bestimmten Bereichen hat, entsteht ein sportlicher Anreiz aufzuholen. Die TMBW-Berichte mit Landesdurchschnitt haben hier bewusst etwas Wettbewerb gefördert – natürlich zum Wohle aller, denn am Ende profitieren alle vom besseren Gesamtdatenpool.

Die Datenchecks machten Datenqualität zu einem **greifbaren Thema**. Statt abstrakt zu sagen „Wir müssten unsere Daten verbessern“, konnte man nun konkret diskutieren: *“Unsere Bildquote ist super, aber bei den Textlängen hinken wir hinterher – lasst uns da als Erstes ansetzen.”* Oder: *“Warum haben wir so wenige Open-Data-Einträge? Vielleicht sollten wir unsere Partner schulen, wie man Lizenzen vergibt.”* Die Berichte lieferten die Faktenbasis für solche Entscheidungen.

Einige Organisationen nutzten die Ergebnisse intern zur **Sensibilisierung** ihres Teams. Wenn ein*e Mitarbeiter*in sieht, dass z.B. 30% der Einträge seines Bereichs keine Kurzbeschreibung haben, versteht er/sie sofort den Handlungsbedarf. Die Visualisierungen machten es fast spielerisch, den eigenen Arbeitsbereich zu analysieren.

Durch die klare Auflistung der Kriterien (Minimale, gute, sehr gute Qualität) wissen alle Beteiligten jetzt, **worauf es ankommt**. Die Aussage "*Eintrag X erfüllt nur 4/7 Kriterien der Mindestqualität*" ist einprägsamer als "*Da fehlt vielleicht irgendwo was*". So entstand bei vielen ein To-do-Gefühl: Man möchte diese Häkchenliste vollständig haben.

Nicht zuletzt schaffen Erfolgserlebnisse Motivation: Wenn der nächste Check – vielleicht in einem Jahr – zeigt, dass die Textquote von 73% auf 90% gestiegen ist, kann das Team stolz darauf sein. Dieses *Feedback* spornt an, kontinuierlich dranzubleiben.

## Ausblick: Vorschläge für weiterführende Analysen

Die durchgeführten Datenchecks waren ein wichtiger Anfang, doch natürlich kann man noch tiefer gehen. Für die Zukunft bieten sich mehrere **Ansatzpunkte** an, um die Datenqualität weiter zu überwachen und zu steigern:

1. **Regelmäßiges Monitoring etablieren:** Einmal im Jahr (oder pro Quartal) einen Datenqualitätsbericht zu ziehen, würde helfen, Fortschritte zu verfolgen – und neue Lücken sofort zu erkennen. Eine kontinuierliche Messung stellt sicher, dass erreichte Verbesserungen nicht wieder verloren gehen. Denkbar ist ein **Dashboard**, in dem jede Organisation ihre Kennzahlen jederzeit einsehen kann (ähnlich einem Tacho für Datenqualität). So ein Tool könnte automatisiert Warnmeldungen geben, wenn z.B. plötzlich viele Einträge ohne Bilder auftauchen.
2. **Qualitätsranking und Best Practices:** Man könnte die Ergebnisse (behutsam) dazu nutzen, ein **Ranking** der Datenqualität zu erstellen – nicht um jemanden an den Pranger zu stellen, sondern um Erfolgsstories sichtbarer zu machen. Wenn eine Destination konstant hervorragende Datenpflege betreibt, könnte sie als **Best Practice** vorgestellt werden: *Wie schafft es Region X, 95% offene Lizenzen zu haben?* Solche Geschichten inspirieren andere und erleichtern den Wissenstransfer untereinander.
3. **Weitere Qualitätsdimensionen einbeziehen:** Die aktuellen Checks konzentrieren sich stark auf Vollständigkeit und Inhaltsqualität. Weitere **Dimensionen der Datenqualität** könnten künftig beleuchtet werden, etwa **Aktualität** (wie schnell werden Änderungen eingepflegt? Wie viele veraltete Veranstaltungen stehen noch im System?) oder **Konsistenz** der Daten. Beispielsweise könnte man prüfen, ob Ortsangaben konsistent (einheitliche Schreibweise) sind, ob es Dubletten über Regionsgrenzen hinweg gibt oder wie aktuell Öffnungszeiten sind. Solche Analysen würden das Qualitätsbild noch abrunden.
4. **Gezielte Schulungen und Hilfsmittel ableiten:** Aus den jetzigen Checks ließen sich **maßgeschneiderte Schulungen** entwickeln. Wenn klar ist, dass viele Texte zu kurz sind, bietet man einen Workshop „Wie schreibe ich gute Beschreibungstexte?“ an. Wenn Lizenzen ein Problem sind, erklärt man den Partnern nochmals die Lizenzierung im System. Auch **Hilfsmaterial** wie die bereits existierenden Checklisten oder Leitfäden können fortgeschrieben werden, konkret basierend auf den gefundenen Schwachstellen. So fließen die Analyse-Erkenntnisse direkt in Verbesserungsmaßnahmen ein.
5. **Technische Lösungen nutzen:** Einige Qualitätsprobleme lassen sich auch technisch adressieren. Beispiel: Wenn Kurzbeschreibungen fehlen, könnte das System automatisch eine gekürzte Version des Haupttextes anzeigen, bis ein manueller Text ergänzt wird. Oder ein *Lizenz-Filter* warnt den Nutzer, bevor er ein Bild ohne Lizenz hochlädt. Durch solche Features in *mein.toubiz* und *SaTourN* könnte die Datenqualität im Alltag quasi „by design“ hochgehalten werden.

## Fazit: Messung als erster Schritt zur Verbesserung

Die Datenchecks für TMBW und TMGS haben eindrucksvoll gezeigt, dass **Transparenz über den Status quo** der Datenqualität der entscheidende erste Schritt ist. Viele Touristiker hatten zuvor nur ein Bauchgefühl zur Güte ihrer Daten – nun haben sie konkrete Zahlen. Und diese Zahlen sprechen eine klare Sprache: Es gibt viel zu tun, aber es lohnt sich. Jede verbesserte Beschreibung, jedes zusätzliche Bild und jede frei lizenzierte Information erhöht die Sichtbarkeit und Attraktivität unseres Angebots im digitalen Raum.

Und bedenken Sie stets das eingangs genannte Motto: **Datenqualität kann nur verbessert werden, wenn sie auch gemessen wird.** In diesem Sinne: Packen wir es an – messen, verbessern, und unseren Gästen sowie Partnern damit ein noch besseres digitales Erlebnis bieten!

**Quellen:** Die im Text verwendeten Daten und Beispiele stammen aus den *Datenchecks 2024/2025* der TMBW (mein.toubiz) und TMGS (SaTourN), aus den Unterlagen im [Tourismusnetzwerk Baden-Württemberg](https://bw.tourismusnetzwerk.info/digitalisierung-mein-toubiz/datenmanagement/datenbank-mein-toubiz/) sowie dem [Tourismusnetzwerk Sachsen](https://sachsen.tourismusnetzwerk.info/digitales/digitalarchitektur/satourn/).

