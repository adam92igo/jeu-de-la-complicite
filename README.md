# 🎯 Jeu de la Complicité

Un jeu de société pour soirées entre amis, jouable directement dans le navigateur — sans installation, sans compte, sans backend.

**→ [Jouer maintenant](https://jeu-de-la-complicite.vercel.app)**

---

## C'est quoi ?

Le jeu de la complicité se joue en équipes de 2. Un joueur doit faire deviner un mot à son partenaire uniquement via des anecdotes et expériences communes — pas d'indices classiques, juste la complicité.

Les autres équipes écoutent et peuvent **voler le point** si elles devinent avant.

## Règles

1. Créer les équipes (minimum 2, pas de maximum)
2. À chaque tour, une équipe est active — l'un de ses joueurs fait deviner le mot à l'autre
3. **+1 point** à l'équipe active si son partenaire devine
4. **+1 point** à une autre équipe si elle devine avant
5. Pas de timer, pas de contraintes — juste la complicité
6. Possibilité de passer un mot qui ne vous parle pas

## Les mots

**2208 mots** répartis dans 40+ catégories :

| Catégorie | Mots |
|---|---|
| Films | 158 |
| Argot & expressions | 131 |
| Musique actuelle | 123 |
| Marques | 121 |
| Mèmes & pop culture | 96 |
| Séries | 92 |
| Personnages | 92 |
| Animaux | 89 |
| Musique | 85 |
| Géographie | 85 |
| … et bien d'autres | — |


## Stack

- HTML / CSS / JS vanilla — zéro dépendance, zéro framework
- Fichier unique `index.html`
- Hébergé sur [Vercel](https://vercel.com)

## Lancer en local

```bash
git clone https://github.com/TON-USERNAME/complicite-jeu.git
cd complicite-jeu
open index.html   # ou double-clic sur le fichier
```

Aucune installation requise.

## Ajouter des mots

Les mots sont dans le tableau `WORDS` dans `index.html`, au format :

```js
{ m: "Nom du mot", c: "Catégorie" }
```

Exemple :

```js
{ m: "Barbenheimer", c: "Film récent" },
{ m: "Rizz", c: "Mèmes" },
{ m: "Capybara", c: "Animaux" },
```

## Déploiement

Le projet est connecté à Vercel — chaque `git push` sur `main` redéploie automatiquement.

```bash
git add index.html
git commit -m "description des changements"
git push
```

## Contribuer

Tu veux ajouter des mots, corriger une catégorie ou suggérer une feature ?  
Ouvre une [issue](../../issues) ou une [pull request](../../pulls), c'est ouvert.

## Licence

MIT — fais-en ce que tu veux.
