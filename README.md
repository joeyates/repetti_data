# Repetti Data

Questo repository contiene i dati del Dizionario Geografico Storico della Toscana
di Emanuele Repetti, pubblicato tra il 1833 e il 1846.

I dati sono disponibili in formato JSON e sono rilasciati con licenza CC0 1.0 Universal
(CC0 1.0) Public Domain Dedication.

I dati sono inseriti nel database del sito https://www.dizionario-repetti.it,
che permette di cercare i luoghi e le località della Toscana storica.

# I File

I file principali sono `vol_I-articles.json`, `vol_II-articles.json`, ecc,
che contengono gli articoli del dizionario, e `vol_I-places.json`, `vol_II-places.json`,
ecc, che contengono i dati derivati
dalle scansioni dei PDF prodotti dall'Università di Siena e scaricati dall'Internet Archive
([esempio](https://web.archive.org/web/20220122004606if_/http://stats-1.archeogr.unisi.it/repetti/documenti/vol_I.pdf)).

Gli altri file contengono metadati.

I file `vol_I-first-in-page.json`, `vol_II-first-in-page.json`, ecc,
contengono il titolo del primo articolo di ogni pagina
del volume, nella pubblicazione originale dell'opera.

Il file `coordinates.json` contiene le coordinate geografiche dei luoghi e delle località.
Alcune coordinate sono state estratte dal testo originale, ma, principalmente
sono state individuate manualmente, con l'ausilio dei dati di OpenStreetMap.

# Correzioni e Integrazioni

I testi preparati dall'Università di Siena erano modificati rispetto al testo originale
con la sostituzione di parole intere al posto delle abbreviazioni usate dal Repetti.

I dati provenienti sono stati corretti **solo** dove non rispecchiano il testo originale.

# Contribuire

Se vuoi contribuire, apri una pull request con la correzione o integrazione.

Le correzioni ai file `vol_XXX-articles.json` vanno fatte
esclusivamente nei campi `title`, `context` e `body`.
Gli altri campi riguardano i dati effettivamente presenti nei PDF di base e servono
solo come riferimenti a quei file.

Se correggi un titolo, in uno dei file `vol_XXX-articles.json`, controllare
se ci sono riferimenti a quel titolo in altri file, come `vol_XXX-first-in-page.json`
o `coordinates.json`, e correggi anche quelli.

L'aggiunta di coordinate geografiche in `coordinates.json` è molto apprezzata.
È essenziale che il campo `title` corrisponda esattamente al titolo dell'articolo
nei file `vol_XXX-articles.json`.

# Licenza

I dati sono rilasciati con licenza CC0 1.0 Universal (CC0 1.0) Public Domain Dedication.
