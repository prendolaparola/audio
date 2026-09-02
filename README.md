# Ascolti di "Prendo la parola"

Sito: **https://prendolaparola.github.io/audio/** — GitHub Pages da `main` / root.
Ogni traccia ha il suo indirizzo: `https://prendolaparola.github.io/audio/N/`, ed è
quello che finisce nel codice QR stampato sull'unità N del libro.

## La regola

**Cartella N = unità N = traccia N.** Dentro ogni cartella il file audio si chiama
sempre `traccia.mp3`. Il numero sta solo nel nome della cartella, mai nel nome dei
file: niente `traccia2.mp3`, niente `index2.html`.

```
index.html            elenco degli ascolti
1/index.html          player dell'unita 1   ->  <source src="traccia.mp3">
1/traccia.mp3         audio dell'unita 1
2/index.html          player dell'unita 2   ->  <source src="traccia.mp3">
2/traccia.mp3         audio dell'unita 2
_template-traccia/    modello da copiare, non e una traccia vera
```

Cosi il player non puo puntare all'audio di un'altra unita: nella sua cartella c'e
un solo file audio e si chiama sempre allo stesso modo. L'unico errore possibile e
mettere il file nella cartella sbagliata, e si sente al primo play.

## Tracce pubblicate

| N. | Titolo | Durata | Unita del libro | URL |
|----|--------|--------|-----------------|-----|
| 1 | Estratti A e B | 2:21 | 1 - Intelligenza artificiale e vita quotidiana | /audio/1/ |
| 2 | Lo butto oggi o lo butto domani? | 1:02 | 2 - Cibo: cucinare, ordinare, sprecare | /audio/2/ |

## Aggiungere la traccia dell'unita N

1. Copia `_template-traccia/` e rinominala `N/` (solo il numero: 3, 4, 10).
2. Nel suo `index.html` sostituisci `NUMERO` con N e `TITOLO DELL'ASCOLTO` con il titolo.
3. Metti l'audio nella cartella e chiamalo `traccia.mp3`.
4. Aggiungi la riga nell'elenco di `index.html` e nella tabella qui sopra.
5. Carica: **Add file > Upload files**, restando **nella radice** del repository,
   e trascina la cartella `N`.
6. Genera il QR per `https://prendolaparola.github.io/audio/N/`.

## L'errore da non rifare

Alla prima pubblicazione e stata trascinata la cartella `audio` invece del suo
contenuto: i file sono finiti in `audio/audio/1/` e l'indirizzo stampato sul QR
(`prendolaparola.github.io/audio/1/`) rispondeva 404. Si trascina il CONTENUTO,
mai la cartella che lo contiene.

## Prima di stampare un QR

- Apri `https://prendolaparola.github.io/audio/N/` dal telefono e fai partire l'audio.
- Scansiona il QR vero con la fotocamera: non fidarti dell'indirizzo scritto sotto.
- Stampa comunque l'URL in chiaro sotto al codice, come rete di sicurezza.

## Note

- Il QR e statico: l'indirizzo e dentro al disegno, non scade e non costa nulla.
  Si rompe solo se rinomini il repository, cambi username, rinomini le cartelle
  numerate o disattivi Pages.
- L'audio si sostituisce quando vuoi: se il file resta `traccia.mp3` nella stessa
  cartella, tutti i QR gia stampati puntano alla nuova registrazione.
- Il repository e pubblico: gli audio sono scaricabili da chiunque conosca l'URL.
  `controlslist="nodownload"` toglie il pulsante dal player, non protegge il file.
- I master degli audio e i PDF del libro stanno nell'altro repository, privato:
  `edwardds89/prendo-la-parola`.
