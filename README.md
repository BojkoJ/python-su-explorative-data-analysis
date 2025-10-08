# SU (Strojové Učení) - Cvičení 2: Exploratory Data Analysis

Tento repozitář obsahuje řešení 2. cvičení z předmětu Strojové učení.

https://homel.vsb.cz/~pla06/subject_ml.html - Exercise 2


Tento projekt obsahuje Explorativní Datovou Analýzu (EDA) datasetu `Fighters Stats.csv`, který pokrývá širokou škálu statistik zápasníků UFC. Výsledky analýzy jsou zdokumentovány v notebooku `eda.ipynb`.

## Obsah repozitáře

-   `Fighters Stats.csv` – zdrojový dataset se statistikami zápasníků.
-   `eda.ipynb` – Jupyter notebook s kompletní EDA, vizualizacemi a škálováním vybraných proměnných.
-   `README.md` – tento soubor s přehledem a instrukcemi.

## Požadavky

-   Python 3.9+
-   Doporučené balíčky:
    -   pandas
    -   numpy
    -   matplotlib
    -   seaborn
    -   scikit-learn

Potřebné knihovny lze doinstalovat globálně pomocí:

```powershell
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Jak spustit notebook

1. Otevřete terminál v kořenové složce projektu `c:/Users/roryb/Desktop/SU/2`.
2. Spusťte Jupyter (např. VS Code, JupyterLab nebo `jupyter notebook`).
3. Otevřete `eda.ipynb` a postupně vykonejte všechny buňky.

Notebook je strukturován do sekcí:

1. **Načtení dat a knihoven** – importy a základní přehled.
2. **Základní přehled datasetu** – první řádky, datové typy a deskriptivní statistiky.
3. **Chybějící hodnoty** – kontrola a report nulových hodnot.
4. **Vizualizace kategoriálních atributů** – rozložení pohlaví, postojů, stylů a vah.
5. **Analýza numerických statistik** – histogramy, korelace a porovnání podle pohlaví.
6. **Min-Max škálování** – škálování numerických atributů pomocí `MinMaxScaler` a porovnání původních vs. škálovaných hodnot.
7. **Shrnutí a doporučení** – klíčové poznatky a návrhy na pokračování.

## Rychlé výsledky

-   Dataset obsahuje 2581 zápasníků bez chybějících hodnot.
-   Dominují mužští zápasníci, nejčastější postoj je Orthodox, styl Striker.
-   Výkonnostní metriky vykazují různá rozložení; korelace odhalila vazby mezi časem v boji (`Ctrl`, `Round`) a úspěšností (`W`, `STR`).
-   Min-Max škálování usnadňuje porovnávání zápasníků napříč metrikami a je k dispozici v rozšířeném DataFrame.
