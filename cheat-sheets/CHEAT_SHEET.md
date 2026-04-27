# 📋 CHEAT SHEET — sazby + vzorce (maturita 16. 5. 2026)

> **Tisknout 1× na A4. Před zkouškou opsat ručně 3× na čistý papír — svalová paměť.**
> ⚠️ POZOR: Hodnoty platí podle **vašich seminářů a testů**, ne nutně oficiálně k 2026.

---

## 🧾 DPH (daň z přidané hodnoty)

| Sazba | % | Příklady |
|-------|---|----------|
| **Základní** | **21 %** | většina zboží a služeb |
| **Snížená** | **12 %** | potraviny, voda, knihy, MHD, ubytování, stavby pro bydlení |
| **Nulová** | **0 %** | export do třetích zemí, knihy (od 2024) |

> ⚠️ **POZOR — ve vašich materiálech je 12 %, NE 15 %!** Nepoužívej zastaralou hodnotu.

### Algoritmus výpočtu

| Z čeho | Vzorec | Příklad (12 %) |
|--------|--------|----------------|
| Cena bez DPH → DPH | `základ × 0,12` | 1 000 × 0,12 = **120 Kč** |
| Cena bez DPH → s DPH | `základ × 1,12` | 1 000 × 1,12 = **1 120 Kč** |
| Cena s DPH → základ | `cena ÷ 1,12` | 1 120 ÷ 1,12 = **1 000 Kč** |
| Cena s DPH → DPH | `cena ÷ 1,12 × 0,12` | 1 120 ÷ 1,12 × 0,12 = **120 Kč** |

### Vlastní daňová povinnost

```
DPH na výstupu (z prodejů) − DPH na vstupu (z nákupů) = vlastní daňová povinnost
```

Pokud kladné → odvod státu. Pokud záporné → nadměrný odpočet (stát ti vrátí).

---

## 💰 ODVODY ZE MZDY

### Sociální pojištění (SP)

| Plátce | Sazba | Z čeho |
|--------|-------|--------|
| **Zaměstnanec** | **6,5 %** | hrubá mzda |
| Zaměstnavatel | 24,8 % | hrubá mzda |
| **Celkem** | **31,3 %** | — |

> ⚠️ **POZOR — ve vašich testech 6,5 % zaměstnanec, NE 7,1 %!**

### Zdravotní pojištění (ZP)

| Plátce | Sazba |
|--------|-------|
| **Zaměstnanec** | **4,5 %** |
| Zaměstnavatel | 9 % |
| **Celkem** | **13,5 %** |

### Daň z příjmu FO (zálohová)

| Pásmo | Sazba | Práh (2026) |
|-------|-------|-------------|
| Základní | **15 %** | do ~36× průměrné mzdy ročně |
| Solidární | **23 %** | nad limit (~131 901 Kč/měsíc) |

**Sleva na poplatníka 2026:** **30 840 Kč ročně** = **2 570 Kč měsíčně**.

---

## 🧮 VÝPOČET MZDY (postup krok za krokem)

```
Hrubá mzda (HM)
↓
+ SP zaměstnavatel (24,8 % z HM)   ← „superhrubá" už neplatí, ale počítá se
+ ZP zaměstnavatel (9 % z HM)

Z HM:
− SP zaměstnanec      6,5 % × HM
− ZP zaměstnanec      4,5 % × HM
− Záloha na daň       15 % × HM (zaokrouhlit na 100 nahoru)
+ Sleva na poplatníka 2 570 Kč

= ČISTÁ MZDA
```

### Příklad: HM 30 000 Kč

| Položka | Výpočet | Kč |
|---------|---------|-----|
| Hrubá mzda | — | 30 000 |
| SP zaměstnanec | 30 000 × 6,5 % | −1 950 |
| ZP zaměstnanec | 30 000 × 4,5 % | −1 350 |
| Záloha daně | 30 000 × 15 % = 4 500 → zaokr. 4 500 | −4 500 |
| Sleva na poplatníka | | +2 570 |
| **Čistá mzda** | | **24 770** |

---

## 🏭 ODPISY DLOUHODOBÉHO MAJETKU

