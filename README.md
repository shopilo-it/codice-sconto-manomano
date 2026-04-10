# Codice sconto ManoMano, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto ManoMano** da [shopilo.it](https://shopilo.it/negozi/manomano.it). Restituisce **coupon ManoMano** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-manomano](https://shopilo-it.github.io/codice-sconto-manomano/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-manomano
cd codice-sconto-manomano
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "ManoMano",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su fai da te e giardinaggio",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/manomano.it"
  }
]
```

## Coupon ManoMano disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su fai da te e giardinaggio | [shopilo.it](https://shopilo.it/negozi/manomano.it) |

Codici attivi: **[shopilo.it/negozi/manomano.it](https://shopilo.it/negozi/manomano.it)**

## Domande frequenti

### Come utilizzo un codice sconto ManoMano?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/manomano.it), aggiungi i prodotti al carrello su ManoMano e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon ManoMano?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher ManoMano piu recenti?
La pagina [shopilo.it/negozi/manomano.it](https://shopilo.it/negozi/manomano.it) viene aggiornata quotidianamente con i codici sconto ManoMano, voucher ManoMano e coupon promozionali ManoMano piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su ManoMano

ManoMano e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/manomano.it) trovi i migliori codici sconto ManoMano, coupon ManoMano verificati e voucher ManoMano attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-manomano
```

```javascript
const { fetchCoupons } = require('codice-sconto-manomano');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
