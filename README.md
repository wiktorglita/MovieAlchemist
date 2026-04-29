# MovieAlchemist - System Analizy i Predykcji Sukcesu Projektów Filmowych

## Opis projektu
Projekt stanowi zaawansowany system wspomagania decyzji, który wykorzystuje metody analizy danych oraz uczenie maszynowe do przewidywania potencjału komercyjnego projektów filmowych. Na podstawie wprowadzonych przez użytkownika parametrów - takich jak gatunek, słowa kluczowe, obsada aktorska czy reżyser - system analizuje zależności i szacuje procentową szansę na sukces danej produkcji.

Głównym celem systemu jest wsparcie twórców i producentów w procesie budowania koncepcji filmowych oraz optymalizacja decyzji biznesowych poprzez analizę historycznych danych kinematograficznych. 

## Źródło danych
Modele analityczne w tym projekcie zostały wytrenowane w oparciu o historyczne dane kinematograficzne pobrane z platformy Kaggle. https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

## Główne funkcjonalności
* **Predykcja sukcesu:** Ocena potencjału komercyjnego filmu na podstawie wybranych cech.
* **Analiza kombinacji:** Badanie wpływu połączeń różnych elementów (np. specyficzne gatunki w zestawieniu z konkretnymi reżyserami) na końcowy sukces.
* **System rekomendacyjny:** Wykorzystanie algorytmów uczenia maszynowego (m.in. wektoryzacja TF-IDF, regresja logistyczna) do analizy tekstowej i rekomendacji.
* **Przetwarzanie danych:** Zaawansowana obróbka i czyszczenie dużych zbiorów danych.

## Interfejs użytkownika
W ramach projektu zaprojektowano nowoczesny, interaktywny interfejs użytkownika, który umożliwia łatwe wprowadzanie danych i odczytywanie wyników predykcji. 

Prototyp aplikacji można obejrzeć pod poniższym adresem:
[Projekt interfejsu (Figma)](https://doll-debug-75782524.figma.site/)

## Zastosowane technologie
* **Język programowania:** Python
* **Biblioteki danych:** Pandas, NumPy
* **Uczenie maszynowe:** Scikit-learn
* **Środowisko:** Jupyter Notebook
* **Interfejs / Design:** Figma

## Struktura plików w repozytorium
* `MovieAlchemist.ipynb` - Główny notatnik zawierający ostateczny model predykcyjny oraz skrypty pozwalające na wprowadzanie i testowanie własnych pomysłów filmowych.
* `System_rekomendacji.ipynb` / `System_rekomendacjiCD.ipynb` - Notatniki analityczne odpowiedzialne za eksplorację danych (EDA), czyszczenie zbiorów, inżynierię cech oraz trenowanie modeli rekomendacyjnych.
* `tmdb_5000_movies.csv` i `tmdb_5000_credits.csv` - Surowe zbiory danych wejściowych (dane historyczne o filmach i obsadzie).
* `system_rekomendacji_final_clean.csv` - Przetworzony, wyczyszczony i gotowy do analizy zbiór danych zasilający model uczenia maszynowego.
* `Dokumentacja_projektu.docx` - Szczegółowa dokumentacja techniczna obejmująca architekturę systemu, wymagania oraz scenariusze użycia.

## Instrukcja uruchomienia
1. Sklonuj niniejsze repozytorium na swój dysk lokalny.
2. Upewnij się, że posiadasz zainstalowane środowisko Python (wersja 3.8+) oraz program Jupyter Notebook.
3. Zainstaluj wymagane zależności projektowe, wykonując w terminalu polecenie:
   ```bash
   pip install pandas numpy scikit-learn
4. Uruchom środowisko Jupyter
   ```bash
   jupyter notebook
5. Otwórz plik MovieAlchemist.ipynb i postępuj zgodnie z instrukcjami w komórkach, aby przetestować działanie modelu na własnych koncepcjach filmowych.
