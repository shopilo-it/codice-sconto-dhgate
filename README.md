# Cod reducere DHgate — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere DHgate** de pe [shopilo.it](https://shopilo.it/magazin/dhgate.com). Returneaza **cupoane DHgate** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-dhgate](https://shopilo-it.github.io/codice-sconto-dhgate/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-dhgate
cd codice-sconto-dhgate
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "DHgate",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto sul primo ordine",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/dhgate.com"
  }
]
```

## Cupoane DHgate disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% di sconto sul primo ordine | [shopilo.it](https://shopilo.it/magazin/dhgate.com) |

Codurile active: **[shopilo.it/magazin/dhgate.com](https://shopilo.it/magazin/dhgate.com)**

## Intrebari frecvente

### Cum folosesc un cod de reducere DHgate?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/dhgate.com), adauga produsele in cos pe DHgate, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele DHgate?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri DHgate?
Pagina [shopilo.it/magazin/dhgate.com](https://shopilo.it/magazin/dhgate.com) este actualizata zilnic cu cele mai noi cod reducere DHgate, voucher DHgate si cupon promotional DHgate.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre DHgate

DHgate este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/dhgate.com) cele mai bune cod reducere DHgate, cupoane DHgate verificate si voucher DHgate active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-dhgate
```

```javascript
const { fetchCoupons } = require('codice-sconto-dhgate');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)