### Odpisové skupiny (vzorové)

| Skupina | Doba odpisování | Příklady |
|---------|----------------|----------|
| 1 | 3 roky | počítače, kancelářské vybavení |
| 2 | 5 let | auta, stroje, nábytek |
| 3 | 10 let | výtahy, klimatizace |
| 4 | 20 let | budovy ze dřeva |
| 5 | 30 let | budovy z pevných materiálů |
| 6 | 50 let | hotely, administrativní budovy |

### Rovnoměrný odpis

```
1. rok:  vstupní cena × sazba_1.rok / 100
2.+ rok: vstupní cena × sazba_další / 100
```

| Skupina | 1. rok | Další roky |
|---------|--------|-----------|
| 1 | 20 % | 40 % |
| 2 | 11 % | 22,25 % |
| 3 | 5,5 % | 10,5 % |

**Příklad:** Auto 500 000 Kč, sk. 2.
- 1. rok: 500 000 × 11 % = **55 000 Kč**
- 2.–5. rok: 500 000 × 22,25 % = **111 250 Kč** každý rok
- Σ = 55 000 + 4 × 111 250 = 500 000 ✓

### Zrychlený odpis (degresivní)

```
1. rok:        vstupní cena ÷ koeficient_1.rok
další roky:    2 × zůstatková cena ÷ (koeficient_další − počet odepsaných let)
```

| Skupina | k₁ | k_další |
|---------|-----|---------|
| 1 | 3 | 4 |
| 2 | 5 | 6 |
| 3 | 10 | 11 |

---

## 📊 BOD ZVRATU (Break-even point)

```
BZ (ks)  = Fixní_náklady ÷ (cena_za_kus − variabilní_náklad_za_kus)
BZ (Kč)  = BZ_ks × cena_za_kus
```

**Příklad:** F = 100 000 Kč, cena = 200 Kč/ks, VN = 120 Kč/ks.
- BZ = 100 000 / (200 − 120) = 100 000 / 80 = **1 250 ks**
- v Kč: 1 250 × 200 = **250 000 Kč** musíš utržit, abys nebyl ve ztrátě.

---

## 📈 HDP (hrubý domácí produkt)

### 3 metody výpočtu

| Metoda | Vzorec | Co sčítá |
|--------|--------|----------|
| Produkční | Σ přidaných hodnot ve všech odvětvích | hodnotu vyrobenou |
| **Výdajová** | **C + I + G + (X − M)** | spotřebu + investice + vláda + čistý export |
| Důchodová | mzdy + zisky + renty + úroky | příjmy domácností |

- **Reálný HDP** = nominální / deflátor (očištěný od inflace)
- **HDP per capita** = HDP / počet obyvatel

---

## 💸 INFLACE

| Hladina | Roční růst CPI |
|---------|----------------|
| Plíživá | do 5 % |
| Pádivá | 5–10 % |
| Cválající | 10–50 % |
| **Hyperinflace** | **nad 150 %** ⚠️ (ve vašich testech!) |

> ⚠️ Standardní definice (Cagan) = >50 % měsíčně. **Ale ve vašich testech 150 %.** Pamatuj si svou hodnotu.

**Cíl ČNB:** **2 %** ± 1 procentní bod.

**Index spotřebitelských cen (CPI)** = poměr cen spotřebitelského koše k základnímu roku.

---

## 🏦 BANKOVNÍ SOUSTAVA ČR

**Dvoustupňová:**
1. **ČNB** (centrální banka) — emise, monetární politika, dohled
2. **Komerční banky** — KB, ČS, ČSOB, Moneta, Air Bank…

### Sazby ČNB (vzorově)

| Sazba | Co dělá |
|-------|---------|
| **Diskontní** | nejnižší, ČNB ji platí bankám za vklady |
| 2T repo | hlavní operativní (nyní např. 4,00 %) |
| Lombardní | nejvyšší, banky platí ČNB za úvěr |

> ⚠️ Ve vašich materiálech se mluví o **diskontní** jako základní. Pamatuj.

---

## 📐 ROZVAHA — bilanční rovnice

```
AKTIVA = PASIVA
```

### 4 typy účetních změn

