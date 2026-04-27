# Prompt 1 — Strukturované shrnutí + mapa pojmů

**Použití:** po přečtení kapitoly / semináře / PDF.
**Vstup:** školní text, skripta, učebnice.
**Výstup:** TL;DR + klíčové pojmy + mapa souvislostí + hierarchie + pasti.

---

## 📋 PROMPT (kopíruj celé do Claude / ChatGPT)

```
Jsi zkušený tutor a didaktik. Dostaneš školní podklad (text, skripta, učebnici).
Tvým úkolem je vytvořit jasný studijní přehled v češtině.

Výstup strukturuj PŘESNĚ takto:

1. **TL;DR (3 věty):** O čem to celé je a proč to je důležité.
2. **Klíčové pojmy (5–10):** Každý pojem → definice jednou větou + příklad.
3. **Mapa souvislostí:** Odrážkový seznam „co souvisí s čím" (pojem A → vede k → pojem B, protože...).
4. **Hierarchie důležitosti:**
   - 🔴 MUSÍŠ UMĚT (základ, na kterém stojí zbytek)
   - 🟡 MĚL BYS UMĚT (rozšiřuje základ)
   - 🟢 DOBRÉ VĚDĚT (detaily, příklady)
5. **Největší pasti:** 3 místa, kde studenti typicky chybují nebo se ztrácejí.

Piš jednoduše, krátké věty. Žádný akademický žargon navíc.
Když text obsahuje vzorce/výpočty, zachovej je doslova.

VSTUP (školní podklad):
[SEM VLOŽ TEXT]
```

---

## 💡 Tipy pro lepší výstup

- **Vlož celý PDF** (Claude umí přečíst PDF přímo).
- Pokud je text >30 stran, dej ho po kapitolách — výstup bude přesnější.
- Po vygenerování si **přepiš 🔴 MUSÍŠ UMĚT** rukou — fixace v paměti.
- Uložené výstupy patří do `shrnuti/` (pojmenuj `SHRNUTI_TEMA_XX.md`).

## 🔗 Návaznost

→ Pak pusť **Prompt 2** (`02_flashcards.md`) na stejný text.
