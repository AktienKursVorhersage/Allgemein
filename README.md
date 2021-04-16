# Allgemein

Im Rahmen unserer Gruppe haben wir uns dazu entschieden, einen Aktienkurs-Verlauf vorherzusagen.

__Warum die VW-Aktie?__

- DAX-Konzern
- passender Kursverlauf mit Höhen und Tiefen
- recht stabile Entwicklung

__Auswahl der Data-Science-Methoden:__

1. Kategorie vorhersagen? - nein
2. Quantität vorhersagen? - ja

--> Regressionsanalyse

Bei der Umsetzung haben wir uns für zwei Varianten der Regressionsanalyse entschieden:
- Lineare Regression
- Polynomiale Regression

Da es bei einem Aktienkurs ebenfalls um Zeitreihendaten handelt, erschien uns die Zeitreihenanalyse als zusätzliche passende Methode. Bei der Umsetzung der Zeitreiehenanalyse fand die Analyse in zwei verschiedenen Vorhersageintervallen statt:
- tagesabhägig
- monatsabhängig

# Gliederung

1. [Regression](https://github.com/AktienKursVorhersage/Regressionsanalyse)  
    1.1 [Lineare Regression](https://github.com/AktienKursVorhersage/Regressionsanalyse/blob/main/Lineare%20Regressionsanalyse.ipynb)  
    1.2 [Polynomiale Regression](https://github.com/AktienKursVorhersage/Regressionsanalyse/blob/main/Polynomial%20Regression.ipynb)  
2. [Zeitreihenanalyse](https://github.com/AktienKursVorhersage/Zeitreihenanalyse)  
    2.1 [Tagesabhängig, Monatsabhängig](https://github.com/AktienKursVorhersage/Zeitreihenanalyse)  
3. Zusammenfassung

# Zusammenfassung

## Ergebnisse

Lineare Regression        |  Polynomiale Regression
:-------------------------:|:-------------------------:
![Lineare Regression](linear.png)  |  ![Polynomiale Regression](poly.png)

Zeitreihenanalyse mit Tagesvorhersage         |  Zeitreihenanalyse mit Monatsvorhersage
:-------------------------:|:-------------------------:
![Lineare Regression](zeitreihe-day.png)  |  ![Polynomiale Regression](zeitreihe-month.png)

## Vergleich verschiedener Ansätze

|     | Lineare Regression | Polynomiale Regression | Zeitreihenanalyse (Tagesabhängig) | Zeitreihenanalyse (Monatsabhängig) |
|:---|:---:|:---:|:---:|:---:|
| **MSE** | 959,436            | 730,269                | 8,765                             | 120,847                            |
| **MAE** | 25,832             | 19,820                 | 2,041                             | 8,102                              |
| **R2**  | 0,714              | 0,782                  | 0,972                             | 0,579                              |
