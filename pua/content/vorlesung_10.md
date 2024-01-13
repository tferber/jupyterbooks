# Vorlesung 10: Numerische Integration und Differentialgleichungssysteme

```{admonition} Hier geht zum Quiz...
:class: tip
<!--[Quiz zum Thema "Strings"](jupyterquiz/quiz_strings)-->

```

## Was Sie wissen sollten
* Numerische Lösungen von Integralen und Differentialgleichungen sind zwei der wichtigsten Anwendungen für Numerik in der Physik
    * u.a. (hochdimensionale) Wahrscheinlichkeitsdichtenm in der Datenanalyse, Matrixelemente in der Teilchenphysik, Black-Scholes-Merton-Gleichung in der Finanzmathematik, Navier-Stokes-Gleichung in der Strömungsmechanik, Finite-Elemente (z.B. Wärmefluss in Festkörpern, mechanische Belastung komplizierter Formen, …)
* Numerische Integrationsmethoden beinhalten u.a. Monte Carlo Verfahren und das Newton-Cotes Verfahren (mit Trapez- und Simpson-Regel)
    * Was sind Limitierungen der Monte Carlo Verfahren und des Newton-Cotes Verfahrens?
* Bei allen numerischen Methoden ist es wichtig zumindest eine Abschätzung des Verfahrensfehlers zu erhalten
    * Wie kann man den Verfahrensfehler reduzieren?
* Differentialgleichungen sind numerisch durch kleine Zeitschritte zu lösen. Das Runge-Kutta Verfahren vierter Ordnung (auch “RK4”) ist ein gängiges Verfahren dieser Art
    * Welche anderen Runge-Kutta Verfahren gibt es? Welche algorithmische Komplexitǎt haben diese Verfahren?
* Differentialgleichungen höherer Ordnung kann man auf ein System von DGLs erster Ordnung umformen
    * Kann man dies immer tun? Was ist mit nichtlinearen Differentialgleichungen?
