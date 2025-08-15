# 🤖 ML Cheatsheets - Twój przewodnik po Machine Learning

Kolekcja praktycznych ściąg z Machine Learning dla kursantów Data Science! Znajdziesz tutaj **konkretne algorytmy, teorię i praktyczne zastosowania** przedstawione w przystępny sposób. Każda ściągawka zawiera wyjaśnienia, przykłady kodu i real-world use cases.

## 🚀 Jak używać (dla kursantów)

### Na GitHub Pages (ZALECANE)
1. **Otwórz stronę:** [link do GitHub Pages]
2. **Wybierz ściągę** z menu ML Cheatsheets
3. **Czytaj wyjaśnienia** i analizuj przykłady kodu
4. **Kopiuj snippety** i testuj je w swoim środowisku (Jupyter, Colab, VS Code)
5. **Eksperymentuj** z parametrami i danymi!

**✨ Każda ściągawka:** Teoria + Praktyka + Real-world przykłady

## 🛠️ Development (dla autorów)

### Lokalne uruchomienie
```bash
# Zainstaluj Quarto
brew install quarto

# Podgląd na żywo
quarto preview

# Renderowanie do docs/
quarto render
```

### Publikacja z aliasem
```bash
# Alias dla szybkiego render + push
alias qpush="quarto render && git add . && git commit -m 'Update cheatsheets' && git push"

# Użycie
qpush
```

### GitHub Pages setup
1. **Settings → Pages → Source:** `main` branch, `/docs` folder
2. Po pierwszym push strona będzie dostępna pod `https://username.github.io/repo-name`
3. Automatyczne aktualizacje przy każdym push!

## 📁 Struktura projektu
```
.
├── _quarto.yml           # Konfiguracja Quarto
├── docs/                 # Wyrenderowane pliki (GitHub Pages)
├── index.qmd             # Strona główna
├── cheatsheets/
│   ├── 01-intro-ml.qmd           # Wprowadzenie do ML
│   ├── 02-linear-regression.qmd  # Linear Regression w praktyce
│   └── 03-decision-trees.qmd     # Decision Trees i klasyfikacja
├── styles.css
└── requirements.txt      # Python dependencies dla przykładów
```

## ✏️ Dodawanie nowych ściąg ML

### 1. Utwórz nowy plik
```bash
cp cheatsheets/01-intro-ml.qmd cheatsheets/04-new-algorithm.qmd
```

### 2. Edytuj zawartość
- Zmień tytuł w YAML header
- Dodaj wyjaśnienie algorytmu (teoria + intuicja)
- Dodaj praktyczny przykład z kodem
- Opisz real-world use cases

### 3. Dodaj do nawigacji
W `_quarto.yml` dodaj nowy link:
```yaml
navbar:
  left:
    - text: "ML Cheatsheets"
      menu:
        - text: "Nowy Algorytm"
          href: cheatsheets/04-new-algorithm.qmd
```

### 4. Opublikuj
```bash
qpush  # alias render + commit + push
```

## 🧠 Co znajdziesz w ML Cheatsheets?

### 📚 **Algorytmy fundamentalne**
- Linear & Logistic Regression
- Decision Trees & Random Forest  
- K-Means & Hierarchical Clustering
- SVM & Neural Networks

### 🔬 **Teoria praktycznie**
- Kiedy użyć którego algorytmu?
- Jak interpretować wyniki?
- Typowe pułapki i jak ich unikać

### 🌍 **Real-world przypadki**
- Predykcja cen nieruchomości
- Segmentacja klientów
- Klasyfikacja obrazów
- Analiza sentymentu

## 🎯 Docelowa grupa

**Idealne dla:**
- Kursantów Data Science na początku drogi
- Osób chcących zrozumieć ML intuicyjnie
- Programistów przechodzących na Data Science
- Wszystkich, którzy chcą praktycznie poznać algorytmy ML

## 📈 Plan rozwoju

**Najbliższe ściągawki:**
- K-Means Clustering 
- Random Forest
- Logistic Regression
- Feature Engineering
- Model Evaluation & Metrics