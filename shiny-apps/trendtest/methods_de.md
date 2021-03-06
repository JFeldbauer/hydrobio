---
title: "Wissenschaftliche Grundlagen und Aufgaben"
output: 
  html_document:
    keep_md: true
    code_folding: hide
bibliography: references.bib    
---


# Wissenschaftliche Grundlagen

## linearer Trend

Ein einfaches lineares Regressionsmodell kann als:

  $$ \hat{y}_i = a + b \cdot x_i $$

geschrieben werden. Wobei $\hat{y}_i$ die geschätzten Werte der abhängigen Variable, $x_i$ die unabhängige Variable, $a$ der Schnittpunkt mit der y-Achse und $b$ die Steigung der Geraden sind. Um die Parameter $a$ und $b$ zu ermitteln wird normalerweise die Summe der Abweichungsquadrate minimiert.

### Residuen

Als Ressiduen $r_i = y_i - \hat{y}_i$ werden die Differenz zwischen den gemessenen Werten $y_i$ und den geschätzten Werten $\hat{y}_i$ bezeichnet.

### Voraussetzungen linearer Trend

Das einfache lineare Modell geht davon aus dass:

 1. Die unabhängige Variable $x$ deterministisch ist (fest gegeben)
 2. Für jedes $x_i$ ist $y_i$ eine Zufallsvariable
 3. Die $y_i$ sind unabhängig voneinander (keine Autokorelation) und identisch verteilt (jedes $y_i$ hat die gleiche Verteilung)
 4. Die Residuen $r_i$ sind normalverteilt
  
## LOESS Glätter

LOESS steht für locally estimated scatterplot smoothing, zu deutsch: lokal gewichteter Regressions-Streudiagramm-Glätter. Glätter werden verwendet,um eine Ausgleichslinie durch einen verrauschten Datensatz zu erhalten, z.B. zur bloßen Visualisierung des  "Trends"  in  einem  Diagramm,  zur  Abtastung  des  mittleren  Verlaufes  oder  auch  zur  Schätzung  von Vertrauensintervallen.

## Mann-Kendall Test

Der Mann-Kendall Test ist ein Test für monotone Trends in einer Zeitreihe, basierend auf der Kendall Rangkorrelation der Zeitreihe. Dabei wird die Stärke des monotonen Zusammenhangs zwischen einer abhängigen und unabhängigen Variable getestet. Der Test ist besonders in den Umweltwissenschaften beliebt, da die Bewertungs-Funktion $S$ für kleine $n$ nahezu normalverteilt ist.


# Literaturverzeichis

Hipel, K.W. and McLeod, A.I., (2005). Time Series Modelling of Water Resources and Environmental Systems. Electronic reprint of our book orginally published in 1994. http://www.stats.uwo.ca/faculty/aim/1994Book/.

Kendall, M.G. (1976). Rank Correlation Methods. 4th Ed. Griffin.

Petzoldt, T. (2019). Datenanalyse mit R Ausgewählte Beispiele - Skript. https://wwwpub.zih.tu-dresden.de/~petzoldt/elements_de.pdf
