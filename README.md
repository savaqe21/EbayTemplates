# eBay Templates

Repozytorium zawiera gotowe szablony HTML do wklejania w opisy aukcji eBay.  
Strona przeglądowa dostępna przez **GitHub Pages** (`index.html`).

---

## Struktura projektu

```
EbayTemplates/
├── index.html                        ← Strona główna (GitHub Pages) z listą szablonów
├── src/
│   ├── logo.png                      ← Logo sklepu (używane w szablonach)
│   └── produkt.webp                  ← Zdjęcie produktu (zamień na własne)
├── Sellnet Szablon/
│   └── ebay-template.html            ← Szablon v1 — turkusowy, styl polski
└── Farys DE Premium/
    └── ebay-template.html            ← Szablon v2 — grafitowy + czerwony, rynek DE
```

---

## Dostępne szablony

| # | Szablon | Produkt | Design |
|---|---|---|---|
| 1 | `Sellnet Szablon/ebay-template.html` | Meble garażowe FR4113 — 3 999,00 zł | Turkusowy + czarny |
| 2 | `Farys DE Premium/ebay-template.html` | Meble garażowe FR4113 — 3 999,00 zł | Grafitowy + czerwony (rynek DE) |

---

## Jak edytować szablon

1. Otwórz `ebay-template.html` w edytorze tekstu (Notatnik, Notepad++, VSCode)
2. Na samej górze pliku jest blok **`JAK EDYTOWAĆ`** — opisuje wszystkie opcje
3. Każde pole do zmiany oznaczone jest w kodzie komentarzem **`✏️`**  
   Szybki sposób na przejście przez wszystkie pola: **CTRL+F → wpisz ✏️**
4. Zmień wartość: **CTRL+H** (Znajdź i Zamień) → stara wartość → nowa → Zamień wszystko
5. Skopiuj zawartość pliku i wklej w pole opisu aukcji eBay (tryb HTML)

### Przez AI (Claude / ChatGPT)

Wklej cały plik do chatu i napisz np.:  
*„Zmień cenę na 2 499 zł, tytuł na [nowy tytuł], numer itemu na 123456789"*  
AI znajdzie i zmieni wszystkie wystąpienia — skopiuj wynik z powrotem.

---

## Sklep eBay

[farys7shop na ebay.de](https://www.ebay.de/str/farys7shop)

---

## Tech stack

- Czysty HTML5 + CSS — zero JavaScript
- Zakładki CSS-only (`input[type=radio] :checked ~`) — zgodne z polityką eBay
- Wszystkie style osadzone w `<style>` — nie wymaga zewnętrznych plików CSS
- Responsywne (mobile-friendly), testowane na desktop i mobile
- Kod podzielony na zakresy (`#ft`, `#ft2`) — nie koliduje ze stylami strony eBay
