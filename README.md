# Toníkova stavba

2D stavěcí hra pro Toníka (6 let). Jeden soubor `index.html`, žádné knihovny, žádná instalace.

## Spuštění
- Stačí otevřít `index.html` v prohlížeči (PC, tablet, telefon na šířku).
- Na tabletu: nahrát na hosting (např. GitHub Pages) a přidat na plochu.

## Ovládání
| | Dotyk | Klávesnice |
|---|---|---|
| Jízda | posuvný joystick vlevo dole | šipky ← → nebo A D |
| Pracovat | zelené ozubené kolo | mezerník / Enter / ↓ |
| Zatroubit | žlutá trubka | ↑ |
| Výběr stroje | ikony dole | 1–4 nebo Tab |

Hra nemá žádný text v zadání – cíl ukazují:
- čárkovaný „plánek“ stavby (duch toho, co se bude stavět),
- žlutá zóna na zemi s bublinou stroje, který tam patří,
- šipka na kraji obrazovky, když je zóna mimo záběr,
- poskakující ikona správného stroje v liště.

## Levely
Dům · Hřiště · Dálnice · Most · Aquapark · Obchodní dům · Letiště · Mrakodrap

Všechny jsou odemčené, dokončené mají zelenou fajfku (ukládá se v prohlížeči).

## Jak přidat / upravit level
Levely jsou jen data v poli `LEVELS` v `index.html` (sekce „LEVELY“):
- `parts` – díly stavby (obdélníky `R`, mnohoúhelníky `P`, kruhy `O`),
- `steps` – kroky: `work` (stroj stojí v zóně + tlačítko), `carry` (nabrat a složit), `drive` (projet úsek),
- `pits` / `mounds` – jámy a kopce, které stroje kopou / srovnávají.
