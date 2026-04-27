# Prompt 3 — Kontrolní samotest (Bloomova taxonomie)

**Použití:** týden před zkouškou nebo po 3 dnech driloningu flashcards.
**Vstup:** školní text NEBO `TEMA_XX.md`.
**Výstup:** 4-úrovňový test 10 otázek + skryté vzorové odpovědi.

---

## 📋 PROMPT (kopíruj celé)

```
Jsi přísný zkoušející. Z přiloženého textu vytvoř test, který ověří, jestli
látku opravdu chápu (ne jen pamatuji nazpaměť).

Sestav test ve 4 úrovních (Bloomova taxonomie):

## ÚROVEŇ 1 — Znalost (3 otázky)
Faktické otázky. „Co je...", „Kdy se stalo...", „Jak se jmenuje..."

## ÚROVEŇ 2 — Porozumění (3 otázky)
„Vysvětli vlastními slovy...", „Uveď příklad...", „Co by se stalo kdyby..."

## ÚROVEŇ 3 — Aplikace (2 otázky)
Modelový problém/úloha, kde musím znalost POUŽÍT na něčem novém.

## ÚROVEŇ 4 — Analýza a hodnocení (2 otázky)
„Porovnej X a Y...", „Který přístup je lepší pro situaci Z a proč...",
„Najdi chybu v tomto tvrzení..."

PRAVIDLA:
- U každé otázky uveď očekávaný rozsah odpovědi (1 věta / odstavec / výpočet).
- NEPIŠ odpovědi hned. Zobraz je až poté, co napíšu „odpovědi prosím".
- Pak ukaž vzorové odpovědi + červeně označ, kde bych typicky ztratil body.

VSTUP:
[SEM VLOŽ TEXT]
```

---

## 📊 Bodování (vlastní pro maturitní simulaci)

Z 10 otázek si počítej body takto, ať odpovídá zkoušce (75 b. praktická část):

| Úroveň | Otázek | Body za otázku | Max |
|--------|--------|----------------|-----|
| 1. Znalost | 3 | 5 | 15 |
| 2. Porozumění | 3 | 7 | 21 |
| 3. Aplikace | 2 | 12 | 24 |
| 4. Analýza | 2 | 7,5 | 15 |
| **Celkem** | **10** | — | **75** |

**Hranice:** ≥ 25 b. (33 %) prošel · ≥ 51 b. (68 %) chvalitebný · ≥ 64 b. (85 %) výborný.

## 🔁 Když propadneš

- **Pod 33 %** → vrať se k Promptu 1 (shrnutí). Něco jsi nepochopil.
- **33–67 %** → drilling Prompt 2 (flashcards) na slabá místa.
- **Nad 68 %** → pusť **Prompt 4** (Feynman) na 1 nejtěžší pojem.

## 💾 Ukládej výstupy

Test + tvá odpověď + vzor → `samotesty/TEST_TEMA_XX_DATUM.md`. Po týdnu vidíš pokrok.
