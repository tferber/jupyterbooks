# Vorlesung 7: Programmentwurf und Fortgeschrittene Methoden

```{admonition} Hier geht zum Quiz...
:class: tip
[Quiz zum Thema "Generatoren"](jupyterquiz/quiz_generators)

[Quiz zum Thema "Lambda-Funktionen"](jupyterquiz/quiz_lambda)

```

```{admonition} Beispiele und Vertiefung
:class: seealso
[Jupyter Notebook zum Thema "Generators and Data Pipelines"](7_generators_datapipeline.ipynb)

[Jupyter Notebook zum Thema "Generators Expressions"](7_generator_expression.ipynb)
```

<!--## Was Sie wissen sollten-->
## The Zen of Python, by Tim Peters

* Beautiful is better than ugly.
    * Das bedeutet, dass Python-Code ästhetisch ansprechend, klar und elegant sein sollte. Er sollte unnötige Komplexität, Unordnung oder Unklarheit vermeiden.

* Explicit is better than implicit.
    * Das bedeutet, dass Python-Code explizit und einfach sein sollte, anstatt sich auf implizite oder versteckte Funktionen zu stützen. Er sollte Zweideutigkeit und Verwirrung vermeiden und die Absichten und Annahmen des Programmierers deutlich machen.

* Simple is better than complex.
    * Das bedeutet, dass Python-Code einfach und leicht zu verstehen sein sollte, anstatt komplex und schwer zu folgen. Er sollte unnötige Abstraktion, Komplikationen oder Raffinesse vermeiden.

* Complex is better than complicated.
    * Das bedeutet, dass Python-Code, auch wenn eine gewisse Komplexität unvermeidlich ist, dennoch organisiert und strukturiert sein sollte und nicht chaotisch und unordentlich. Er sollte willkürliche oder inkonsistente Regeln vermeiden und einer kohärenten Logik und Gestaltung folgen.

* Flat is better than nested.
    * Das bedeutet, dass Python-Code flach und linear sein sollte und nicht verschachtelt und hierarchisch. Er sollte übermäßige Einrückungsebenen, Verschachtelungen oder Verzweigungen vermeiden, die das Lesen und Debuggen des Codes erschweren können.

* Sparse is better than dense.
    * Es sollte vermieden werden, zu viele Elemente oder Anweisungen in eine Zeile oder einen Block zu packen, und Leerzeichen und Leerzeilen sollten verwendet werden, um sie zu trennen und zu gruppieren.

* Readability counts.
    * Python-Code sollte lesbar und verständlich sein, nicht nur für den/die Programmierer\*in, der/die ihn geschrieben hat, sondern auch für andere Programmierer\*innen, die ihn möglicherweise verwenden oder ändern müssen. Er sollte gängigen Konventionen und Standards folgen und sinnvolle Namen und Kommentare verwenden.

* Special cases aren't special enough to break the rules.
    * Python-Code sollte den allgemeinen Grundsätzen und Richtlinien folgen, anstatt Ausnahmen oder Sonderfälle für bestimmte Situationen zu machen. Er sollte Inkonsistenz und Unvorhersehbarkeit vermeiden und die etablierten Normen und Erwartungen der Sprache respektieren.

* Although practicality beats purity.
    * Das bedeutet, dass Python-Code praktisch und realistisch sein sollte, statt rein und idealistisch. Er sollte die Beschränkungen und Kompromisse der realen Welt anerkennen und sich bei Bedarf an sie anpassen. Er sollte nicht die Funktionalität oder Benutzerfreundlichkeit zugunsten von Perfektion oder Eleganz opfern.

* Errors should never pass silently.
    * Python-Code sollte Fehler und Ausnahmen richtig behandeln, anstatt sie zu ignorieren oder zu unterdrücken. Er sollte den/die Programmierer\*in oder den/die Benutzer\*in warnen, wenn etwas schief läuft, und nützliche Informationen oder Rückmeldungen liefern.

* Unless explicitly silenced.
    * Das bedeutet, dass Python-Code Fehler oder Ausnahmen absichtlich zum Schweigen bringen kann, aber nur, wenn es dafür einen guten Grund gibt und wenn dies ausdrücklich und absichtlich geschieht. Er sollte Fehler (“errors”) oder Ausnahmen (“exceptions”) nicht standardmäßig oder versehentlich unterdrücken.

* In the face of ambiguity, refuse the temptation to guess.
    * Das bedeutet, dass Python-Code nicht versuchen sollte, zu erraten oder anzunehmen, was der/die Programmierer\*in oder der/die Benutzer\*in will oder erwartet, wenn es mehr als eine mögliche Interpretation oder ein Ergebnis gibt. Er sollte Mehrdeutigkeit und Unsicherheit vermeiden und Klarheit und Gewissheit verlangen.

