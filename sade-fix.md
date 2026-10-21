# Riepilogo Correzioni e Armonizzazione SADE

Documento generato a seguito della revisione linguistica, strutturale e regolistica del testo di **SADE (Second ADvanced Edition)** in [`SADE.tex`](file:///home/azanzani/SADE/SADE.tex).

---

## 1. Correzioni Ortografiche, Morfologiche e Refusi

- **Abilità Magus (*Incantesimo da Combattimento*):** corretti i tre refusi (`ablità` $\to$ `abilità`, `e'` $\to$ `è`, `comulabile` $\to$ `cumulabile`).
- **Tabella Armature ed Elmi:** corretto il refuso `armarmatura` $\to$ `armatura`.
- **Appendice Classi:**
  - Corretto `Dadi Vida` $\to$ `Dadi Vita` (progressione Ranger).
  - Corretto `a discrizione` $\to$ `a discrezione`.
- **Appendice N e Crediti:**
  - Corretto `Dungeon Masters Guide` $\to$ `Dungeon Master's Guide`.
  - Corretta spaziatura e punteggiatura in `Dungeons & Dragons` e `Wizards of the Coast`.
- **Apostrofi ed Elisioni:** armonizzati accenti ed elisioni (`All'8°`, `d'azzardo`, `aure distinte`, `davanti a una caotica massa`).

---

## 2. Layout, Tipografia e Impaginazione LaTeX

- **Indici Analitici di Fine Volume:**
  - Risolto il problema per cui il titolo dell'indice tagliava orizzontalmente le colonne adiacenti dei sottomoduli (rilevato in `/home/azanzani/Istantanea_2026-10-21_12-30-55.png`).
  - Creata la macro `\indexheading` con modulo protetto `\needspace{3\baselineskip}` e `\begin{minipage}{\linewidth}`, che applica il filetto separatore `\rule{\linewidth}{1.2pt}` limitato alla singola colonna e configurato via `\indexsetup{level=\indexheading, firstpagestyle=fancy}`.

---

## 3. Armonizzazione Meccanica e Incongruenze Regolistiche (Audit OSR)

### A. Combattimento e Mortalità
1. **Progressione attacchi 3/2:**
   - Armonizzata la sequenza su due round sia nel manuale base che nell'appendice a: *"1 attacco nel primo round, 2 attacchi nel secondo round, poi si ripete"* (standard classico AD&D 2E).
2. **Regola Formale Morte e Moribondo (0 PF / −10 PF):**
   - Inserita la sezione formale mancante `\subsection{Ferite, Moribondo e Morte}`:
     - **0 PF o meno:** personaggio incosciente e indifeso; perde 1 PF a round per dissanguamento.
     - **Stabilizzazione:** tramite prova di *Primo Soccorso* o incantesimi di cura; ferma il dissanguamento ma mantiene l'inconscienza fino a PF positivi.
     - **Morte definitiva:** a −10 PF (o danno massiccio negativo pari ai PF massimi in un solo colpo).
3. **Scacciare Non-Morti (Dado):**
   - Corretta la legenda delle tabelle di scacciare non-morti: rimpiazzato il refuso `2d10` con `1d20`, coerentemente con la scala numerica (4, 7, 10, 13, 16, 19, 20) e con la procedura descritta nel testo.
4. **Protezione degli Elmi e Classe Armatura:**
   - Chiarito che il bonus alla CA concesso dagli elmi (+1 cuoio, +2 grande elmo) si applica esclusivamente ai colpi mirati alla testa, evitando il bug che rendeva l'elmo un bonus sommabile indiscriminatamente all'armatura base.

### B. Classi, Razze e Personaggi
5. **Incantesimi del Ranger:**
   - Fissato l'accesso agli incantesimi all'**8° livello** sia nella scheda della classe base sia nell'appendice, eliminando il riferimento al 7° livello.
6. **Seguaci del Paladino:**
   - Armonizzata la dicitura: non attira un corpo di soldati generici come il Guerriero, ma ha diritto a scudieri e a un seguito religioso/paladinesco alla fondazione della roccaforte.
7. **Dadi Vita del Barbaro:**
   - Esplicitato e confermato il dado vita **d12** con apposita nota alla tabella dei combattenti.
8. **Modificatori di Scalata Razziali:**
   - Separati i valori di Gnomi (-5%) e Halfling (-15%) nella tabella generale dell'esplorazione, allineandoli esattamente ai modificatori razziali della tabella Ladro.
9. **Bonus Costituzione +3 e +4:**
   - Esplicitata la nota per cui i bonus superiori a +2 sono riservati ai Combattenti.

### C. Magia ed Economia
10. **Numero Scuole di Magia Arcana:**
    - Corretto il testo introduttivo a *"undici scuole di magia"*, corrispondente alle 11 voci elencate (incluse Magia Selvaggia, Divinazione Minore e Universale).
11. **Sfere Sacerdotali:**
    - Aggiunta nota chiarificatrice che spiega la presenza delle sfere addizionali da *Tome of Magic* (Caos, Fato, Legge, Numeri, Pensiero, Tempo, Viaggio) utilizzabili per la creazione con Punti Personaggio e per i culti specifici.
12. **Trucchetti (Livello 0):**
    - Aggiunto il minimo garantito di 1 trucchetto memorizzabile per Maghi e Chierici con INT/SAG senza linguaggi bonus.
13. **Tratto Umano Bonus PE:**
    - Specificata la cumulabilità del +5% PE da tratto umano con il +5% conferito dal requisito primario 16+.
14. **Prezzo della Partigiana:**
    - Corretto il prezzo di acquisto da 55 mo a 6 mo nella tabella delle armi in asta.
15. **Velocità di Viaggio Terrestre:**
    - Uniformata la distanza giornaliera a piedi su terreno pianeggiante a 21 km (6m), 32 km (9m) e 43 km (12m).

---

## 4. Stato Finale della Compilazione

- **Documento:** [`SADE.tex`](file:///home/azanzani/SADE/SADE.tex)
- **Output:** [`SADE.pdf`](file:///home/azanzani/SADE/SADE.pdf) (349 pagine)
- **Compilazione:** `pdflatex -interaction=nonstopmode SADE.tex` (stabilizzata su due passaggi completi, 0 errori bloccanti).
