# Ascolto con QR — istruzioni

**URL finale:** https://prendolaparola.github.io/audio/1/
**QR:** `qr-traccia-1.svg` (vettoriale, per la stampa) e `qr-traccia-1.png` (2050×2050 px)

Il repository `prendolaparola/audio` è già creato e pubblico. Mancano due passaggi.

---

## 1. Carica i file

Nella pagina del repo, clicca **"uploading an existing file"** (il link nel riquadro azzurro).

Poi apri la cartella `audio` che ti ho preparato e **trascina nella finestra del browser
questi due elementi**:

- il file `index.html`
- la cartella `1` (intera — GitHub mantiene la struttura)

Non trascinare la cartella `audio` stessa: finiresti con un livello di troppo e l'URL
diventerebbe `.../audio/audio/1/`.

La struttura corretta nel repo, a fine caricamento:

```
index.html          ← elenco delle tracce
1/
  index.html        ← pagina con il player
  traccia.mp3       ← il tuo file audio
```

In fondo alla pagina clicca **Commit changes**.

## 2. Attiva GitHub Pages

**Settings → Pages** (menù di sinistra)

- **Source:** `Deploy from a branch`
- **Branch:** `main` — cartella `/ (root)` → **Save**

Aspetta 1-2 minuti (la prima pubblicazione è la più lenta). Poi apri
https://prendolaparola.github.io/audio/1/ e verifica che l'audio parta,
possibilmente da telefono.

**Scansiona il QR con il tuo telefono prima di mandare in stampa.**

---

## 3. Stampa

- Usa l'**SVG** se il programma di impaginazione lo accetta: resta nitido a qualsiasi
  dimensione. Altrimenti il PNG.
- **Dimensione minima 2 × 2 cm.** Sotto diventa inaffidabile su carta economica.
- Lascia il **bordo bianco** attorno al codice — è già incluso nel file, non ritagliarlo.
- Nero su bianco, massimo contrasto. Niente colori tenui o bianco-su-nero.
- Stampa l'URL in chiaro sotto al QR, come rete di sicurezza:
  `prendolaparola.github.io/audio/1`

---

## Sulle scadenze

Questo QR è **statico**: l'indirizzo è codificato nel disegno stesso, non passa da nessun
servizio intermedio. Non c'è niente da pagare e niente che possa scadere. I QR che
"scadono" sono quelli **dinamici** dei generatori commerciali, che ti fanno passare dai
loro server: quando smetti di pagare, spengono il redirect. Qui non succede.

Le uniche cose che possono rompere il link, tutte sotto il tuo controllo:

- cancellare o rinominare il repository `audio`
- cambiare l'username GitHub `prendolaparola`
- rinominare la cartella `1/` o disattivare Pages

Il **contenuto** invece lo cambi quando vuoi: sostituisci `traccia.mp3` con un'altra
registrazione e tutti i QR già stampati punteranno automaticamente alla nuova.

## Se vuoi essere blindato al 100%

Compra un dominio tuo (~10€/anno) e puntalo sul repo (Settings → Pages → Custom domain).
L'URL diventa `tuodominio.it/audio/1/` e da quel momento sei indipendente anche da GitHub:
se un giorno cambi hosting, i QR stampati continuano a funzionare.
Da fare **prima** di stampare, però: il QR va rigenerato con il nuovo indirizzo.

## Per aggiungere altre tracce

Crea le cartelle `2/`, `3/` ecc. con la stessa struttura (`index.html` + `traccia.mp3`),
cambiando titolo e numero nella pagina. Poi chiedimi i QR corrispondenti.