* There should be one-- and preferably only one --obvious way to do it.
    * Python-Code sollte eine klare und offensichtliche Lösung für jedes Problem oder jede Aufgabe haben und nicht mehrere obskure oder verwirrende Alternativen. Er sollte Redundanz und Doppelungen vermeiden und Konsistenz und Einfachheit fördern.

* Although that way may not be obvious at first unless you're Dutch.
    * Dies ist eine humorvolle Anspielung auf Guido van Rossum, den Schöpfer von Python, der Niederländer ist. Es impliziert, dass einige Aspekte von Python auf den ersten Blick nicht offensichtlich oder intuitiv sind, aber sie ergeben Sinn, wenn man mehr über sie erfährt.

* Now is better than never.
    * Python-Code sollte so schnell wie möglich geschrieben und ausgeführt werden, anstatt ihn auf unbestimmte Zeit zu verschieben oder zu verzögern. Es ermutigt zum Handeln und Experimentieren, statt zum Zögern und Zaudern.

* Although never is often better than \*right\* now.
    * Das bedeutet, dass Python-Code nicht voreilig oder unbedacht geschrieben oder ausgeführt werden sollte, ohne angemessene Planung oder Tests. Letzteres entmutigt Impulsivität und Nachlässigkeit, die zu Fehlern oder Bugs führen können.

* If the implementation is hard to explain, it's a bad idea.
    * Python-Code sollte leicht zu erklären und zu verstehen sein, nicht nur für den/die Programmierer\*in, der/die ihn geschrieben hat, sondern auch für andere Programmierer\*innen, die ihn möglicherweise verwenden oder ändern müssen. Wenn der Code schwer zu erklären ist, ist er wahrscheinlich schlecht entworfen oder implementiert.

* If the implementation is easy to explain, it may be a good idea.
    * Python-Code kann eine gute Idee sein, wenn er leicht zu erklären und zu verstehen ist, aber das ist keine Garantie dafür, dass er immer eine gute Idee ist. Es impliziert, dass es andere Faktoren oder Kriterien geben kann, die bei der Bewertung der Qualität oder Eignung des Codes zu berücksichtigen sind.

* Namespaces are one honking great idea -- let's do more of those!
    * Dies ist eine positive und enthusiastische Befürwortung von Namespaces, einer Funktion von Python, die es Programmierer\*innen ermöglicht, die Namen von Variablen, Funktionen, Klassen, Modulen und anderen Elementen in ihrem Code zu organisieren und zu verwalten. namespaces helfen, Namenskonflikte und -kollisionen zu vermeiden und verbessern die Modularität und Lesbarkeit.

## Was Sie wissen sollten
* Lambda-Funktionen können den Code einfacher und eleganter machen, indem sie die Notwendigkeit vermeiden, eine separate Funktion zu definieren und zu benennen.
    * Wie schreiben sie Lambda-Funktionen? Wann setzen sie sie ein, und wann besser nicht? Was sind die Limitierungen von Landa-Funktionen?
* Ein Generator ist eine besondere Art von Funktion, die einen sog. Iterator zurückgibt, der eine Folge von Werten erzeugt, wenn er durchlaufen wird.
    * Welchen Vorteil bieten Generatoren - und welche Nachteile?
* Dekoratoren sind eine Möglichkeit, das Verhalten einer Funktion oder einer Klasse zu ändern, ohne den ursprünglichen Code zu verändern.
    * Was sind typische Anwendungen von Dekoratoren? Wie schreibt man sie, und wie setzt man sie ein?
* Python bitweise Operatoren werden verwendet, um Operationen auf einzelnen Bits von Ganzzahlen durchzuführen, die im Binärformat dargestellt werden.
    * Wie werden ganze Zahlen im Computer dargestellt? Was ist das Zweierkomplement? Wie werden negative Zahlen im Computer dargestellt?

* Programmentwurf ist der Prozess der Entwicklung und Definition von Softwarelösungen für ein Problem
* Beim Programmdesign geht es darum, den Zweck des Programms, seine Eingaben, Ausgaben und Verarbeitung zu verstehen und ein Modell des Programms zu erstellen
* Zu den Entwurfswerkzeugen gehören 
    * Flussdiagramme, die die Logik und den Fluss eines Programms grafisch darstellen
    * Skeleton Code (eine Vorlage oder ein Rahmen, der die grundlegende Struktur und Funktionalität eines Programms bietet
    * Pseudocode, eine vereinfachte und informelle Version des Codes, der den Algorithmus beschreibt
* Bei der Programmentwicklung können je nach Art und Komplexität des Problems und der Lösung verschiedene Programmierparadigmen zum Einsatz kommen, wie z. B. objektorientierte oder funktionale Programmierung

## Download Vorlesungsfolien

{Download}`Hier <https://ilias.studium.kit.edu/goto.php?target=fold_2215340&client_id=produktiv>` können sie die Vorlesungsfolien zur Vorlesung 7 herunterladen.

