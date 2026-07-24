# 🚴 Carnet vélo — suivi entraînement & nutrition

Petite web app personnelle de suivi quotidien pour cycliste : charge d'entraînement, récupération et nutrition, le tout en un seul fichier HTML, sans compte ni serveur.

## Fonctionnalités

- **Journée** : check-in du réveil (FC repos, poids, sommeil), repas ajoutés au fil de la journée avec estimation automatique des calories et macros (protéines / glucides / lipides), saisie de la sortie vélo.
- **Calcul de la dépense** à partir de la puissance : `kcal ≈ watts moyens × heures × 3,6` (équivalence kJ ≈ kcal), affichée sur un écran façon compteur, avec balance mangé − dépensé.
- **Historique** : fiche récapitulative par journée, modifiable d'un tap.
- **Tendances** : courbes (poids, FC réveil, sommeil, dépense, apports, macros, balance) et charge d'entraînement en kJ/jour, agrandissables en grand graphique interactif.
- **Bilan** : moyennes par période (tout / 7 / 14 / 30 jours) et texte récapitulatif à copier pour un rendez-vous nutrition.

## Installation (iPhone)

1. Héberger `index.html` et `icon.png` (GitHub Pages : Settings → Pages → branche `main`).
2. Ouvrir l'adresse dans **Safari** → Partager → **Sur l'écran d'accueil**.
3. Toujours ouvrir l'app depuis cette icône.

## Données & sauvegardes

- Les données restent **sur l'appareil** (localStorage du navigateur), rien n'est envoyé en ligne.
- ⚠️ Supprimer l'icône de l'écran d'accueil efface les données locales.
- Onglet **Bilan → Télécharger une sauvegarde** : export JSON complet, à conserver (iCloud). Restauration via **Restaurer une sauvegarde**.

## Avertissement

Les calories et macros sont des **estimations** indicatives, pas des mesures médicales. La dépense de base (kcal/j hors vélo) est un paramètre réglable dans l'onglet Bilan.
