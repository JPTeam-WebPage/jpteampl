# CLAUDE.md — jpteam.pl

## Repo i deploy

- Repo: `github.com/JPTeam-WebPage/jpteampl`
- Branch `main` → produkcja (jpteam.pl) via Vercel auto-deploy
- Branch `draft` → Vercel preview URL (prototypy, nie idzie na prod)
- **Zawsze pracuj na `draft` jeśli nie powiedziano inaczej**

## Struktura plików

```
index.html                  ← strona główna
poradniki.html              ← lista wszystkich poradników
poradniki/[slug]/index.html ← każdy poradnik to osobny folder z index.html
polityka-prywatnosci.html
favicon.ico
logo-navbar.png
*.webp / *.jpg              ← obrazy (cannes, nice, provence)
```

## Design system

- Brand color: `#FF622E` (--orange)
- Fonts: `Montserrat` (headings), `Inter` (body) — ładowane z Google Fonts
- Język: polski, forma grzecznościowa „Państwo" (nigdy ty/Ty)
- Mobile-first, responsive

## Nowy poradnik — kroki

1. Utwórz folder: `poradniki/[slug-po-polsku]/`
2. Skopiuj strukturę z istniejącego poradnika jako bazę HTML
3. Wypełnij treść zgodnie z content-agent skill (`99 Systems/Skills/content-agent/SKILL.md`)
4. Dodaj wpis do `poradniki.html` (lista artykułów)
5. `git add` → `git commit` → `git push origin draft`
6. Vercel preview URL pojawi się automatycznie (~1-2 min)

## Zmiana UI — kroki

1. Edytuj odpowiedni plik HTML/CSS
2. `git push origin draft` → sprawdź na Vercel preview
3. Gdy OK → `git merge draft main` + `git push origin main`

## Kontekst biznesowy

JP Team = polskojęzyczny buyer's agent, Lazurowe Wybrzeże (Cannes, Nicea, Antibes).
Segment: 300k–1M+ EUR. Pełny kontekst: `../../../99 Systems/Context/CONTEXT_01_firma_i_misja.md`
Skill content: `../../../99 Systems/Skills/content-agent/SKILL.md`
