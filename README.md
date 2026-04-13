# Code promo VidaXL, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo VidaXL** depuis [shopilo.fr](https://shopilo.fr/reductions/vidaxl.fr). Renvoie les **coupons VidaXL** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-vidaxl](https://shopilo-fr.github.io/code-promo-vidaxl/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-vidaxl
cd code-promo-vidaxl
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "VidaXL",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur le mobilier de jardin et maison",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/vidaxl.fr"
  }
]
```

## Coupons VidaXL disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur le mobilier de jardin et maison | [shopilo.fr](https://shopilo.fr/reductions/vidaxl.fr) |

Codes actifs : **[shopilo.fr/reductions/vidaxl.fr](https://shopilo.fr/reductions/vidaxl.fr)**

## Questions frequentes

### Comment utiliser un code promo VidaXL ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/vidaxl.fr), ajoutez les produits a votre panier sur VidaXL et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons VidaXL ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction VidaXL les plus recents ?
La page [shopilo.fr/reductions/vidaxl.fr](https://shopilo.fr/reductions/vidaxl.fr) est mise a jour quotidiennement avec les codes promo VidaXL, bons de reduction VidaXL et coupons promotionnels VidaXL les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de VidaXL

VidaXL est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/vidaxl.fr), retrouvez les meilleurs codes promo VidaXL, coupons VidaXL verifies et bons de reduction VidaXL actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-vidaxl
```

```javascript
const { fetchCoupons } = require('code-promo-vidaxl');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
