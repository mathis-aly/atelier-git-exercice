# Exercice — Branches et Pull Request

## Objectif

L'objectif de cet exercice est de réaliser le cycle complet de développement d'une fonctionnalité avec Git et GitHub :

**Créer une branche → Modifier le projet → Commit → Push → Pull Request → Merge → Synchronisation**

Vous disposez d'un projet déjà présent sur GitHub et cloné sur votre machine.

---

## 1. Vérifier votre situation initiale

Vérifiez la branche sur laquelle vous vous trouvez et l'état de votre dépôt.

Vous devez être sur la branche `main` et ne pas avoir de modifications en attente.

Pensez également à récupérer les éventuelles dernières modifications présentes sur le dépôt distant.

---

## 2. Créer une branche

Vous devez ajouter une nouvelle fonctionnalité au projet.

Créez une branche :

`feature/about`

Positionnez-vous sur cette nouvelle branche.

Vérifiez ensuite que vous travaillez bien sur `feature/about`.

---

## 3. Modifier le projet

Créez un fichier :

`about.html`

Ajoutez-y une page HTML simple contenant :

- Un titre « À propos »
- Un paragraphe présentant le projet
- Votre prénom

Enregistrez le fichier.

Vérifiez avec Git que le nouveau fichier est correctement détecté.

---

## 4. Créer un commit

Ajoutez le nouveau fichier à la zone de staging.

Créez ensuite un commit avec un message explicite, par exemple :

`feat: ajout de la page à propos`

Vérifiez que le commit apparaît bien dans l'historique Git.

---

## 5. Publier la branche sur GitHub

Votre branche existe actuellement sur votre dépôt local.

Publiez `feature/about` sur le dépôt distant GitHub.

Vérifiez ensuite sur GitHub que deux branches sont maintenant présentes :

`main`

`feature/about`

La branche `main` ne doit pas encore contenir votre nouvelle page.

---

## 6. Créer une Pull Request

Depuis GitHub, créez une **Pull Request** pour proposer l'intégration de :

`feature/about` → `main`

Donnez un titre explicite à la Pull Request.

Dans sa description, indiquez brièvement la modification réalisée.

Avant de poursuivre, observez les informations fournies par GitHub :

- Les commits concernés
- Les fichiers modifiés
- Les différences entre les deux versions
- La branche source
- La branche cible

---

## 7. Valider et fusionner

Vérifiez le contenu de la Pull Request.

Si les modifications sont correctes, validez la Pull Request puis effectuez le **Merge** dans `main`.

La branche `main` distante contient maintenant votre modification.

Vous pouvez supprimer la branche distante `feature/about` après la fusion.

---

## 8. Mettre à jour votre dépôt local

Attention : votre `main` locale n'a pas été automatiquement mise à jour.

Retournez dans votre terminal.

Revenez sur la branche `main`.

Récupérez les dernières modifications du dépôt distant.

Vérifiez que :

- `about.html` est maintenant présent sur votre branche `main` locale
- Le commit réalisé précédemment apparaît dans l'historique
- Votre dépôt local est synchronisé avec GitHub

---

## Résultat attendu

À la fin de l'exercice :

`feature/about` a été créée localement.

La modification a été commitée sur cette branche.

La branche a été publiée sur GitHub.

Une Pull Request a permis de proposer la modification.

La Pull Request a été vérifiée puis fusionnée dans `main`.

La branche `main` distante contient la modification.

La branche `main` locale a été mise à jour pour récupérer cette modification.

## Question finale

Expliquez pourquoi la modification réalisée sur `feature/about` n'était pas immédiatement présente sur `main`.

Expliquez également pourquoi un `git pull` est nécessaire sur votre `main` locale après avoir réalisé le merge depuis GitHub.