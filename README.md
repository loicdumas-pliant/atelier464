# Atelier 464

Site vitrine d'Atelier 464 — espace de design cambodgien contemporain,
31b Street 464, Tuol Tom Poung, Phnom Penh.

Marques : Kingdom of Wow · Maison Sirivan · Morowood · Tamara Venn.

## Structure

- `index.html` — page d'accueil
- `kingdom-of-wow/`, `maison-sirivan/`, `morowood/`, `tamara-venn/` — une page détaillée par marque (`index.html`)
- `css/style.css` — toute la mise en forme et les animations (CSS seul, sans JavaScript)
- `img/<marque>/` — un dossier d'images par marque (`atelier464`, `kingdom-of-wow`, `maison-sirivan`, `morowood`, `tamara-venn`) ; les photos des pages marques sont dans `img/<marque>/gallery/`
- `fonts/` — Josefin Sans et Inter (licence SIL OFL)

## Mise à jour

Après une modification du CSS, incrémenter `?v=` dans le lien `css/style.css?v=…` de `index.html`
pour que les navigateurs rechargent la feuille de style.

## Pages de campagne (`promo/`)

Pages courtes liées à une action précise (flyer, QR code, publicité, soldes).
Elles ne sont pas dans le menu du site : on y accède par leur lien direct.

| Dossier | Adresse en ligne | Usage |
|---|---|---|
| `promo/_template/` | — | Modèle à copier (non indexé par Google) |
| `promo/follow-us/` | `…/atelier464/promo/follow-us/` | Carte QR « Join our community » : Instagram, Facebook, avis Google |
| `promo/espadrilles-sale/` | `…/atelier464/promo/espadrilles-sale/` | Exemple d'après le flyer « Wild Sale » (non indexé) |

Créer une nouvelle campagne :
1. Copier `promo/_template/` et renommer le dossier (minuscules, tirets : `fete-des-meres`).
2. Remplacer chaque texte entre `[CROCHETS]` et les images.
3. Garder `<meta name="robots" content="noindex">` pour une offre limitée dans le temps ; le retirer pour une page permanente.
4. Générer le QR code vers l'adresse de la page.
5. Quand l'offre est terminée : supprimer le dossier, ou rediriger le texte vers « Offer ended — visit us ».
