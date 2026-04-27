# Prompt 2 — Flashcards pro active recall

**Použití:** druhý den po shrnutí. Opakuj 3–5 dní.
**Vstup:** školní text NEBO výstup z Promptu 1.
**Výstup:** 15–30 atomických flashcards.

---

## 📋 PROMPT (kopíruj celé)

```
Jsi expert na spaced repetition a techniku aktivního vybavování (active recall).
Z přiloženého textu vytvoř sadu flashcards v češtině podle těchto pravidel:

PRAVIDLA:
- Jedna karta = jedna myšlenka (atomic). Nikdy nespojuj 2 fakta do jedné karty.
- Otázka musí nutit k aktivnímu vybavení, ne jen k rozpoznání.
- Vyhýbej se „ano/ne" otázkám — použij „Co je...", „Proč...", „Jak...", „Kdy...", „Čím se liší...".
- U definicí vytvoř OBOUSTRANNOU kartu (pojem → definice A definice → pojem).
- U procesů/postupů vytvoř „cloze deletion" — věta s vynechaným klíčovým slovem [...].

FORMÁT (přesně):
---
Q: [otázka]
A: [odpověď, max 2 věty]
Obtížnost: 🟢 snadná / 🟡 střední / 🔴 těžká
Tag: [kategorie, např. „definice", „vzorec", „proces", „datum"]
---

Vytvoř 15–30 karet (dle rozsahu textu). Pokryj všechny 🔴 MUSÍŠ UMĚT pojmy.
Na konci přidej 3 „syntetizační" karty (propojují více pojmů dohromady).

VSTUP:
[SEM VLOŽ TEXT]
```

---

## 💡 Kde karty drilovat

| Nástroj | Pro/proti |
|---------|-----------|
| **Anki** (mobil + desktop) | ✅ spaced repetition algoritmus, ✅ free, ⚠️ import z markdownu vyžaduje konverzi |
| **NotebookLM** | ✅ generuje studio karty automaticky, ⚠️ ne tak chytrá rotace |
| **Notion DB** | ✅ filtry, ⚠️ ručně klikat „další" |
| **Tištěné karty** | ✅ svalová paměť při psaní, ❌ pomalé |

## 🔄 Konverze na Anki (CSV)

Pokud chceš import do Anki, požádej Claude:
> „Převeď flashcards na CSV formát: Q;A;tag (oddělovač středník)."

Pak v Anki: File → Import → vyber CSV → pole 1=Front, 2=Back.

## 🔗 Návaznost

→ Po 3 dnech opakování pusť **Prompt 3** (`03_samotest.md`) k ověření.
