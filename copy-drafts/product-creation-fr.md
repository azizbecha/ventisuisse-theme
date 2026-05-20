# VentiSuisse — Création du produit (FR)

Guide complet pour créer le produit dans Shopify Admin → Products → Add product.
Toutes les valeurs ci-dessous sont prêtes à coller, dans l'ordre où elles apparaissent dans le formulaire.

---

## 1. Title (en haut de la page)

```
VentiSuisse — Gourde de trail
```

---

## 2. Description (éditeur de texte enrichi)

Cliquer sur l'icône `<>` (source HTML) dans la barre d'outils, puis coller :

```html
<p><strong>Une bouteille. Un bol. Des sentiers sans fin.</strong></p>
<p>Vous marchez, votre chien suit. Jusqu'ici, ça voulait dire : porter deux bouteilles — ou faire demi-tour quand l'eau était finie.</p>
<p>La gourde VentiSuisse résout ça en un seul objet. Une bouteille en inox double paroi de 285 ml — avec un panneau en silicone flexible qui s'ouvre d'une pression du pouce pour former un bol intégré. Vous avez de l'eau fraîche. Votre chien a un bol propre. Voilà.</p>
<ul>
  <li><strong>Étanche.</strong> Le bouchon se ferme hermétiquement. Glissez-la dans le sac à dos — pas une goutte.</li>
  <li><strong>Isolation double paroi.</strong> L'eau reste fraîche même après des heures au soleil.</li>
  <li><strong>Matériaux de qualité alimentaire.</strong> Inox 304 (intérieur), silicone sans BPA (bol).</li>
  <li><strong>Légère pour le trail.</strong> 150 g à vide. 285 ml de contenance. 9 × 9 × 8,7 cm compact.</li>
  <li><strong>Deux couleurs.</strong> Sky Blue ou Pink — choisissez celle qui convient à votre chien.</li>
</ul>
<p>Livraison en Suisse en 1–3 jours ouvrables. Offerte dès CHF 49. Retours sous 30 jours, sans question.</p>
```

---

## 3. Media (glisser-déposer)

Glissez ces 6 fichiers depuis `~/code/ventisuisse-theme/assets/`, **dans cet ordre** (le premier devient l'image principale) :

1. `vs-hero-corgi.jpg` ← image hero / principale
2. `vs-product-teal.jpg`
3. `vs-product-pink.jpg`
4. `vs-product-folding.jpg`
5. `vs-product-variants.jpg`
6. `vs-product-steel.jpg`

---

## 4. Pricing (Tarification)

| Champ                       | Valeur     |
|-----------------------------|------------|
| **Price**                   | `34.90`    |
| **Compare-at price**        | (vide)     |
| **Cost per item**           | (vide)     |
| **Charge tax on this product** | ✅ coché (pour appliquer la MWST 8.1%) |

---

## 5. Inventory (Inventaire)

| Champ                             | Valeur     |
|-----------------------------------|------------|
| **SKU (base)**                    | `VS-FLASK` |
| **Track quantity**                | ✅ coché   |
| **Continue selling when out of stock** | ❌ décoché |
| **Quantity**                      | sera défini par variante (voir §7) |

---

## 6. Shipping (Expédition)

| Champ                       | Valeur      |
|-----------------------------|-------------|
| **This is a physical product** | ✅ coché |
| **Weight**                  | `0.15 kg`   |
| **Country/region of origin** | `Chine`    |
| **HS code**                 | (à laisser vide pour l'instant) |

---

## 7. Variants — la partie clé

Cliquez sur **"+ Add options like size or color"**.

### Configuration de l'option

| Champ            | Valeur               |
|------------------|----------------------|
| **Option name**  | `Couleur`            |
| **Option values**| `Sky Blue`, `Pink`   |
   *(Tapez chacune et appuyez sur Entrée. Note : le produit réel a une teinte plus turquoise que "sky blue" — si vous préférez, utilisez `Turquoise` à la place de `Sky Blue`.)*

### Détail par variante

Après avoir créé les variantes, cliquez sur "Edit" dans le tableau et remplissez pour chacune :

| Variante     | Price  | Quantity | SKU             | Image à assigner       |
|--------------|--------|----------|-----------------|------------------------|
| **Sky Blue** | 34.90  | 50       | `VS-FLASK-SB`   | `vs-product-teal.jpg`  |
| **Pink**     | 34.90  | 50       | `VS-FLASK-PK`   | `vs-product-pink.jpg`  |

---

## 8. Product organization (panneau de droite)

| Champ            | Valeur                                                |
|------------------|-------------------------------------------------------|
| **Product type** | `Accessoires pour chien`                              |
| **Vendor**       | `VentiSuisse`                                         |
| **Collections**  | (à laisser vide pour l'instant)                       |
| **Tags**         | `chien, gourde, suisse, outdoor, trail, dog, water-bottle` |

---

## 9. Status & Sales channels (panneau de droite)

| Champ            | Valeur                  |
|------------------|-------------------------|
| **Status**       | `Active`                |
| **Sales channels** | ✅ Online Store        |

---

## 10. Search engine listing (référencement, optionnel mais recommandé)

Faites défiler tout en bas de la page :

- **Page title** : `Gourde de trail pour chien — VentiSuisse`
- **Meta description** : `Bouteille isotherme 285 ml avec bol intégré en silicone. Pour les chiens qui suivent partout. Livraison gratuite en Suisse dès CHF 49.`
- **URL handle** : `ventisuisse-gourde-trail` (Shopify le génère automatiquement, vérifiez juste qu'il soit propre)

---

## 11. Enregistrer

Cliquez sur **Save** (en haut à droite).

Après sauvegarde, l'URL affichera l'ID du produit. Copiez-la et envoyez-la dans le chat — je vérifierai que la PDP du storefront affiche correctement toutes les sections (sélecteur de couleur → pack picker → bouton d'achat → onglets repliables → barre ATC mobile).

---

## Récapitulatif rapide

- **Produit** : Gourde de trail VentiSuisse, 285 ml, étanche, avec bol intégré
- **Prix** : CHF 34.90 (TVA 8.1% incluse)
- **Variantes** : 2 couleurs × 50 unités chacune = 100 unités en stock
- **Poids** : 150 g (pour calcul des frais d'expédition)
- **Statut** : Actif, publié sur Online Store
- **Langue principale** : FR (la traduction DE + EN viendra ensuite via l'app Translate & Adapt)
