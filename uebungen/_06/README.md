# Layoutschulung SH
## LAY06 Layout Bundle anlegen

### Anlegen des Bundles
1. Erstellen sie innerhalb des bundles Verzeichnis in Visual Studio Code einen Ordner mit dem Namen alternatelayout.

2. Entpacken sie die Datei alternatelayout.zip aus dem Trainings Verzeichnis in den, im Schritt 1 erstellten Ordner.



*app.json*
```javascript
{
    "widgetRole": "coordinateviewer",
    "sublayout": ["tablet_landscape","tablet_portrait","mobile_landscape","mobile_portrait"],
    "attachTo": "map_bottomleft"
}
```

2. Laden Sie die App im Browser neu und verändern sie die Größe des Browserfensters um die Größe eines mobilen Clienten zu simulieren.

3. Öffnen sie erneut die ***app.json*** und fügen sei folgenden Codeblock ein.

*app.json*
```javascript
{
    "widgetRole": "printing",
    "sublayout": ["tablet_landscape","tablet_portrait"],
    "window": {
        "draggable": false,
        "dndDraggable": false,
        "marginBox": {
            "l": 20,
            "w": 300,
            "t": 120,
            "b": 60
        }
    }
}
```
4. Laden Sie die App im Browser neu und verändern sie die Größe des Browserfensters um die Größe eines mobilen Clienten zu simulieren.

### Ergebnis
Die Koordinatenanzeige befinden sich für Browserbreiten zwischen 800px und 1000px unten links. Ansonten oben rechts. Außerdem verändert sich das Verhalten des Fenster für die Drucken Funktion abhängig von der Browserfenstergröße.


