# Style-guide – Fitness štúdio Pulz

## Zadanie
Podľa `text.txt` vytvor vlastné `index.html` a `assets/css/style.css`.
Obrázky (ikony) nájdeš v priečinku `assets/images/`.

Musíš použiť:
- [ ] sémantické HTML (`header`, `nav`, `main`, `section`, `article`, `footer`)
- [ ] CSS premenné v `:root` (farby z tabuľky nižšie)
- [ ] Google Fonts cez `@import` (nadpisy: Bebas Neue, text: Barlow)
- [ ] relatívne jednotky (`rem`, `%`, `fr`, `vw`) a `clamp()` pre veľkosť nadpisov
- [ ] **flexbox** (aspoň hlavička a navigácia)
- [ ] **grid** (aspoň karty a pätička)
- [ ] mobile first: základné štýly sú pre mobil, ďalej len `@media (min-width: ...)`
- [ ] BEM názvy tried (napr. `hlavicka__logo`)
- [ ] `:hover` na odkazoch a tlačidlách
- [ ] žiadny JavaScript

## Farby
| Premenná | Hodnota | Použitie |
|---|---|---|
| `--noc` | `hsl(230, 35%, 9%)` | pozadie stránky |
| `--karta` | `hsl(230, 30%, 15%)` | pozadie kariet a pätičky |
| `--limetka` | `oklch(88% 0.2 125)` | hlavný akcent |
| `--ruzova` | `oklch(65% 0.24 10)` | druhý akcent – hover |
| `--text` | `hsl(0, 0%, 94%)` | farba textu |
| `--tlmeny` | `hsla(0, 0%, 100%, 0.65)` | tlmený text |

## Fonty
```css
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Barlow:wght@300..700&display=swap');
```
- Nadpisy a logo: **Bebas Neue**
- Text: **Barlow**
- Základná veľkosť textu: `1.1rem`, riadkovanie `1.7`

## Breakpointy
| Zariadenie | Šírka | Karty |
|---|---|---|
| Mobil | do 639px (základ) | 1 stĺpec |
| Tablet | od 640px | 2 stĺpce |
| Desktop | od 1024px | viď layout nižšie |

Desktop layout karty: 4 stĺpce.

## Odsadenia
- Bočné odsadenie sekcií: `5%` (na desktope môže byť viac)
- Vertikálne odsadenie sekcií: `3rem`
- Medzery medzi prvkami: `1rem` až `2rem`