| Typ | Aktiva | Pasiva | Příklad |
|-----|--------|--------|---------|
| 1 | + | + | nákup zásob na fakturu (zásoby↑, závazky↑) |
| 2 | − | − | platba dodavateli z účtu (BÚ↓, závazky↓) |
| 3 | +/− | beze změny | nákup zásob z hotovosti (zásoby↑, pokladna↓) |
| 4 | beze změny | +/− | převod zisku na rezervní fond (HV↓, RF↑) |

### Struktura

```
AKTIVA                          PASIVA
A. Pohledávky za upsaný kapitál  A. Vlastní kapitál
B. Dlouhodobý majetek            B. Cizí zdroje
   B.I. Nehmotný                    B.I. Rezervy
   B.II. Hmotný                     B.II. Závazky
   B.III. Finanční                C. Časové rozlišení
C. Oběžný majetek
   C.I. Zásoby
   C.II. Pohledávky
   C.III. Krátkodobý fin. majetek
D. Časové rozlišení
```

---

## 🎯 4P MARKETINGOVÉHO MIXU

| P | Anglicky | Co | Příklad |
|---|----------|-----|---------|
| **Produkt** | Product | co prodáváš | kvalita, design, značka |
| **Cena** | Price | za kolik | sleva, cenová strategie |
| **Distribuce** | Place | kde | e-shop, kamenný obchod |
| **Propagace** | Promotion | jak prodat | reklama, PR, sociální sítě |

Rozšíření na **7P**: + **People** (lidé), **Process** (proces), **Physical evidence** (hmotné prostředí) — pro služby.

---

## 🔍 SWOT ANALÝZA

```
                 INTERNÍ                EXTERNÍ
  POZITIVNÍ   ┌──────────────┐   ┌──────────────┐
              │  S Strengths │   │ O Opportunit.│
              │   (silné)    │   │ (příležitost)│
  NEGATIVNÍ   ├──────────────┤   ├──────────────┤
              │ W Weaknesses │   │  T Threats   │
              │   (slabé)    │   │  (hrozby)    │
              └──────────────┘   └──────────────┘
```

**Postup:**
1. Brainstorming všech 4 kvadrantů (5–8 položek)
2. Bodování (váha × intenzita)
3. Strategie:
   - **SO** — využít silné stránky pro příležitosti (ofenzivní)
   - **WO** — odstranit slabosti pro příležitosti
   - **ST** — využít silné stránky proti hrozbám
   - **WT** — minimalizovat slabosti i hrozby (defenzivní)

---

## 💼 DALŠÍ VZORCE

### Produktivita práce

```
P = výkon ÷ počet pracovníků      (naturální)
P = tržby ÷ mzdové náklady        (hodnotová)
```

### Plánování počtu zaměstnanců

```
Počet_zam = (objem_výkonů × normohodina) ÷ fond_pracovní_doby
```

### Zisk

```
Zisk = výnosy − náklady
EBIT = zisk před zdaněním a úroky
EAT  = čistý zisk po zdanění
```

### Fiskální vs monetární politika

| Politika | Provádí | Nástroje |
|----------|---------|----------|
| **Fiskální** | vláda | daně, výdaje, transfery, dotace |
| **Monetární** | ČNB | úrokové sazby, povinné minimální rezervy, operace na volném trhu |

---

## 🚨 SLABÁ MÍSTA — FIXOVAT NAPAMĚŤ

1. **DPH 21 / 12 / 0** — NE 15 %
2. **SP zaměstnanec 6,5 %** — NE 7,1 %
3. **Hyperinflace 150 %** — ve vašich testech
4. **ČNB sazba diskontní** jako základní — ne repo
5. **Daně PATŘÍ do fiskální politiky** (pozor na otázky „co NEpatří")
6. **Sleva na poplatníka 30 840 Kč/rok** = 2 570 Kč/měsíc
7. **Fakturace s DPH:** k základu se PŘIČÍTÁ DPH, neodečítá

---

📅 *Aktualizováno: 27. 4. 2026 · Před zkouškou zkontroluj sazby s nejnovějším EKO seminářem č. 1 a 11.*
