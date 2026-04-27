# 📓 Notion Template — Maturita 2026

Tento dokument popisuje **strukturu Notion workspace**, který má být tvůj **denní plánovač**.
GitHub repo = sklad obsahu. Notion = řízení.

---

## 🚀 Setup za 15 minut

### Krok 1 — Vytvoř workspace

1. Notion → New page → název **„Maturita 16.5.2026"**
2. Ikona: 🎓, cover dle libosti.

### Krok 2 — Vytvoř 4 databáze (níže návod)

---

## 📅 Database 1: „Plán 19 dnů"

**Typ:** Database — Calendar (default view)
**Properties:**

| Pole | Typ | Hodnoty |
|------|-----|---------|
| Den | Title | „Den 1", „Den 2"… „Den 19" |
| Datum | Date | 27. 4. 2026 → 15. 5. 2026 |
| Téma A | Relation → Témata 1-20 | T1 |
| Téma B | Relation → Témata 1-20 | T2 |
| Status | Select | ⬜ Nezačato / 🟡 Probíhá / ✅ Hotovo |
| Fáze | Select | 🟢 Stavba / 🟡 Simulace / 🔴 Finále |
| Čas studia | Number (h) | např. 4 |
| Reflexe | Text | „co jsem se naučil, co bylo těžké" |

**Views:**
- 📅 Calendar (Datum)
- ✅ Today (filter: Datum = Today)
- 📋 Table (sort: Datum asc)

**Naplň 19 řádků** podle `PLAN_MATURITA_16_5.md`:

```
Den 1  · Po 27.4. · T1 + T2  · 🟢 Stavba
Den 2  · Út 28.4. · T3 + T4  · 🟢 Stavba
Den 3  · St 29.4. · T5 + T6  · 🟢 Stavba
Den 4  · Čt 30.4. · T7 + T8  · 🟢 Stavba
Den 5  · Pá 1.5.  · T9 + T10 · 🟢 Stavba
Den 6  · So 2.5.  · T11+T12  · 🟢 Stavba
Den 7  · Ne 3.5.  · T13+T14  · 🟢 Stavba
Den 8  · Po 4.5.  · T15+T16  · 🟢 Stavba
Den 9  · Út 5.5.  · T17+T18  · 🟢 Stavba
Den 10 · St 6.5.  · T19+T20  · 🟢 Stavba
Den 11 · Čt 7.5.  · BUFFER   · 🟢 Stavba
Den 12 · Pá 8.5.  · Sim T1-5 · 🟡 Simulace
Den 13 · So 9.5.  · Sim T6-10· 🟡 Simulace
Den 14 · Ne 10.5. · Sim T11-15·🟡 Simulace
Den 15 · Po 11.5. · Sim T16-20·🟡 Simulace
Den 16 · Út 12.5. · Slabá místa·🟡 Simulace
Den 17 · St 13.5. · Cheat sheet·🔴 Finále
Den 18 · Čt 14.5. · Generálka · 🔴 Finále
Den 19 · Pá 15.5. · KLID     · 🔴 Finále
ZK     · So 16.5. · 🎯 ZKOUŠKA
```

---

## 📚 Database 2: „Témata 1-20"

**Typ:** Database — Gallery view (default)
**Properties:**

| Pole | Typ | Hodnoty |
|------|-----|---------|
| # | Title | „T1 Rozvaha + SWOT + DPH"… |
| Účto | Text | rozvaha |
| Mng/Mktg | Text | SWOT analýza |
| Eko | Text | DPH |
| Status | Select | 🔴 Nezačato / 🟡 Rozpracováno / 🟢 Hotovo / ⭐ Procvičit |
| Skóre v simulaci | Number (z 75) | např. 58 |
| Slabá místa | Text | „výpočet vlastní daň. povinnosti" |
| Github link | URL | odkaz na `temata/TEMA_X.md` |
| Notebook LM link | URL | tvůj NotebookLM URL |

