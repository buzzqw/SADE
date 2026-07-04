<div align="center">

# S.AD.E.
### *Second ADvanced Edition*

*Un regolamento fantasy in lingua italiana, derivato da e compatibile con AD&D 2ª Edizione*

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](#licenza)
[![Scritto con pdfLaTeX](https://img.shields.io/badge/Scritto%20con-pdfLaTeX-008080.svg)](#compilazione)
[![Lingua: Italiano](https://img.shields.io/badge/Lingua-Italiano-009246.svg)](#i-manuali)
[![Pagine: 1500+](https://img.shields.io/badge/Pagine-1500%2B-blue.svg)](#i-manuali)
[![Incantesimi: 839](https://img.shields.io/badge/Incantesimi-839-9b59b6.svg)](#i-manuali)
[![Mostri: 396](https://img.shields.io/badge/Mostri-396-8b0000.svg)](#i-manuali)
[![Donate](https://img.shields.io/badge/Donate-PayPal-00457C.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=azanzani@gmail.com&item_name=Support+SADE+Project)

**[📖 Scarica il Manuale Base](SADE.pdf) · [🔮 Incantesimi](SADE-Incantesimi-vol1.pdf) · [👹 Mostruario](SADE-MonstruousManual.pdf) · [🛡️ Schermo del Master](screengem.pdf)**

</div>

<br>

> *La più grande delle avventure non si vive su una mappa, ma nell'immaginazione, attorno a un tavolo, tra amici pronti a sfidare l'impossibile armati solo di matite, dadi e coraggio.*

**S.AD.E.** è scritto da Andres Zanzani, ed è il frutto di anni di tavoli giocati, appunti a margine delle regole ufficiali e la testardaggine di chi non si è mai rassegnato a chiudere il libro di AD&D 2ª Edizione nel cassetto. Non è una semplice riproposizione del regolamento classico, ma una **rispettosa evoluzione**: l'obiettivo è catturare lo spirito e la profondità tattica dell'Advanced Dungeons & Dragons di seconda edizione, levigandone le asperità e avvicinandolo a uno stile di gioco più moderno e fluido, restando al contempo il più fedele possibile al materiale originale — pensato sia per i veterani nostalgici sia per chi si avvicina per la prima volta a questo stile di gioco.

Ogni pagina di questi manuali è composta a mano in LaTeX, tabella per tabella: **oltre 1.500 pagine** di regole, **839 incantesimi**, **243 poteri psionici** e **396 creature**, tutte tradotte, adattate e verificate incrocio dopo incrocio contro il materiale originale. Non un progetto "finito e dimenticato", ma un tavolo di lavoro sempre aperto.

---

## Indice

- [I manuali](#i-manuali)
- [Strumenti da tavolo](#strumenti-da-tavolo)
- [Struttura del repository](#struttura-del-repository)
- [Compilazione](#compilazione)
- [Supporta il progetto](#supporta-il-progetto)
- [Licenza](#licenza)

---

## I manuali

Tutti i manuali sono distribuiti **pronti da leggere** in PDF e **aperti da modificare** nel loro sorgente LaTeX: clicca sul nome del PDF per scaricarlo, oppure apri il `.tex` per vedere (o rimettere le mani) nel codice sorgente.

| Manuale | Contenuto | Pagine | Scarica | Sorgente |
|---|---|:---:|:---:|:---:|
| **Manuale Base** | Creazione del personaggio, razze, classi, kit, allineamento, competenze, specializzazione nelle armi, talenti, equipaggiamento, alleati e domini, combattimento, movimento, esplorazione, navigazione, magia, il pantheon, masterizzare (guida per il Game Master), tesori, oggetti magici, i piani di esistenza, le condizioni, oltre a un'appendice ("Giocare a SADE... senza SADE") che ripropone le tabelle regola per regola nella loro forma originale vanilla AD&D 2E, per chi preferisce disattivare le modifiche homebrew. | 345 | [📖 PDF](SADE.pdf) | [`SADE.tex`](SADE.tex) |
| **Incantesimi — Vol. I** | Il compendio della magia del *Player's Handbook*, tradotta e adattata in italiano incantesimo per incantesimo. **839 incantesimi** e **243 poteri psionici** in totale tra i due volumi. | 214 | [🔮 PDF](SADE-Incantesimi-vol1.pdf) | [`SADE-Incantesimi-vol1.tex`](SADE-Incantesimi-vol1.tex) |
| **Incantesimi — Vol. II** | La magia del *Tome of Magic* e i poteri psionici del *Complete Psionic Handbook*, con la stessa cura filologica del primo volume. | 286 | [🔮 PDF](SADE-Incantesimi-vol2.pdf) | [`SADE-Incantesimi-vol2.tex`](SADE-Incantesimi-vol2.tex) |
| **Mostruario** | Il bestiario completo in italiano: **396 creature**, ciascuna con THAC0 per Dadi Vita e tabelle di morale, pronte da portare al tavolo. | 653 | [👹 PDF](SADE-MonstruousManual.pdf) | [`SADE-MonstruousManual.tex`](SADE-MonstruousManual.tex) |

## Strumenti da tavolo

Oltre ai manuali, il repository include fogli di consultazione rapida pensati per essere stampati e usati durante le sessioni — le tabelle sono verificate riga per riga contro i `\label{tab:...}` dei manuali, non ricopiate a memoria.

| Strumento | Contenuto | Scarica | Sorgente |
|---|---|:---:|:---:|
| **Schermo del Master** *(beta, in miglioramento)* | 5 pannelli A4 orizzontali con le tabelle più consultate al tavolo: THAC0, tiri salvezza, scacciare non-morti, danno armi, incantesimi al giorno, esplorazione e incontri. | [🛡️ PDF](screengem.pdf) | [`screengem.tex`](screengem.tex) |

## Struttura del repository

Ogni file `.tex` è un documento **standalone** con il proprio preambolo completo: non esiste un grafo di `\input`/`\include` condiviso tra i volumi — puoi aprire un solo file e trovarci dentro tutto il necessario per compilarlo. La cartella [`immagini/`](immagini/) raccoglie le illustrazioni e gli asset grafici usati nei manuali.

## Compilazione

I manuali sono scritti in LaTeX e compilati con **pdfLaTeX**. `SADE.tex` usa `imakeidx` con indici multipli (analitico, Abilità, Incantesimi, Poteri Psionici, Mostruario, Oggetti Magici, Kit, Competenze, Equipaggiamento), che richiedono un passaggio `makeindex` dedicato per ciascuno prima della compilazione finale:

```bash
pdflatex -interaction=nonstopmode SADE.tex
makeindex -o SADE.ind SADE.idx
makeindex -o Kit.ind Kit.idx
# ... ripetere per ogni indice
pdflatex -interaction=nonstopmode SADE.tex   # 2-3 passate per assestare TOC/indici/riferimenti
```

Gli altri file (`SADE-Incantesimi-vol1.tex`, `SADE-Incantesimi-vol2.tex`, `SADE-MonstruousManual.tex`, la scheda del personaggio e lo schermo del master) si compilano allo stesso modo, con una singola passata di `pdflatex` e senza indici multipli.

## Supporta il progetto

S.AD.E. è un progetto scritto e mantenuto da una sola persona, nel tempo libero, per passione verso questo gioco. Se lo trovi utile al tuo tavolo e vuoi ringraziare l'autore, puoi offrirgli un caffè tramite PayPal — ogni contributo è molto apprezzato e aiuta a tenere vivo il progetto.

[![Dona con PayPal](https://img.shields.io/badge/Donate-PayPal-00457C.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=azanzani@gmail.com&item_name=Support+SADE+Project)

## Licenza

**S.AD.E.** © 2025 Andres Zanzani. Quest'opera è distribuita con licenza **Creative Commons Attribuzione - Non Commerciale - Condividi allo stesso modo 4.0 Internazionale (CC BY-NC-SA 4.0)**.

Maggiori dettagli nel capitolo "Immagini e Licenza" del manuale base.
</content>
</invoke>
