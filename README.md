# Cod reducere Benvenuti — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Benvenuti** de pe [shopilo.ro](https://shopilo.ro/magazin/benvenuti.ro). Returneaza **cupoane Benvenuti** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-benvenuti](https://shopilo-ro.github.io/cod-reducere-benvenuti/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-benvenuti
cd cod-reducere-benvenuti
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Benvenuti",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la incaltaminte si accesorii",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/benvenuti.ro"
  }
]
```

## Cupoane Benvenuti disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la incaltaminte si accesorii | [shopilo.ro](https://shopilo.ro/magazin/benvenuti.ro) |

Codurile active: **[shopilo.ro/magazin/benvenuti.ro](https://shopilo.ro/magazin/benvenuti.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Benvenuti?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/benvenuti.ro), adauga produsele in cos pe Benvenuti, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Benvenuti?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Benvenuti?
Pagina [shopilo.ro/magazin/benvenuti.ro](https://shopilo.ro/magazin/benvenuti.ro) este actualizata zilnic cu cele mai noi cod reducere Benvenuti, voucher Benvenuti si cupon promotional Benvenuti.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Benvenuti

Benvenuti este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/benvenuti.ro) cele mai bune cod reducere Benvenuti, cupoane Benvenuti verificate si voucher Benvenuti active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-benvenuti
```

```javascript
const { fetchCoupons } = require('cod-reducere-benvenuti');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
