<p>
  <h1>📊 Projekty Analizy Danych i Uczenia Maszynowego</h1>
  <p>
    Zestawienie trzech projektów obejmujących eksplorację danych, modele predykcyjne oraz klasteryzację.
  </p>
</p>

---

## 📖 Spis treści

1. [Predykcja decyzji kredytowej](https://github.com/kslapinski/CV-projects/tree/main/1.%20Predykcja%20decyzji%20kredytowej)  
2. [Czynniki wpływające na wyniki egzaminów studentów](https://github.com/kslapinski/CV-projects/tree/main/2.%20Czynniki%20wpływające%20na%20wyniki%20egzaminu%20studentów)  
3. [Klasteryzacja poziomu otyłości](https://github.com/kslapinski/CV-projects/tree/main/3.%20Ocena%20poziomu%20otyłości%20na%20podstawie%20nawyków)

---

## 1. Predykcja decyzji kredytowej

### 📝 Streszczenie
Analiza **45 000** wniosków kredytowych (14 atrybutów) z celem przewidywania wartości `loan_status` (0/1).  
Projekt koncentruje się na automatyzacji decyzji kredytowych, redukcji ryzyka oraz usprawnieniu procesów finansowych.

### 🎯 Cele projektu
- **Eksploracja danych (EDA)**  
  - Sprawdzenie rozkładów cech (zmienne numeryczne i kategoryczne)  
  - Wykrywanie braków danych i wartości odstających  
- **Przygotowanie cech**  
  - Czyszczenie
  - Kodowanie zmiennych kategorycznych
  - Skalowanie cech numerycznych  
- **Budowa i porównanie modeli**  
  - **Logistic Regression**  
  - **Random Forest**  
  - **XGBoost**  
  - **SGDClassifier**  
  - **Model hybrydowy (Stacking)**  
- **Ewaluacja i walidacja**  
  - Metryki: accuracy, F1-score, AUC  
  - Analiza: confusion matrix, ROC curve, lift chart, gain chart  

### 🛠️ Metody i narzędzia
- `pandas`, `numpy`  
- `scikit-learn`  
- `xgboost`  
- `matplotlib`, `seaborn`  

---

## 2. Czynniki wpływające na wyniki egzaminów studentów

### 📝 Streszczenie
Zbiór danych zawierający **6607** rekordów i **20** atrybutów dotyczących nawyków nauki, frekwencji oraz wsparcia ze strony rodziców.  
Celem jest identyfikacja kluczowych czynników wpływających na wyniki egzaminów.

### 🎯 Cele projektu
1. **Eksploracja i wizualizacja danych**  
   - Analiza rozkładów cech ilościowych i kategorycznych  
   - Macierz korelacji zmiennych numerycznych  
2. **Modelowanie statystyczne**  
   - **Regresja logistyczna**  
   - **LASSO** w celu zbadania istotnych cech  
   - **ANOVA** (analiza wariancji) do porównania grup uczniów  
3. **Analiza asocjacyjna**  
   - Generowanie reguł apriori (wykrywanie zależności między atrybutami)  
4. **Modelowanie probabilistyczne**  
   - Budowa sieci bayesowskiej do wnioskowania
5. **Analiza korespondencji**  
   - Badanie relacji pomiędzy zmiennymi kategorycznymi 

### 🛠️ Metody i narzędzia
- `pandas`, `numpy`  
- `scikit-learn`, `statsmodels`  
- `mlxtend` (reguły asocjacyjne)  
- `pgmpy` (sieci bayesowskie), `networkx` (wizualizacja sieci)  
- `prince` (analiza korespondencji)  
- `altair`, `matplotlib`, `seaborn` (wizualizacje)  

---

## 3. Klasteryzacja poziomu otyłości

### 📝 Streszczenie
Ocena poziomu otyłości u **2111** osób z Meksyku, Peru i Kolumbii na podstawie nawyków żywieniowych i aktywności fizycznej.  
Dane w **77 % syntetyczne** (SMOTE), **23 %** z ankiet online. Klasa docelowa `NObesity` obejmuje siedem kategorii od niedowagi do otyłości III stopnia.

### 🎯 Cele projektu
- **Eksploracja i przygotowanie danych**  
  - Kodowanie zmiennych kategorycznych  
  - Skalowanie zmiennych numerycznych  
- **Klasteryzacja**  
  - **KMeans**  
  - **AgglomerativeClustering (Ward)**  
- **Optymalizacja liczby klastrów**  
  - Metoda łokcia  
  - Wskaźnik silhouette score  
- **Ewaluacja efektów klasteryzacji**  
  - `silhouette_score`  
  - `adjusted_rand_score`  
  - Profilowanie uzyskanych grup (np. średnia waga, wiek, aktywność fizyczna)  

### 🛠️ Metody i narzędzia
- `pandas`, `numpy`  
- `scikit-learn`  
- `matplotlib`, `seaborn`  
