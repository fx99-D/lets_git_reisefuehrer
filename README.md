# Der Reiseführer zum MOOC "Let's Git - Versionsverwaltung und Open Source"

Hier sammeln wir die Lieblingsorte der Teilnehmer:innen des Kurses Let's Git - Versionsverwaltung und Open Source. Beiträge sind sehr willkommen! Wenn Du Änderungen oder neue Inhalte hinzufügen möchten, öffne bitte ein Issue oder erstelle einen Pull Request.

## Einen neuen Eintrag hinzufügen

Wenn du einen Ort hinzufügen möchtest, dann erstelle ein Issue und beschreibe diesen kurz. Anschließend kannst du den Reiseführereintrag schreiben (wie in [Beispielort.md](Beispielort.md) beschrieben) und mit einem Pull Request einreichen. Bitte achte darauf, dass du den Ort in den richtigen Ordner einordnest (Bitte bis auf Länderebene, also Berlin in Europa/Deutschland/Berlin.md) und schön mit Markdwon formatierst.
Um Deinen Ort leichter finden zu können, bietet es sich an, diesen in die interaktive Karte (siehe unten) aufzunehmen.

## Struktur dieses Projekts ändern

Dieses Projekt ist auf die Schnelle entstanden und ist nicht perfekt. Falls du Vorschläge zur besseren Organisation hast, erstelle ein Issue und dann kann dort gemeinsam diskutiert werden.

## Wie läuft ein Pull Request Review?

Da ich nicht alle Orte ausführlich durchlesen kann, ist jeder Pull Request Review willkommen, um Rechtschreibfehler und mehr zu erkennen. Ich werde dann deinen Einreich mergen.

## Maintainer gesucht

Ich kann hier nicht über alle Let's Git Repositories alles überblicken, weswegen ich mich freuen würde wenn wir bis zu 5 Maintainer für dieses Projekt finden. Gerne kann dafür in einem Issue diskutiert werden.

## Ort in die interaktive Karte aufnehmen
Das Einfügen von neuen Orten in die interaktive Karte geht folgendermaßen:
* Bestimmung der geographischen Koordinaten z.B. mit Wikipedia. Hier sind die geographischen Koordinaten immer rechts oben in der Seite aufgeführt.

  <img src="https://github.com/fx99-D/lets_git_reisefuehrer/blob/update_README2/Worldmap/Koordinaten-Wikipedia.JPG"/>
  
  Beim Klicken auf die Koordinaten geht eine weitere Seite auf. Hier findet man ebenfalls rechts oben die Koordinaten in Dezimalschreibweise, wie sie benötigt werden.
  
  <img src="https://github.com/fx99-D/lets_git_reisefuehrer/blob/update_README2/Worldmap/Koordinaten-Geohack.JPG"/>
* In der Datei Worldmap/WorldMap.htm an der Stelle 
``` 
// hier weitere Lokalitäten ergänzen
  L.marker({lon: 16.373, lat: 48.208}).bindPopup('Wien<br><a href="https://de.wikipedia.org/wiki/Wien">Wikipedia</a>').addTo(map);
  L.marker({lon: 149.117, lat: -35.3}).bindPopup('Canberra<br><a href="https://de.wikipedia.org/wiki/Canberra">Wikipedia</a>').addTo(map);
```
    Zeile einfügen und Koordinaten sowie Stadtname und Link entsprechend setzen.

    Achtung: gegenüber der Geo URI 	geo Darstellung sind die Koordinaten vertauscht.
      
* Die Datei Worldmap/WorldMap.htm sollte mit jedem aktuellen Browser darstellbar sein.
