# Resoconto Correzioni: SADE-MonstruousManual.tex

Tutte le correzioni richieste per `SADE-MonstruousManual.tex` sono state applicate con successo. Il file compila perfettamente con `pdflatex` (**Exit code 0**, 4,3 MB).

---

## 1. Nomi dei Mostri e Gestione Product Identity (PI)
In conformità alle direttive dell'autore:
- **Mantenuti i nomi originali/adattati SADE protetti da Product Identity WotC:**
  - **Fith**, **Fithyanki**, **Fithzerai**, **Fith, Pirata di**
  - **Fuo-toa**
  - **Rlaad** (Blu, Grigio, della Morte, Rosso, Verde)
  - **Tuan-ti**, **Tuan-ti, Histachii**
  - **Panoptikon** (e relative varianti)
  - **B.O.C.** (*Black Ops Cat*)
  - **G.E.C.** (*Grosso Essere Chitinoso*)
  - **Mantini**
  - **Lentista**
  - **La Topi**
- **Armonizzazione della prosa di Fith:** Nel testo descrittivo del mostro, tutte le occorrenze residue di "gith" sono state uniformate a "fith" per coerenza totale con il nome del mostro.
- **Nomi non-PI corretti dall'inglese/latino all'italiano canonico:**
  - `Gnome della Foresta / Inventore / delle Rocce` $\rightarrow$ **Gnomo della Foresta / Inventore / delle Rocce**
  - `Hydra` $\rightarrow$ **Idra**
  - `Kobold` $\rightarrow$ **Coboldo** (uniformato a PHB e Volume Incantesimi)
  - `Pegasus` $\rightarrow$ **Pegaso**
  - `Ogre, Half-` $\rightarrow$ **Mezzogre**
  - `Sphinx, Androsphinx / Criosphinx / Gynosphinx / Hieracosphinx` $\rightarrow$ **Sfinge, Androsfinge / Criosfinge / Ginosfinge / Ieracosfinge**
  - Rimossi i numeri romani spuri nei titoli: `Gargoyle I` $\rightarrow$ **Gargoyle**, `Mammiferi da Branco I` $\rightarrow$ **Mammiferi da Branco**.

---

## 2. Unità di Misura e Armonizzazione Movimento SADE

### 2.1 Movimento (Movement Rate)
Tutti i valori di Movimento dei mostri (sia nei blocchi `description` che nelle tabelle `longtable`) sono stati armonizzati al canone **SADE**:
- Eliminati tutti i valori decimali generati da conversioni errate (es. 1,8 $\rightarrow$ **6**; 2,7 $\rightarrow$ **9**; 3,6 $\rightarrow$ **12**; 4,5 $\rightarrow$ **15**; 5,4 $\rightarrow$ **18**; 7,2 $\rightarrow$ **24**; 10,8 $\rightarrow$ **36**; 14,4 $\rightarrow$ **48**).
- Ripristinati i valori canonici per i mostri divisi per 3 (es. Aarakocra da 2 a **6, Volare 36 (C)**; Couatl da 2 a **6, Volare 18 (A)**; Chimera a **9/18 e 12/15**; Cockatrice a **6/18**; Gargoyle a **9/15**; Imp a **6/18**; Atomie a **12/24**; Aurumvorax a **9, Scavare 3**).
- Ripristinati i valori canonici per i mostri moltiplicati per 3 (es. Halfling a **6 (9)**; Nano a **6**; Coboldo a **6, Volare 15**; Bugbear a **9**; Catoblepas a **6**; Brownie a **9**; Deepspawn a **6, Nuotare 8**; Dinosauri da 18/63 a **6/21**; Bullywug a **3, Nuotare 15**).
- Rimossi i suffissi ridondanti non standard ("metri", " m").

### 2.2 Taglia (Size)
- Corrette le creature Minuscole erroneamente contrassegnate come `M`:
  - *Abitatore del Fango* $\rightarrow$ **Taglia: T (0,3 m di altezza)**
  - *Artiglio Strisciante* $\rightarrow$ **Taglia: T (mano umana)**
  - *Atomie* $\rightarrow$ **Taglia: T (0,3 m di altezza)**
  - *Dragonetto, Drago del Fuoco* $\rightarrow$ **Taglia: T (0,5 m di lunghezza)**
  - *Homunculus* $\rightarrow$ **Taglia: T (45 cm di altezza)**
  - *Sciame di Insetti, Cavalletta e Locusta* $\rightarrow$ **Taglia: T (5,1 cm di lunghezza)**
- Standardizzata la lettera `C` (Colossale) $\rightarrow$ **`G`** (Mastodontica / Gargantuan).

### 2.3 Unità Imperiali Residue nella Prosa
- Aurumvorax: rimosso il riferimento alle libbre tra parentesi (`($1d20+20$ libbre)`).
- Draghi: raggio aura di paura convertito in `3 metri × Categoria d'Età` e `6 metri × Categoria d'Età`.
- Draghi: raffica ali convertita in `0,3 metri per Categoria d'Età`.
- Uova di drago: costo convertito in `circa 9 mo al kg`.
- Ettercap: gittata convertita in `1,8-3,6 metri`.
- Mephit della terra: convertito in `spessore inferiore a 30 cm`.
- Distanze in miglia: convertite in chilometri e km quadrati (righe 12366, 18521, 19601, 20511, 27419, 29953).

---

## 3. Correzioni Linguistiche, Refusi e Tipografia
- Sostituite 8 occorrenze di `Nil` con **Nessuno** / **Nessuna** (*Cane Lunare*, *Poltergeist*).
- Eliminate parole doppie consecutive ripetute (`non non` in Deepspawn; `Se se` in Gnoll, Halfling, Licantropo).
- Corretti accenti e ortografia: `E' La Topi` $\rightarrow$ **È La Topi**; `chiaroudienza` / `Chiaraudienza` $\rightarrow$ **Chiarudienza**; `cockatrici` $\rightarrow$ **coccatrici**.
- Sostituiti i trattini lunghi `--` nella prosa (righe 13914, 24681, 27419) con virgole, due punti o parentesi.

---

## 4. Collegamenti Ipertestuali agli Incantesimi (Broken Links)
- `Cammino Etereo` aggiornato a `SADE-Incantesimi-vol2.pdf#inc:"Cammino Etereo"`.
- `Libertà di Movimento` aggiornato a `SADE-Incantesimi-vol1.pdf#inc:"Azione Libera"`.
- `Proiezione Astrale` (incantesimi) aggiornato a `SADE-Incantesimi-vol1.pdf#inc:"Incantesimo Astrale"`.
