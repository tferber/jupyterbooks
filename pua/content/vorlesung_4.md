# Vorlesung 4: Datenstrukturen

```{admonition} Hier geht zum Quiz...
:class: tip
[Quiz zum Thema "Listen"](jupyterquiz/quiz_listen)

[Quiz zum Thema "Datenstrukturen und Funktionen"](jupyterquiz/quiz_datenstrukturen_und_funktionen)

[Quiz zum Thema "Dictionaries, Sets, Tuples"](jupyterquiz/quiz_dictionaries)

```

```{admonition} Beispiele und Vertiefung
:class: seealso
[Jupyter Notebook zum Thema "Verschachtelte Listen"](4_nestedlistcomprehension.ipynb)

[Jupyter Notebook zum Thema "Bedingungen und Listen"](4_listcomparison.ipynb)

[Jupyter Notebook zum Thema "Reverse Lookup mit Dictionaries"](4_reverselookup.ipynb)

[Jupyter Notebook zum Thema "Globale Variablen"](4_global.ipynb)

[Jupyter Notebook zum Thema "Mengenoperationen auf Sets"](4_set_operations.ipynb)
```

## Datenstrukturen
### Listen:

* Listen sind geordnete Sammlungen von Elementen.
* Listen sind veränderbar, d.h. Sie können ihren Inhalt ändern.
* Die Elemente in einer Liste werden von 0 an indiziert.
* Listen werden definiert, indem die Elemente in eckige Klammern [] eingeschlossen und durch Kommata getrennt werden.
* Typischer Anwendungsfall: Verwenden Sie Listen, wenn die Reihenfolge der Elemente wichtig ist und wenn Elemente möglicherweise geändert werden müssen.

### Dictionaries:
* Dictionaries sind ungeordnete Sammlungen von Schlüssel-Werte-Paaren.
* Dictionaries sind veränderbar.
* Der Zugriff auf Werte in einem Wörterbuch erfolgt über Schlüssel, nicht über Indizes.
* Wörterbücher werden definiert, indem die Schlüssel-Wert-Paare in geschweifte Klammern {} eingeschlossen werden, wobei die Paare durch Kommas und Schlüssel und Wert durch einen Doppelpunkt getrennt werden:.
* Typischer Anwendungsfall: Verwenden Sie Dictionaries, wenn Sie eine logische Assoziation zwischen einem Schlüssel:Wert-Paar benötigen.

### Tuple:
* Tuple sind geordnete Sammlungen von Elementen.
* Tuple sind unveränderlich, d. h. ihr Inhalt kann nach der Erstellung nicht mehr geändert werden.
* Die Elemente in einem Tuple werden von 0 an indiziert.
* Tuple werden definiert, indem die Elemente in Klammern () eingeschlossen und durch Kommata getrennt werden.
* Typischer Anwendungsfall: Verwenden Sie Tuple, wenn die Reihenfolge der Elemente wichtig ist und die Elemente nicht geändert werden sollen.

### Sets:
* Sets sind ungeordnete Sammlungen eindeutiger Objekte.
* Sets sind veränderbar, können aber nur immutable Objekte enthalten.
* Sets unterstützen keine Indizierung oder Slicing.
* Sets werden definiert, indem die Elemente in geschweifte Klammern {} eingeschlossen und durch Kommata getrennt werden. Alternativ können Sie auch die Funktion set() verwenden, um eine Set zu erstellen.
Typischer Anwendungsfall: Verwenden Sie Sets, wenn Sie mehrere Elemente in einer einzigen Variablen speichern möchten und wenn Sie sich um die Einzigartigkeit der Elemente und nicht um ihre Reihenfolge kümmern.

## Was Sie wissen sollten
* Datenstrukturen erlaubten die effiziente Anordnung von Werten und Operationen mit diesen
    Welche Operationen sind für die verschiedenen Datenstrukturen erlaubt?
* Wir unterscheiden in immutable (nach dem Erzeugen unveränderbare) und mutable (nach dem Erzeugen veränderbare) Datenobjekte
* Über Datenstrukturen können sie mit for-Schleifen iterieren
    * Wie genau lautet die Syntax hierfür? Unterscheidet sie sich für verschiedene Datenstrukturen? Wie prüfen sie mit dem `in`-Operator ob eine Datenstruktur ein bestimmtes Element enthält?
* List-comprehensions sind eine effiziente Art map und filter Operationen durchzuführen
    * Was ist die Syntax für list-comprehensions? Funktioniert das auch für Sets, Tuples, oder Dictionaries? Wie funktioniert List-comprehension für verschachtelte Listen?
* Listen, Dictionaries, Tuple, und Sets haben verschiedene Vor- und Nachteile
    * Welche Vor- und Nachteile sind das?
* Verwenden sie NIEMALS mutable Datenobjekte als optionale Funktionsargumente!
    * Warum ist es riskant mutable Datenobjekte als optionale Funktionsargumente zu verwenden? In welcher Reihenfolge müssen optionale Funktionsargumente angebenen werden? Wie funktionert \* gather von Argumenten?


<!--## Videos to watch...-->
<!--::::{grid}-->
<!--:class-container: text-center-->
<!--:gutter: 3-->
<!---->
<!--:::{grid-item-card}-->
<!--:columns: 5-->
<!--:class-header: bg-light-->
<!--Facts and Myths about Python names and values - PyCon 2015 (Ned Batchelder)-->
<!---->
<!--<iframe width="200" height="113" src="https://www.youtube.com/embed/_AEJHKGk9ns" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>-->
<!--:::-->
<!---->
<!--:::{grid-item-card}-->
<!--:columns: 5-->
<!--:class-header: bg-light-->
<!--The PEP 8 Song (Leon Sandøy)-->
<!---->
<!--<iframe width="200" height="113" src="https://www.youtube.com/embed/hgI0p1zf31k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>-->
<!--:::-->
<!---->
<!---->
<!--::::-->

