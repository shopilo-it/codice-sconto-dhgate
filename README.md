# Codice sconto DHgate, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto DHgate** da [shopilo.it](https://shopilo.it/negozi/dhgate.com). Restituisce **coupon DHgate** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-dhgate](https://shopilo-it.github.io/codice-sconto-dhgate/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-dhgate
cd codice-sconto-dhgate
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "DHgate",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto sul primo ordine",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/dhgate.com"
  }
]
```

## Coupon DHgate disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto sul primo ordine | [shopilo.it](https://shopilo.it/negozi/dhgate.com) |

Codici attivi: **[shopilo.it/negozi/dhgate.com](https://shopilo.it/negozi/dhgate.com)**

## Domande frequenti

### Come utilizzo un codice sconto DHgate?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/dhgate.com), aggiungi i prodotti al carrello su DHgate e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon DHgate?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher DHgate piu recenti?
La pagina [shopilo.it/negozi/dhgate.com](https://shopilo.it/negozi/dhgate.com) viene aggiornata quotidianamente con i codici sconto DHgate, voucher DHgate e coupon promozionali DHgate piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su DHgate

DHgate e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/dhgate.com) trovi i migliori codici sconto DHgate, coupon DHgate verificati e voucher DHgate attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-dhgate
```

```javascript
const { fetchCoupons } = require('codice-sconto-dhgate');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
