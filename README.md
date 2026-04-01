# Oracle des Trois Arcanes
### *Compositeur oraculaire — Tarot de Marseille · Jeu Camoin-Jodorowsky*

> *« Le Bateleur transmute les éléments sur la table. »*

Un outil oraculaire interactif basé sur le Tarot de Marseille (jeu Camoin-Jodorowsky), conçu autour d'une mécanique syntaxique originale : chaque carte contribue un **fragment de phrase** selon sa position, et l'assemblage des trois fragments produit une sentence oraculaire unique.

---

## Concept

L'oracle repose sur une grammaire à trois positions, inspirée de la structure sujet–complément–circonstance :

| Position | Rôle grammatical | Exemple (Le Bateleur) |
|----------|-----------------|----------------------|
| **I — Sujet agissant** | Le verbe et son sujet | *Le Bateleur transmute* |
| **II — Objet en jeu** | Le complément d'objet | *les éléments* |
| **III — Lieu & manière** | Le complément circonstanciel | *sur la table* |

Chaque arcane possède **trois fragments distincts**, un par position. Le tirage de trois cartes (une par position) produit une phrase syntaxiquement cohérente parmi **78³ = 474 552 combinaisons possibles** pour le jeu complet.

Les fragments ont été composés par **Arnauld de Beaugency**, pseudonyme littéraire de l'auteur, selon une logique ésotérique propre — chaque mot choisi porte un poids symbolique lié à la tradition du tarot, à la Kabbale, et à la pensée hermétique.

---

## Fichiers

| Fichier | Description |
|---------|-------------|
| `tarot.html` | Oracle 22 Arcanes Majeurs — tirage aléatoire — fragments pos1/pos2/pos3 |
| `tarot-selector.html` | Oracle 22 Majeurs — **sélection manuelle** des trois cartes |
| `tarot-78.html` | Oracle 78 cartes — tirage aléatoire — Majeurs + 4 familles |
| `tarot-78-img.html` | Oracle 78 cartes — tirage aléatoire — **avec illustrations** |
| `tarot-selector-78.html` | Oracle 78 cartes — **sélection manuelle** — filtre par famille |
| `tarot-v1.html` | Variante Passé / Présent / Futur — 22 Majeurs |
| `tarot-v1-78.html` | Variante Passé / Présent / Futur — 78 cartes |
| `tarot-v1-78-img.html` | Variante Passé / Présent / Futur — 78 cartes — **avec illustrations** |

Tous les fichiers sont **autonomes** (standalone HTML) : aucune dépendance externe, aucun serveur requis. Les images sont encodées en base64 directement dans le HTML.

---

## Deux logiques de tirage

### Logique A — Sujet · Objet · Circonstance
*(fichiers `tarot.html`, `tarot-78.html`, `tarot-selector-78.html`)*

Chaque carte exprime un fragment syntaxique selon sa position fixe. Le résultat est une phrase au présent, immédiate, intemporelle.

**Exemple :**
> *La Tempérance transvase · l'âme · du nectar de vie.*

### Logique B — Passé · Présent · Futur
*(fichiers `tarot-v1.html`, `tarot-v1-78.html`, `tarot-v1-78-img.html`)*

Chaque carte exprime un fragment narratif conjugué selon sa position temporelle. Le résultat est une phrase qui raconte un arc dans le temps.

**Exemple :**
> *Un équilibre patient forgea la sagesse du temps, et aujourd'hui le flux circule doucement en cherchant l'harmonie — car demain, la juste mesure retrouvée apportera la sérénité.*

---

## Les familles des Arcanes Mineurs

Les 56 arcanes mineurs sont répartis en quatre familles, chacune dotée de ses propres fragments :

| Famille | Symbole | Registre symbolique |
|---------|---------|-------------------|
| **Bâtons** | 🪵 | Feu · action · émanation · volonté |
| **Deniers** | 🪙 | Terre · matière · pouvoir · intériorité |
| **Épées** | ⚔️ | Air · intellect · dialectique · gnose |
| **Coupes** | 🏆 | Eau · amour · mutation · communion |

---

## Illustrations

Les illustrations utilisées sont issues du **Tarot de Marseille Camoin-Jodorowsky** (© Jodo Camoin), restauré et publié par Philippe Camoin et Alejandro Jodorowsky à partir de 1997. Ce jeu est considéré comme l'une des reconstructions les plus rigoureuses du tarot de Marseille originel.

> Les images sont intégrées à titre de documentation culturelle et d'outil d'étude ésotérique non commercial, dans le respect de la tradition tarotique.

---

## Utilisation

### En local
Télécharger le fichier HTML souhaité et l'ouvrir dans un navigateur. Aucune installation, aucun serveur.

### Sur GitHub Pages
1. Forker ce dépôt
2. Activer GitHub Pages dans les paramètres du dépôt (`Settings > Pages > Branch: main`)
3. Les fichiers sont accessibles à `https://[votre-nom].github.io/[nom-du-repo]/`

---

## Structure du code

Chaque fichier HTML suit la même architecture :

```
CARD_IMG { }          // Dictionnaire nom → base64 (fichiers avec images)
ARCANES [ ]           // Tableau des 22 ou 78 cartes avec pos1/pos2/pos3
drawCards()           // Tirage aléatoire sans remise
flipCard(i)           // Animation de retournement 3D
showInterpretation()  // Assemblage et affichage de la phrase
resetReading()        // Réinitialisation
```

Les données sont entièrement séparées de la logique d'affichage : il est aisé de modifier les fragments textuels sans toucher au code JavaScript.

---

## Auteur

**Arnauld de Beaugency** — pseudonyme littéraire
Auteur de *La Trilogie de Keranna* (mythologie celtique, gnose, compagnonnage)
Beaugency, Loiret, France

Intérêts : Kabbale · Tarot · I Ching · Cinema · Ésotérisme occidental · Littérature mythologique

---

## Licence

Ce projet est publié sous licence **MIT**.

Les fragments textuels (pos1, pos2, pos3) sont une œuvre originale de l'auteur.
Les illustrations du Tarot Camoin-Jodorowsky restent la propriété de leurs ayants droit.

```
MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software to deal in the Software without restriction, including the
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
sell copies of the Software.
```

---

## Contribuer

Les contributions sont bienvenues :
- Traductions des fragments dans d'autres langues
- Nouvelles logiques de tirage (croix celtique, arbre séphirotique…)
- Intégration d'autres jeux de tarot (Rider-Waite, Thoth…)
- Amélioration de l'interface et de l'expérience utilisateur

Ouvrir une *issue* ou proposer une *pull request*.

---

*« Le Monde se façonne par le refreinement de nombreux désirs. »*
