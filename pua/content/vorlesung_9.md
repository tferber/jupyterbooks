# Vorlesung 9: Sortieren, lineare Gleichungssysteme und Interpolation

```{admonition} Hier geht zum Quiz...
:class: tip
<!--[Quiz zum Thema "Strings"](jupyterquiz/quiz_strings)-->

```

## Was Sie wissen sollten
* Suchalgorithmen sind eine der wichtigsten numerischen Anwendungen. Viele verschiedene Methoden existieren mit unterschiedlichen Stärken und Schwächen.
    ** Welche Sortieralgorithmen gibt es? Welche eigenen sich besonders gut oder besonders schlecht für unterschiedliche Anwendungen (z.B. sehr lange oder sehr kurze Listen, Listen die bereits fast sortiert sind, Listen die nur Ganzzahlen enthalten, ...)
* Die Komplexität eines Algorithmus gibt an, wie sich der Algorithmus im Grenzfall ￼ im Bezug auf Ausführungszeit oder Speicherbedarf verhält. Sie wird i.A. durch die “Big-O-Notation” angegeben.  
    ** Wie messen sie die Zeitkomplexität oder die Speicherkomplexität? (vgl. VL8 mit Details zur Zeitmessung und Messung des Speicherbedarfs)
* Lineare Gleichungssysteme (LGS) können numerisch z.B. durch das Gaußverfahren gelöst werden.
    ** Was sind Vor- und Nachteile des Gaußverfahrens? Ist das Verfahren immer numerisch stabil? Ist es immer anwendbar? (Was passiert bei sehr großen LGS?)
* Messwerte müssen Interpoliert werden um analytisch differenzierbare oder integrierbare Funktionen zu erhalten. Eine gängige Methode sind kubische Splines für die ein (großes) lineares Gleichungssystem gelöst werden muss.
    ** Neben kubischen Splines gibt es auch andere Methoden der interpolation - welche?
    ** Interpolation beschreibt Methoden zwischen bekannten Messwerten eine analytische Funktion zu erhalten. Extrapolation beschreibt das fortführen einer analytischen Funktion unter- und oberhalb der bekannten Messwerte. Was müssen sie hier beachten?
