# Hjem drinks

Drinksopskrifter til cocktailkortet i Hjem, mit eget Home Assistant-dashboard. 375 drinks på dansk, alle med billede. 109 billeder er fra folderne (Råstoff, CUBA, Pure Shots, BARMIX, Harlegin, Små Shots), og resten er tegnet til Hjem.

Hjem henter listen herfra og viser den som standardmenu. "Hvad kan jeg lave?" i appen søger i den ud fra det, du har i skabet.

## Kategorier

| Kategori | Drinks |
|---|---|
| Vodka | 53 |
| Gin | 51 |
| Likør | 45 |
| Rom | 44 |
| Kaffe & dessert | 34 |
| Spritz | 30 |
| Alkoholfri | 29 |
| Små Shots | 28 |
| Whisky | 26 |
| Tequila | 23 |
| Cognac & brandy | 12 |

## Format

`drinks.json` er en liste. Hver drink ser sådan ud:

```json
{
  "n": "Negroni",
  "c": "Gin",
  "d": "Bitter, sød og stærk på én gang",
  "i": ["3 cl gin", "3 cl Campari", "3 cl sød vermouth", "Appelsinskive", "Isterninger"],
  "m": "Rør det hele med is i et røreglas og si over i et glas med en stor isterning."
}
```

| Felt | Indhold | Højst |
|---|---|---|
| `n` | Navn | 40 tegn |
| `c` | Kategori | 20 tegn |
| `d` | Kort beskrivelse | 120 tegn |
| `i` | Ingredienser, én pr. linje, med mængde i cl | 14 linjer á 60 tegn |
| `m` | Sådan gør du | 400 tegn |
| `g` | Billede (valgfrit), sti i repoet, fx `billeder/negroni.jpg` | 70 kB |

Skriv ingredienserne med almindelige navne (`gin`, `hvid rom`, `limesaft`, `sukkersirup`), så "Hvad kan jeg lave?" i Hjem kan genkende flaskerne. Pynt som `Appelsinskive` og alt, der starter med `Evt.`, tæller ikke med.

## Tilføj en drink

Ret `drinks.json` og lav en pull request. Tjek, at filen stadig er gyldig JSON.

## Billeder

Billederne ligger i `billeder/`. Læg en ny som JPG (højst ca. 360 px og 70 kB), og skriv stien i `g`.
