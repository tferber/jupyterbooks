# Vorlesung 8: import, Kommandozeile, Zeichenketten und Debugging

```{admonition} Hier geht zum Quiz...
:class: tip
[Quiz zum Thema "Strings"](jupyterquiz/quiz_strings)

```

## Was Sie wissen sollten
* import erweitert die Standard-Python Funktionalität und Python erlaubt Ihnen auch eigene Module zu importieren
    * Wie importieren sie eigene Module? Was passiert wenn sie ein Modul mehrfach importieren? Wie lösen sie zirkuläre imports? Was passiert wenn verschiedene Module die gleichen Methoden bereitstellen?
* Oftmals werden Programmen Variablen über die Kommandozeile übergeben, argparse ist ein flexibles Werkzeug hierfür
    * Wie legen sie fest welchen Variablentyp der argparse Parameter hat? Wie übergeben sie eine Liste mit argparse? Was bedeutet "store_true" (sog. on/off flags)?
* Zeichenketten können mit in, find() oder regular expressions durchsucht werden, und mit split() in einzelne Tokens geteilt werden
* Techniken zur Fehlersuche und -behebung in Python umfassen Assertions, Logging, die Messung der Ausführungsdauer und die Überwachung des Speicherverbrauchs sowie interaktive Debugger wie pdb
    * Wie benutzen sie pdb um den aktuellen Wert einer Variable auszugeben? Was sind breakpoints? 
