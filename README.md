# Code promo Amazon, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Amazon** depuis [shopilo.fr](https://shopilo.fr/reductions/amazon.fr). Renvoie les **coupons Amazon** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-amazon](https://shopilo-fr.github.io/code-promo-amazon/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-amazon
cd code-promo-amazon
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Amazon",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur une selection de produits",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/amazon.fr"
  }
]
```

## Coupons Amazon disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur une selection de produits | [shopilo.fr](https://shopilo.fr/reductions/amazon.fr) |

Codes actifs : **[shopilo.fr/reductions/amazon.fr](https://shopilo.fr/reductions/amazon.fr)**

## Questions frequentes

### Comment utiliser un code promo Amazon ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/amazon.fr), ajoutez les produits a votre panier sur Amazon et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Amazon ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Amazon les plus recents ?
La page [shopilo.fr/reductions/amazon.fr](https://shopilo.fr/reductions/amazon.fr) est mise a jour quotidiennement avec les codes promo Amazon, bons de reduction Amazon et coupons promotionnels Amazon les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Amazon

Amazon est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/amazon.fr), retrouvez les meilleurs codes promo Amazon, coupons Amazon verifies et bons de reduction Amazon actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-amazon
```

```javascript
const { fetchCoupons } = require('code-promo-amazon');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
