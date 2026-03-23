# JP Team — strona internetowa

Statyczna strona HTML gotowa do wdrożenia na Vercel.

## Struktura plików

```
jpteam-website/
├── index.html        ← strona główna (jpteam.pl)
├── poradniki.html    ← podstrona /poradniki
├── realizacje.html   ← podstrona /realizacje
├── vercel.json       ← konfiguracja routingu (czyste URL-e bez .html)
└── README.md
```

## Jak wdrożyć na Vercel

### Krok 1 — GitHub
1. Wejdź na [github.com](https://github.com) i utwórz konto (lub zaloguj się)
2. Kliknij **New repository** → nazwa: `jpteam-website` → Public → **Create**
3. Wgraj pliki: kliknij **uploading an existing file**, zaznacz wszystkie pliki z tego folderu, kliknij **Commit changes**

### Krok 2 — Vercel
1. Wejdź na [vercel.com](https://vercel.com) i zaloguj się przez GitHub
2. Kliknij **Add New → Project**
3. Wybierz repozytorium `jpteam-website` → kliknij **Import**
4. Framework Preset: **Other** (statyczna strona, bez frameworka)
5. Kliknij **Deploy** — Vercel sam wykryje pliki HTML

### Krok 3 — Własna domena
1. W ustawieniach projektu na Vercel → **Domains** → dodaj `jpteam.pl`
2. Vercel pokaże rekordy DNS do ustawienia u rejestratora domeny
3. Po propagacji DNS (do 24h) strona będzie dostępna pod jpteam.pl

## Aktualizacja strony

Po każdej zmianie plików — wgraj zaktualizowany plik na GitHub (ten sam repozytorium).
Vercel automatycznie wykryje zmianę i przebuduje stronę w ciągu ~30 sekund.
