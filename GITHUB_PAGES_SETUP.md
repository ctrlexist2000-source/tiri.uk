# Tiri's Blog - GitHub Pages Setup

Blog oparty na Hugo z 170 postami.

## 📋 Kroki wdrożenia na GitHub Pages

### Krok 1: Przygotowanie repozytorium GitHub

1. Stwórz nowe repozytorium na GitHub o nazwie `tiri.uk` lub `tiri-uk`
   - Możesz użyć nazwy `<username>.github.io` aby uniknąć przesyłu źródła na GitHub Pages

### Krok 2: Konfiguracja Git

```bash
cd c:\Users\AnnPi\OneDrive\Documents\GitHub\tiri.uk
git init
git add .
git commit -m "Initial commit: Hugo blog with 170 posts"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/tiri.uk.git
git push -u origin main
```

### Krok 3: Włącz GitHub Pages

1. Przejdź do Settings repozytorium na GitHub
2. Poszukaj sekcji "Pages" w lewym menu
3. Ustaw "Source" na `Deploy from a branch`
4. Wybierz branch `gh-pages` i folder `/ (root)`
5. Kliknij Save

### Krok 4: Poczekaj na build

GitHub Actions automatycznie:
- Zbuduje stronę Hugo
- Wdrożymy na branch `gh-pages`
- Strona będzie dostępna w ciągu 1-2 minut

### Krok 5: Połącz domenę www.tiri.uk

**W registrze domeny (np. Namecheap, GoDaddy):**

Jeśli używasz `tiri.uk.github.io`:
```
CNAME: tiri.uk -> tiri.uk.github.io
```

Jeśli używasz custom repozytorium:
```
A Records:
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**Na GitHub Pages settings:**
- Wpisz: `tiri.uk`
- Zaznacz "Enforce HTTPS"

### Krok 6: Weryfikacja

Po 5-15 minutach strona będzie dostępna pod:
- `https://tiri.uk`
- `https://www.tiri.uk`

## 📝 Dodawanie nowych postów

1. Dodaj nowy plik w `content/posts/YYYY-MM-DD-slug.md`
2. Commit i push: `git add . && git commit -m "New post" && git push`
3. GitHub Actions automatycznie zbuduje i wdroży stronę

## 🔧 Lokalne testowanie

```bash
hugo server
# Otwórz http://localhost:1313/
```

## 📁 Struktura projektu

```
tiri.uk/
├── .github/
│   └── workflows/
│       └── deploy.yml         # GitHub Actions automation
├── content/
│   ├── posts/                 # 170 postów blogowych
│   └── archives.md
├── themes/
│   └── PaperMod/             # Temat Hugo
├── hugo.toml                 # Konfiguracja
└── README.md
```

## ✅ Checklist

- [ ] Repozytorium GitHub stworzone
- [ ] Git skonfigurowany lokalnie
- [ ] Kod wrzucony na GitHub
- [ ] GitHub Actions uruchomiony pomyślnie
- [ ] GitHub Pages włączone (gh-pages branch)
- [ ] Domena skonfigurowana (DNS records)
- [ ] HTTPS działające
- [ ] Strona dostępna na www.tiri.uk
