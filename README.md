# CliniThink Community — Waitlist Landing Page

Strona listy oczekujących dla **CliniThink Community** — profesjonalnej społeczności dla psychoterapeutów CBT, ACT i Terapii Schematu.

## Wdrożenie

### GitHub Pages (najprostsze)
1. Utwórz nowe repozytorium (np. `clinithink-waitlist`)
2. Wgraj `index.html` do głównego katalogu
3. Settings → Pages → Branch: `main` → Folder: `/ (root)` → Save
4. Strona dostępna pod: `https://TWOJA-NAZWA.github.io/clinithink-waitlist/`

### Własna domena (Zenbox / inny hosting)
1. Wgraj `index.html` do katalogu `public_html` przez FTP lub panel hostingu
2. W panelu DNS dodaj rekord A lub CNAME wskazujący na serwer

### Domena + GitHub Pages
W repozytorium utwórz plik `CNAME` z treścią:
```
clinithink.pl
```
W panelu DNS (Zenbox) dodaj:
```
CNAME  www  → TWOJA-NAZWA.github.io
A      @    → 185.199.108.153
A      @    → 185.199.109.153
A      @    → 185.199.110.153
A      @    → 185.199.111.153
```

## Integracje (już skonfigurowane w pliku)

| Serwis | Status | Co robi |
|--------|--------|---------|
| **GetResponse** | ✅ aktywny | Dodaje kontakt do listy mailingowej |
| **Formspree** | ✅ aktywny | Zapisuje odpowiedzi ankiety (cena, rola, wyzwania) |

### Aktywacja analityki (opcjonalne)
W pliku `index.html` odszukaj komentarze `<!-- FB Pixel` i `<!-- GA4` i odkomentuj bloki wklejając swoje ID.

## Pola Formspree (widoczne w panelu formspree.io)

| Pole | Zawartość |
|------|-----------|
| `Imie_i_nazwisko` | Imię i nazwisko |
| `Email` | Adres e-mail |
| `Rola` | Rola zawodowa |
| `Wyzwania` | Wybrane wyzwania (multi-select) |
| `Doswiadczenie` | Lata doświadczenia |
| `Cena_zbyt_niska` | Van Westendorp — zbyt niska |
| `Cena_zaporowa` | Van Westendorp — zbyt wysoka |
| `Cena_adekwatna` | Van Westendorp — adekwatna |

## Struktura strony

```
index.html          ← cały projekt w jednym pliku (self-contained)
README.md           ← ten plik
CNAME               ← opcjonalnie dla własnej domeny
```

## Autor

Adam Elżanowski — Superwizor-Dydaktyk CBT, współzałożyciel Szkoły Psychoterapii HarmonJa
