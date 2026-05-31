# Come organizzo Obsidian come secondo cervello, non come un altro cassetto digitale

L'idea di "secondo cervello" viene spesso raccontata come se bastasse installare un'app, creare qualche cartella ordinata e iniziare a salvare link.

Non basta.

Quello crea inventario. Non crea pensiero.

Un secondo cervello utile non è il posto dove salvi tutto. È il sistema che ti aiuta a tornare a un'idea quando può migliorare una decisione, un progetto o una spiegazione.

Obsidian funziona bene per questo perché non ti obbliga a trattare la conoscenza come documenti isolati. Ti dà file Markdown, link, proprietà, alias, Map of Content e query. Ma proprio questa flessibilità rende facile progettare troppo.

Troppe cartelle. Troppi plugin. Troppi campi. Troppi tag.

A un certo punto il sistema richiede più energia di quanta ne restituisca.

Il mio approccio è più semplice: poche cartelle, note collegate, metadati minimi e revisione regolare.

## 1. Le cartelle sono vaschette, non l'architettura della conoscenza

Una cartella funziona bene quando descrive lo stato di una nota:

```txt
0-Inbox
1-Templates
2-Notes
3-Media
```

Questo è utile.

- Inbox: cattura rapida e materiale non ancora processato.
- Templates: strutture riutilizzabili.
- Notes: conoscenza già integrata.
- Media: PDF, immagini, disegni, audio e file esterni.

Funziona meno bene quando proviamo a far rappresentare alle cartelle tutta la conoscenza. Un'idea reale raramente appartiene a un solo posto. Una nota sull'apprendimento può toccare università, carriera, psicologia, lingue e produttività.

Se la struttura dipende solo dalle cartelle, il sistema ti obbliga a scegliere una scatola.

Per questo preferisco che le cartelle descrivano il flusso di lavoro, mentre il significato vive nei link, nelle proprietà e nelle mappe.

## 2. I MOC sono migliori di una tassonomia rigida

Un MOC, Map of Content, è una nota indice. Non è una cartella mascherata. È una porta d'ingresso a un tema.

Un MOC `Languages`, per esempio, può collegare italiano, inglese, grammatica, vocabolario, espressioni, confronti tra lingue e risorse. La parte importante è che la mappa può includere giudizio umano: note principali, note collegate, domande aperte, query dinamiche e regole d'uso.

Un tag ti dice che qualcosa appartiene a un tema. Un MOC ti aiuta a navigarlo.

Quando un tema cresce, non devo riorganizzare tutto il vault. Creo o aggiorno un MOC. La conoscenza resta collegata senza dipendere da una gerarchia perfetta.

## 3. Le proprietà servono per recuperare, non per decorare

Le Properties di Obsidian sono potenti se usate con misura. Diventano burocrazia se ogni nota richiede venti campi prima ancora di scrivere.

Un modello piccolo basta:

```yaml
type: note
area:
  - learning
topics:
  - "[[Obsidian]]"
  - "[[PKM]]"
aliases:
status: draft
lang:
  - en
created: 2026-05-31
updated: 2026-05-31
```

Ogni campo deve rispondere a una domanda reale:

- `type`: che tipo di nota è?
- `area`: dove appartiene principalmente?
- `topics`: a quali temi si collega?
- `aliases`: con quali altri nomi potrei cercarla?
- `status`: è bozza, attiva, stabile, privata o archiviata?
- `lang`: in che lingua è scritta?
- `next_action`: qual è il prossimo passo, se esiste?

Se un campo non aiuta a cercare, filtrare, rivedere o agire, probabilmente è rumore.

## 4. Dataview e Bases servono per la revisione, non per pensare al posto tuo

Le query sono utili perché mostrano lo stato del sistema:

- note senza area;
- progetti senza prossima azione;
- idee attive;
- task aperti;
- scadenze vicine;
- bozze da processare.

Una dashboard con Dataview può essere molto pratica. Ma c'è una trappola: passare più tempo a perfezionare la dashboard che a pensare davvero attraverso le note.

La query non fa il lavoro intellettuale. Lo rende solo visibile.

Una buona nota ha ancora bisogno di qualcosa di più semplice: spiegare un'idea con parole tue, collegarla ad altre idee e decidere a cosa serve.

## 5. Prendere note non significa copiare. Significa processare.

Quando leggo un libro o guardo un video, cerco di non copiare interi paragrafi. La fonte esiste già.

La nota dovrebbe obbligarmi a recuperare e riformulare:

1. leggo o ascolto un'idea;
2. chiudo la fonte;
3. provo a spiegarla con parole mie;
4. torno alla fonte solo se non riesco a formularla bene;
5. copio letteralmente solo definizioni, citazioni o frasi che meritano di restare identiche.

Così prendere note diventa più vicino all'active recall che al collezionismo digitale.

L'obiettivo non è costruire una biblioteca di frammenti. È costruire una rete di idee comprese.

## 6. Una nota piccola può essere migliore di una nota enorme

Spesso creiamo note gigantesche per temi generali: `Intelligenza Artificiale`, `Produttività`, `Italiano`, `Sistemi Operativi`, `Economia`.

Le note grandi vanno bene quando funzionano come mappe. Il problema nasce quando una sola nota prova a contenere tutto.

Se una sezione inizia ad avere vita propria, merita una nota separata.

La granularità giusta non è la regola dogmatica "una nota per idea". Una regola migliore è: se un'idea può essere riutilizzata, collegata o sviluppata in modo indipendente, dalle una nota.

## 7. La revisione settimanale mantiene vivo il sistema

Un vault si degrada per accumulo. Catturare è facile. Processare è il vero lavoro.

Una revisione settimanale minima può bastare:

- svuotare Inbox;
- eliminare catture di basso valore;
- trasformare le catture utili in note reali;
- collegare note isolate ai MOC;
- rivedere progetti e idee attive;
- aggiornare le prossime azioni;
- trovare bozze aperte da troppo tempo.

Senza revisione, Obsidian diventa un altro posto dove nascondere pensiero non finito.

## 8. La regola finale

Una nota appartiene al sistema se fa almeno una di queste cose:

- chiarisce un'idea;
- collega idee;
- funziona come mappa;
- registra qualcosa di importante;
- trasforma una fonte in comprensione personale;
- lascia una prossima azione chiara.

Se non fa nessuna di queste cose, probabilmente non appartiene al tuo secondo cervello.

## Starter kit pubblico

Ho preparato uno starter kit pubblico con template puliti, esempi di MOC, una dashboard, query Dataview e una checklist per la privacy.

Il punto non è pubblicare un vault reale. Sarebbe un errore. I vault reali contengono contesto privato, nomi, decisioni, emozioni, percorsi, file e link che non appartengono a GitHub.

Ha senso pubblicare il sistema: regole, template puliti ed esempi generici.

Repository: `obsidian-second-brain-starter`

Se usi Obsidian, il mio consiglio è semplice: parti piccolo. Non progettare il sistema perfetto. Progetta il sistema che ti aiuta a pensare meglio questa settimana.