**Views:**
- 🖼️ Gallery (group by Status)
- 📋 Table (sort: # asc)
- ⭐ Slabá místa (filter: Status = ⭐ Procvičit)

**Naplň 20 řádků** podle tabulky v `README.md`.

---

## 🃏 Database 3: „Flashcards"

**Typ:** Database — Gallery
**Properties:**

| Pole | Typ |
|------|-----|
| Q (otázka) | Title |
| A (odpověď) | Text |
| Téma | Relation → Témata 1-20 |
| Obtížnost | Select (🟢/🟡/🔴) |
| Tag | Multi-select (definice/vzorec/proces/datum) |
| Datum dalšího opakování | Date |
| Počet správných | Number |
| Počet chybných | Number |

**Views:**
- 🎯 Dnes opakovat (filter: Datum opakování ≤ Today)
- 🔴 Těžké (filter: Obtížnost = 🔴)
- 📋 Per téma (group by Téma)

**Workflow:**
1. Vyber kartu → klikni → otevři stránku.
2. Mentálně odpověz, pak rozbal toggle „Odpověď".
3. Zaktualizuj Datum opakování:
   - Správně poprvé → +1 den
   - Správně podruhé → +3 dny
   - Správně potřetí → +7 dní → +14 → +30
   - Špatně → reset na zítra

> 🚀 **Tip:** Pokud chceš silnější algoritmus, místo Notionu použij **Anki** s csv exportem.

---

## ✅ Database 4: „Samotesty"

**Typ:** Database — Table
**Properties:**

| Pole | Typ |
|------|-----|
| Datum | Title (např. „2026-05-08 T1") |
| Téma | Relation → Témata 1-20 |
| Skóre | Number (z 75) |
| % | Formula: `Skóre / 75 * 100` |
| Hodnocení | Formula: `if(% < 33, "❌ Propadl", if(% < 68, "🟡 Dobrý", if(% < 85, "✅ Chvalitebný", "⭐ Výborný")))` |
| Slabá místa | Text |
| Plán nápravy | Text |

**Views:**
- 📊 Per téma (group by Téma, sort: Datum desc)
- 📈 Progres (chart? Notion má bar charts)

---

## 📌 Hlavní stránka — „Maturita Hub"

Vytvoř hlavní stránku se 4 sloupci:

```
┌─────────────────────┬─────────────────────┐
│ 🎯 DNES             │ ⏰ ODPOČET          │
│ • Den 1 / 19        │ Zbývá: 19 dní       │
│ • Téma A: T1        │ Datum: 16. 5. 2026 │
│ • Téma B: T2        │                     │
│ • Status: 🟡 Probíhá│                     │
├─────────────────────┼─────────────────────┤
│ 📊 PROGRES          │ 📋 CHEAT SHEET      │
│ Hotovo: 0/20 témat  │ • DPH 21/12/0       │
│ Avg simulace: -/75  │ • SP 6,5%           │
│ Slabá místa: -      │ • ZP 4,5%           │
└─────────────────────┴─────────────────────┘

[Plán 19 dnů — Calendar view embedded]
[Témata 1-20 — Gallery embedded]
```

**Embed databáze:** v hlavní stránce napiš `/linked database` → vyber.

---

## 🔄 Sync s GitHubem

Notion **neumí** auto-sync s GitHubem markdownu. Workflow:

**Generování obsahu (Claude → GitHub):**
1. V Claude pusť Prompt 1-4
2. Ulož výstup do `temata/TEMA_X.md`
3. `git push` do `ufi-daman/maturita-2026`

**Konzumace v Notion:**
1. V Notion stránce „Téma 1" napiš `/embed`
2. Vlož raw GitHub URL: `https://raw.githubusercontent.com/ufi-daman/maturita-2026/main/temata/TEMA_01.md`
3. Notion zobrazí markdown
4. Alternativně: `/import` → Markdown → upload (kopie, ne live sync)

**Lepší alternativa** — používej GitHub mobilní app pro náhled, Notion jen pro plánování (nemíchej obsah).

---

## 📱 Mobilní setup

1. Stáhni **Notion app** (iOS/Android)
2. Stáhni **GitHub Mobile**
3. Přidej Notion „Maturita Hub" mezi Favorites
4. Widget na home screen: Notion „Today" view → vidíš dnešní téma na uzamčené obrazovce

---

## 🚀 Rychlejší alternativa — Notion AI šablona

Místo ručního setupu (15 min) můžeš:
1. V Notion → Templates → search „Study planner"
2. Najdi vhodný + duplikuj
3. Customizuj podle tabulky výše

Ale ručně je to robustnější, protože víš, kde co je.

---

📅 *Setup ideálně dnes večer — pak už jen plníš obsahem.*
