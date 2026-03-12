# Analiza i Predykcja Cen Samochodów Używanych w Polsce

Projekt przedstawia analizę rynku samochodów używanych w Polsce oraz próbę przewidywania cen na podstawie cech pojazdu i danych ogłoszeniowych. Całość została wykonana w formie notebooka Jupyter i obejmuje przygotowanie danych, analizę eksploracyjną, wizualizacje oraz budowę modeli regresyjnych.

## Zakres projektu
- wczytanie i wstępna analiza danych,
- czyszczenie oraz przygotowanie zbioru,
- analiza braków danych i statystyk opisowych,
- wizualizacja zależności między cechami a ceną,
- predykcja cen samochodów z użyciem modeli ML,
- porównanie jakości modeli.

## Dane
W projekcie wykorzystano zbiór danych **Car Prices in Poland** pobrany z Kaggle. Dane zawierają m.in. informacje o:
- marce i modelu,
- generacji pojazdu,
- roku produkcji,
- przebiegu,
- pojemności silnika,
- rodzaju paliwa,
- lokalizacji ogłoszenia,
- cenie.

## Zawartość notebooka
Notebook prowadzi przez cały proces analityczny:
1. **Analiza eksploracyjna danych (EDA)** – podstawowe informacje o zbiorze, braki danych, statystyki opisowe i korelacje.
2. **Przygotowanie danych** – uzupełnianie braków, filtrowanie błędnych rekordów, uproszczenie części zmiennych.
3. **Wizualizacja danych** – histogramy, boxploty, wykresy słupkowe, wykresy rozrzutu i mapy ciepła.
4. **Uczenie maszynowe** – przygotowanie cech, kodowanie zmiennych kategorycznych i trening modeli.

## Zastosowane modele
W projekcie porównano dwa podejścia do regresji:
- **Regresja liniowa**
- **Drzewo regresyjne**

### Wyniki
- **Regresja liniowa**: MAE ≈ **23 133 PLN**, R² ≈ **0.778**
- **Drzewo regresyjne**: MAE ≈ **9 481 PLN**, R² ≈ **0.931**

Wyniki pokazują, że model drzewa regresyjnego znacznie lepiej odwzorował zależności występujące w danych niż klasyczna regresja liniowa.

## Technologie
Projekt został wykonany w Pythonie z użyciem bibliotek:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `category_encoders`
- `kagglehub`

## Uruchomienie
1. Zainstaluj wymagane biblioteki.
2. Otwórz notebook `PRiAD_projekt(predykcja aut).ipynb` w Jupyter Notebook lub JupyterLab.
3. Uruchom komórki po kolei.

Przykładowa instalacja zależności:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn category_encoders kagglehub
```

## Cel projektu
Celem projektu było sprawdzenie, które cechy samochodu najsilniej wpływają na jego cenę oraz zbudowanie modelu, który potrafi możliwie trafnie oszacować wartość używanego auta na podstawie dostępnych danych.

---
Autorzy: **Daniel Kaźmierczak, Jakub Sak**
