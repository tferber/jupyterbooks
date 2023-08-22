# Vorlesung 2

```{admonition} Hier geht zum Quiz...
:class: tip
[Quiz zum Thema "Variablen"](jupyterquiz/quiz_variablen.ipynb)

[Quiz zum Thema "f-strings"](jupyterquiz/quiz_fstrings.ipynb)

[Quiz zum Thema "void-Funktionen"](jupyterquiz/quiz_funktionen_1.ipynb)
```

<!--## Download Vorlesungsfolien-->
<!---->
<!--{Download}`Hier<slides/V2.pdf>` können sie die Vorlesungsfolien zur Vorlesung 2 herunterladen.-->

## Warum sollten Sie Code dokumentieren und kommentieren?
* Lesbarkeit: 
    * Kommentare verbessern die Lesbarkeit Ihres Codes, indem sie Kontext liefern und erklären, was jeder Teil des Codes tut. Dies ist besonders hilfreich bei komplexen Algorithmen oder komplizierter Logik.
* Wartbarkeit: 
    * Kommentare helfen bei der Pflege des Codes. Wenn Sie Ihren Code in Zukunft aktualisieren oder ändern müssen, helfen Ihnen die Kommentare dabei, die einzelnen Teile des Codes zu verstehen.
* Kollaboration: 
    * Wenn Sie in einem Team arbeiten, helfen Kommentare Ihren Teamkollegen, Ihren Code zu verstehen. Dies ist entscheidend für eine effektive Zusammenarbeit und die Produktivität des Teams.
* Fehlersuche:
    * Wenn etwas schief geht, können Kommentare Ihnen helfen, den Ablauf Ihres Codes zu verstehen und die Fehlersuche zu erleichtern.
* Lernen: 
    * Wenn Sie ein/e Anfänger\*in sind oder versuchen eine neue Programmiersprache zu verstehen, können Kommentare sehr lehrreich sein und einen guten Einblick in die Funktionsweise des Codes geben.
    
* Mehr Informationen in [PEP8 - Style Guide for Python Code](https://peps.python.org/pep-0008/) und [PEP257 - Docstring Conventions](https://peps.python.org/pep-0257/).


## Was Sie wissen sollten
* Variablen sind Namen die Objekten z.B. mit dem Assignment-Operator “=“ zugewiesen werden
    * Was ist der Unterschied zwischen den Gleichheitszeichen in der Mathematik und dem Assignment-Operator in Python?
* Variablen referenzieren immer Werte. Variablen referenzieren niemals Variablen.
    * Kann die gleiche Variable gleichzeitig verschiedene Werte referenzieren? Kann sie nacheinander verschiedene Werte referenzieren? Kann eine Variable auf eine andere Variable referenzieren?
* Um andere Variablen in Zeichenketten zu verwenden, nutzen sie` f-strings`.
    * Welche anderen Methoden gibt es? Warum sollten sie `f-strings` bevorzugen? Wie beschränkt man die Zahl der Nachkommastellen von Gleitkommazahlen (`float`) und warum ist das wichtig?
* Für wiederkehrende Anweisungen bietet es sich an Funktionen selbst zu schreiben
    * Was genau ist eine `void`-Funktion? Was ist der Rückgabewert einer `void`-Funktion? Was sind Header und Body einer Funktion? Welche Argumente können sie einer Funktion übergeben? Können sie eine Variable, die sie ausserhalb einer Funktion definiert haben, auch innerhalb einer void-Funktion ändern so dass sie auch ausserhalb der Funktion geändert ist?
* Code muss so dokumentiert, dass die Intention klar ist. Jede Funktion (Modul, Klasse, Methode) muss mit einem docstring versehen sein.
    * Gute Dokumentation braucht Erfahrung - dokumentieren sie am Anfang eher zu viel als zu wenig.

## Videos to watch...
::::{grid}
:class-container: text-center
:gutter: 3

:::{grid-item-card}
:columns: 5
:class-header: bg-light
Facts and Myths about Python names and values - PyCon 2015 (Ned Batchelder)

<iframe width="200" height="113" src="https://www.youtube.com/embed/_AEJHKGk9ns" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
:::

:::{grid-item-card}
:columns: 5
:class-header: bg-light
The PEP 8 Song (Leon Sandøy)

<iframe width="200" height="113" src="https://www.youtube.com/embed/hgI0p1zf31k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
:::


::::

