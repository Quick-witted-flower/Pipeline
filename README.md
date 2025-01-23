#Model Pipeline dla klasyfikacji - Diabetes Dataset


##Wprowadzenie

Celem tego projektu jest zastosowanie klasyfikacji do przewidywania, czy pacjent ma cukrzycę na podstawie danych medycznych. Używamy popularnego zbioru danych o cukrzycy, który zawiera takie cechy jak: wiek, liczba ciąż, BMI, pedigré cukrzycy itp. Projekt obejmuje eksplorację danych, przygotowanie danych do modelowania oraz zastosowanie procesu pipeline do trenowania modelu klasyfikacyjnego, porównując go z modelami tworzonymi w innych modułach.

Zadanie obejmuje następujące kroki:

    Eksploracja zbioru danych.
    Przygotowanie danych do modelowania.
    Stworzenie Pipeline dla przetwarzania danych i nauki modelu.

##Funkcjonalności

Projekt realizuje następujące etapy:
1. Eksploracja danych:

    Podsumowanie statystyczne cech (średnia, odchylenie standardowe, itp.).
    Analiza korelacji między cechami.
    Wizualizacja rozkładów cech dla pacjentów z cukrzycą i bez cukrzycy.

2. Przygotowanie danych:

    Obsługa brakujących wartości (wypełnienie medianą).
    Standaryzacja cech numerycznych.
    Podział danych na zestawy treningowe i testowe (80/20).

3. Stworzenie Pipeline:

    Pipeline łączy proces przetwarzania danych oraz trenowania modelu w jeden obiekt.
    W pipeline zawarto:
        Imputację brakujących wartości.
        Standaryzację cech numerycznych.
        Model regresji logistycznej do klasyfikacji.

4. Uczenie modelu:

    Model regresji logistycznej jest uczony na przetworzonych danych.

5. Ewaluacja modelu:

    Obliczenie metryk dla modelu:
        Dokładność (accuracy).
        Precision, Recall, F1-Score.
        AUC (Area Under the Curve).
        Macierz pomyłek.
        Krzywa ROC.

##Technologie

Projekt został stworzony z użyciem:

    Python: Język programowania użyty do analizy danych i uczenia modeli.
    Scikit-learn: Biblioteka do uczenia maszynowego i budowania pipeline.
    Pandas: Biblioteka do manipulacji i analizy danych.
    Matplotlib/Seaborn: Biblioteki do wizualizacji danych.

Pliki projektu:

    diabetes.csv: Zbiór danych zawierający informacje o pacjentach.
    main.py: Główny skrypt, który realizuje cały proces eksploracji, przygotowania 