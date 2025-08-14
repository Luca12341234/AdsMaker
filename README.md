# README.md

# SponsorLock — segmento sponsorizzato non‑skippabile (Proof‑of‑Concept)

> **TL;DR**: questo repository contiene un prototipo di player che permette al creator di marcare un **intervallo non skippabile** dentro il proprio video. È pensato per **demo/valutazione**. L’uso in produzione o l’integrazione in servizi è **vietato** salvo licenza commerciale.

![badge](https://img.shields.io/badge/status-PoC-blue) ![license](https://img.shields.io/badge/license-Proprietary--Eval-lightgrey)

## Perché

Gli spot “nativi” dentro i video vengono spesso saltati con il seek. SponsorLock consente al creator di scegliere un **segmento non skippabile** (con regole di durata/cadenza) mantenendo la trasparenza verso l’utente.

## Funzioni principali

* Segmento **non skippabile** scelto dal creator (blocco del seek).
* Possibilità di **velocità libera** (0.5×–2×) durante il segmento.
* Overlay informativo “Contenuto sponsorizzato” con **barra di avanzamento**.
* **Token di completamento** (demo) quando il segmento termina.

> ⚠️ **Nota piattaforme**: questo PoC non modifica YouTube/Twitch. È destinato a **player proprietari** (es. siti/app del creator). L’uso su piattaforme terze richiede il rispetto dei relativi **Termini di Servizio** e/o accordi con la piattaforma.

## Demo rapida

1. Apri `index.html` in un browser moderno.
2. Clicca **Carica video demo** *oppure* carica un tuo file `.mp4`.
3. Imposta **Inizio/Fine** del segmento e clicca **Applica**.
4. Riproduci: nel tratto marcato non puoi **avanzare** con il seek (puoi solo tornare indietro). Alla fine del segmento, il player si **sblocca**.

## Struttura progetto

```
/             # questo repo
├─ index.html # prototipo single‑file (player + UI)
└─ LICENSE    # licenza Proprietary Evaluation
```

## Roadmap

* [ ] Più segmenti non‑skippabili per video.
* [ ] Integrazione HLS/DASH con marker nel manifest.
* [ ] Dashboard metriche e verifica lato server.
* [ ] Opzione "soft‑gate" (tasto Continua dopo N secondi).

## Licenza

Questo repository è rilasciato con **Proprietary Evaluation License** (vedi `LICENSE`).
**Non** è consentito l’uso commerciale, la ridistribuzione o l’integrazione in prodotti/servizi senza un accordo scritto.

Per ottenere una licenza commerciale: `contatto: you@example.com` (sostituisci con i tuoi dati).

## Avvertenze legali

* **Copyright**: © 2025, *\[Il tuo nome o alias]*. Tutti i diritti riservati.
* **Marchi**: *SponsorLock™* è un marchio non registrato dell’autore.
* **Brevetti**: questo rilascio **non concede** alcuna licenza su eventuali diritti di brevetto presenti o futuri. L’implementazione di funzionalità simili potrebbe richiedere una licenza separata.
* **Nessuna garanzia**: software fornito “as‑is”.

---

# LICENSE (Proprietary Evaluation License v1.0)

**SponsorLock — Proprietary Evaluation License v1.0**
Copyright (c) 2025 *\[Il tuo nome o alias]*. **Tutti i diritti riservati.**

## 1. Concessione limitata di licenza

Ti è concesso un diritto personale, non esclusivo, non trasferibile e revocabile a:

* visualizzare, clonare, compilare ed eseguire localmente il Software **solo** per **valutazione non commerciale** e demo interne;
* recensire il codice sorgente allo scopo di valutarne l’idoneità.

Qualsiasi altro uso è vietato senza **licenza commerciale scritta** dell’Autore.

## 2. Restrizioni

Senza previo consenso scritto **non puoi**:

* usare il Software **in produzione** o a fini **commerciali** (inclusi SaaS, servizi a terzi, campagne sponsor);
* modificare, creare opere derivate, distribuire, sublicenziare, vendere, affittare, ospitare o rendere disponibile pubblicamente il Software o parti di esso;
* rimuovere avvisi di copyright/marchio;
* combinare o collegare il Software a modo da aggirare queste restrizioni.

## 3. Proprietà intellettuale

Il Software è protetto da copyright e altre leggi. Questa licenza **non** concede alcuna licenza, espressa o implicita, su brevetti dell’Autore. L’uso di idee coperte da eventuali brevetti richiede licenza separata.

## 4. Feedback

Qualsiasi feedback è volontario e potrà essere usato dall’Autore **senza obbligo** di compenso o attribuzione.

## 5. Termine

La licenza termina automaticamente in caso di violazione. Alla cessazione devi cessare l’uso e distruggere le copie.

## 6. Esclusione di garanzia

IL SOFTWARE È FORNITO “COSÌ COM’È”, SENZA GARANZIE DI ALCUN TIPO, ESPLICITE O IMPLICITE.

## 7. Limitazione di responsabilità

In nessun caso l’Autore sarà responsabile per danni indiretti, speciali, incidentali o consequenziali.

## 8. Legge applicabile e foro

Questa licenza è regolata dalla legge **italiana**. Foro esclusivo: **\[la tua città]**.

---

> **Nota importante**: una **licenza proprietaria** protegge il tuo **codice** (chi copia/redistribuisce viola il diritto d’autore e il contratto). **Non** impedisce ad altri di implementare un’idea simile **da zero**; per quello serve un **brevetto**. Se ti serve, valuta un deposito nazionale per fissare la priorità.
