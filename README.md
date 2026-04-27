# 🎓 Maturita 2026 — Praktická zkouška Podnikání (16. 5. 2026)

> Repozitář s podklady, prompty a výstupy pro přípravu na praktickou maturitu.
> Termín: **sobota 16. 5. 2026**, nástup 7:00, 180 min zpracování + 20 min prezentace.
> Hodnocení: 25 b. Účto + 25 b. Mng/Mktg + 25 b. Eko + 25 b. prezentace = **100 b.** (≥ 33 % prošel)

---

## 🗺️ Struktura repa

```
maturita-2026/
├── 📅 PLAN_MATURITA_16_5.md   ← 19denní plán (master dokument)
├── 📋 prompts/                 ← 4 univerzální prompty na jakýkoliv text
│   ├── 01_shrnuti.md             „Strukturované shrnutí + mapa pojmů"
│   ├── 02_flashcards.md          „Flashcards pro active recall"
│   ├── 03_samotest.md            „Bloomův 4-úrovňový test"
│   └── 04_feynman.md             „Feynmanova technika"
├── 📚 temata/                  ← TEMA_01..TEMA_20.md (4 sekce + Q&A + slabá místa)
├── 📝 shrnuti/                 ← výstupy z Promptu 1
├── 🃏 flashcards/              ← výstupy z Promptu 2
├── ✅ samotesty/               ← výstupy z Promptu 3
├── 🧠 feynman/                 ← výstupy z Promptu 4
├── 📋 cheat-sheets/            ← rychlé reference (sazby, vzorce)
└── 📂 zdroje/                  ← původní PDF semináře (učitelovo)
```

---

## 🚀 Quick start (každý den)

1. **Otevři `PLAN_MATURITA_16_5.md`** → najdi dnešní téma A + B
2. **Otevři Notion** (databáze „Plán 19 dnů") → odškrtni úkol
3. **Pro každé téma:**
   - Přečti seminář v `zdroje/EKO seminář - Téma X.pdf` + `MKTG MGM seminář - Téma X.pdf`
   - Pusť `prompts/01_shrnuti.md` → ulož do `shrnuti/SHRNUTI_TEMA_X.md`
   - Pusť `prompts/02_flashcards.md` → ulož do `flashcards/FLASH_TEMA_X.md`
   - Vyřeš 1 účetní příklad ručně
4. **Večer:** rychlý quiz nad dnešními kartami (5 min)
5. **Push do GitHubu:** `git add . && git commit -m "Den X: T1+T2" && git push`

---

## 📊 3 fáze přípravy

### 🟢 Fáze 1 (dni 1–11, 27. 4. – 7. 5.) — Stavební bloky
2 témata denně → vznikne 20× `temata/TEMA_XX.md` se 4 sekcemi a Q&A.

### 🟡 Fáze 2 (dni 12–16, 8. – 12. 5.) — Simulace
Bez nahlížení do podkladů: 60 min na téma, srovnání s `TEMA_XX.md`, body z 75.

### 🔴 Fáze 3 (dni 17–19, 13. – 15. 5.) — Finalizace
Cheat sheet ručně, generálka 20min prezentace, pak SPÁT.

→ Detail v `PLAN_MATURITA_16_5.md`.

---

## 🛠️ Pracovní nástroje

| K čemu | Nástroj | Odkaz |
|--------|---------|-------|
| **Plánování + denní úkoly** | Notion | viz `NOTION_TEMPLATE.md` |
| **Generování obsahu** | Claude / ChatGPT | `prompts/` |
| **Drill flashcards na mobilu** | Anki | https://apps.ankiweb.net |
| **Audio při dojíždění** | NotebookLM | upload `TEMA_X.md` → audio overview |
| **Verzování + sklad** | GitHub | tento repo |

---

## 🔥 Klíčové sazby — pamatuj naslepo

```
DPH:     21 % / 12 % / 0 %    ⚠️ NE 15 %
SP zam:  6,5 %                ⚠️ NE 7,1 %
ZP zam:  4,5 %
Daň FO:  15 %
Sleva:   30 840 / rok = 2 570 / měsíc
Hyper:   nad 150 %            ⚠️ ve vašich testech
ČNB:     diskontní je základ
```

→ Detail v `cheat-sheets/CHEAT_SHEET.md`.

---

## 📚 20 témat × 3 části

| # | Účetnictví | Marketing/Mng | Ekonomika |
|---|------------|---------------|-----------|
| 1 | rozvaha, výsledovka | SWOT analýza | DPH (nepřímé daně) |
| 2 | finanční účty | dotazníkové šetření | odpisy DLM |
| 3 | ceniny | mkt mix - propagace | zásobovací činnost |
| 4 | zásoby materiálu | personální plánování | hospodaření podniku |
| 5 | zásoby zboží | hodnocení zaměstnanců | nezaměstnanost |
| 6 | převod/vyskladnění | optimalizace mzd. nákladů | monetární politika |
| 7 | prodej zboží/materiálu | získávání zaměstnanců | fiskální politika |
| 8 | spotřeba mat./cenin | motivační dopis + CV | sociální politika |
| 9 | pořízení DHM | krizová komunikace | HDP |
| 10 | odpisy DM | manažerské dovednosti | bod zvratu |
| 11 | pohledávky a závazky | hodnotící metody (Mng) | mzdy a výpočet |
| 12 | náklady a výnosy | mkt mix - cena | podnikatelský plán |
| 13 | služební cesta | obsazení volné pozice | daň z příjmu FO |
| 14 | faktury přijaté | mkt mix - výrobek | náklady podniku |
| 15 | faktury vydané | odměňování zam. | zdravotní pojištění |
| 16 | DPH na vstupu | pracovní smlouva | sociální pojištění |
| 17 | DPH na výstupu | produktivita práce | bankovní soustava |
| 18 | odvody daně ze mzdy | personální pohovor | plánování počtu zam. |
| 19 | zúčtování s institucemi | rozhodovací metody | plánování pers. nákladů |
| 20 | zúčtování hrubých mezd | vize, plánování, cíle | inflace |

---

## ✅ Progres trackující

Tento repo má napojený **Notion workspace** (viz `NOTION_TEMPLATE.md`) — tam veď progres. GitHub = sklad obsahu, Notion = plánovač.

---

📅 **Termín:** sobota 16. 5. 2026, 7:00
🎯 **Cíl:** ≥ 68 % = chvalitebný · ≥ 85 % = výborný

*Repo created 27. 4. 2026 · Maintained by [@ufi-daman](https://github.com/ufi-daman)*
