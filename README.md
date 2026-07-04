<div align="center">

# S.AD.E.
### *Second ADvanced Edition*

*Un regolamento fantasy in lingua italiana, derivato da e compatibile con AD&D 2ª Edizione*

</div>

<br>

> *La più grande delle avventure non si vive su una mappa, ma nell'immaginazione, attorno a un tavolo, tra amici pronti a sfidare l'impossibile armati solo di matite, dadi e coraggio.*

**S.AD.E.** è scritto da Andres Zanzani. Non è una semplice riproposizione del regolamento classico, ma una **rispettosa evoluzione**: l'obiettivo è catturare lo spirito e la profondità tattica dell'Advanced Dungeons & Dragons di seconda edizione, levigandone le asperità e avvicinandolo a uno stile di gioco più moderno e fluido, restando al contempo il più fedele possibile al materiale originale — pensato sia per i veterani nostalgici sia per chi si avvicina per la prima volta a questo stile di gioco.

---

## Indice

- [I manuali](#i-manuali)
- [Ambientazione](#ambientazione)
- [Strumenti da tavolo](#strumenti-da-tavolo)
- [Struttura del repository](#struttura-del-repository)
- [Compilazione](#compilazione)
- [Licenza](#licenza)

---

## I manuali

| File | Contenuto | Dimensione |
|---|---|:---:|
| [`SADE.tex`](SADE.tex) | Il manuale base. Creazione del personaggio, razze, classi, kit, allineamento, competenze, specializzazione nelle armi, talenti, equipaggiamento, alleati e domini, combattimento, movimento, esplorazione, navigazione, magia, il pantheon, masterizzare (guida per il Game Master), tesori, oggetti magici, i piani di esistenza, le condizioni, oltre a un'appendice ("Giocare a SADE... senza SADE") che ripropone le tabelle regola per regola nella loro forma originale vanilla AD&D 2E, per chi preferisce disattivare le modifiche homebrew. | 345 pagine |
| [`SADE-Incantesimi-vol1.tex`](SADE-Incantesimi-vol1.tex)<br>[`SADE-Incantesimi-vol2.tex`](SADE-Incantesimi-vol2.tex) | Il compendio completo degli incantesimi, tradotto e adattato in italiano: tutta la magia del *Player's Handbook*, del *Tome of Magic* e i poteri psionici del *Complete Psionic Handbook*, divisi in due volumi. | 214 + 286 pagine |
| [`SADE-MonstruousManual.tex`](SADE-MonstruousManual.tex) | Il mostruario completo in italiano, con tutte le creature, i valori di THAC0 per Dadi Vita e le tabelle di morale. | 653 pagine |

## Strumenti da tavolo

Oltre ai manuali, il repository include alcuni fogli di consultazione rapida pensati per essere stampati e usati durante le sessioni:

| File | Contenuto |
|---|---|
| [`screengem.tex`](screengem.tex) | Schermo del master: 5 pannelli A4 orizzontali con le tabelle più consultate al tavolo (THAC0, tiri salvezza, scacciare non-morti, danno armi, incantesimi al giorno, esplorazione e incontri), verificate contro il manuale base. |

## Struttura del repository

Ogni file `.tex` è un documento **standalone** con il proprio preambolo completo: non esiste un grafo di `\input`/`\include` condiviso tra i volumi. La cartella [`immagini/`](immagini/) raccoglie le illustrazioni e gli asset grafici usati nei manuali.

## Compilazione

I manuali sono scritti in LaTeX e compilati con **pdfLaTeX**. `SADE.tex` usa `imakeidx` con indici multipli (analitico, Abilità, Incantesimi, Poteri Psionici, Mostruario, Oggetti Magici, Kit, Competenze, Equipaggiamento), che richiedono un passaggio `makeindex` dedicato per ciascuno prima della compilazione finale:

```bash
pdflatex -interaction=nonstopmode SADE.tex
makeindex -o SADE.ind SADE.idx
makeindex -o Kit.ind Kit.idx
# ... ripetere per ogni indice
pdflatex -interaction=nonstopmode SADE.tex   # 2-3 passate per assestare TOC/indici/riferimenti
```

Gli altri file (`SADE-Incantesimi-vol1.tex`, `SADE-Incantesimi-vol2.tex`, `SADE-MonstruousManual.tex`, `SADE-Khorameth.tex`, la scheda del personaggio e lo schermo del master) si compilano allo stesso modo, con una singola passata di `pdflatex` e senza indici multipli.

## Licenza

**S.AD.E.** © 2025 Andres Zanzani. Quest'opera è distribuita con licenza **Creative Commons Attribuzione - Non Commerciale - Condividi allo stesso modo 4.0 Internazionale (CC BY-NC-SA 4.0)**.

Maggiori dettagli nel capitolo "Immagini e Licenza" del manuale base.
