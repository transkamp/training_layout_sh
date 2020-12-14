# Layoutschulung SH
## LAY04: Widget innerhalb der Anwendung umpositionieren

1. Öffnen Sie die manuelle Konfiguration Ihrer App ***"sample"*** und ergänzen Sie die Konfiguration im Abschnitt ***templates*** um den unten stehenden Codeblock:

*app.json*
```json
"widgets": [
    {
    ...
    },
    {
       "widgetRole":"coordinateviewer",
       "attachTo": "map_topright",
       "cssClass": "background-highlight padding-default"
    }
]
```

3. Laden Sie die App im Browser neu öffnen sich das Fenster für die Druck-Funktion.

### Ergebnis
Die Koordinatenanzeige befinden sich nicht mehr in der Fußzeile der Anwendung sondern in der rechten oberen Ecke der Karte. Außerdem hat sie einen farbigen Hintergrund.





