# 🔐 Projet Atelier — Escape Game JPO

> Jeu d'évasion numérique pour la Journée Portes Ouvertes  
> Lycée Jean Jaurès, Argenteuil · Janvier 2026

[![HTML](https://img.shields.io/badge/HTML-JS-E34F26?style=flat&logo=html5)](https://developer.mozilla.org/fr/docs/Web/HTML)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-7952B3?style=flat&logo=bootstrap)](https://getbootstrap.com)

---

## 📋 Description

Escape game web créé pour la JPO du Lycée Jean Jaurès (session orientation secondes, janvier 2026). Les joueurs (élèves de seconde en visite) devaient résoudre une série d'énigmes pour "récupérer le trésor" et gagner des jetons récompense.

Le jeu mettait en scène un scénario de récupération de données via une caméra IP sécurisée, avec une énigme de chiffrement César comme verrou central.

---

## 🎮 Déroulement du jeu

1. **Introduction** : Les joueurs confirment faire partie de l'équipe de récupération
2. **Énigme César** : Un mot chiffré (`SURFHVVXHU`) doit être déchiffré (décalage de 3 → `PROCESSEUR`)
3. **Accès caméra** : Identifiants de l'interface web fournis après succès (sanitisés dans cette version)
4. **Code final** : Code affiché par la caméra à saisir (`COFFREMAGIQUE`)
5. **Récompense** : Les joueurs gagnent leurs jetons (60 de départ, −10 par mauvaise tentative)

---

## 🏗️ Structure

```
projet-atelier-jpo/
│
├── site/
│   ├── CoffreCaméra.html     # Interface web du jeu (HTML + JS vanilla)
│   └── bg.jpeg               # Image de fond
│
├── documents/
│   ├── utiles/               # Documents clés mis à disposition des joueurs
│   │   ├── Alphabet.jpg      # Alphabet de référence pour le chiffrement
│   │   ├── cesar3.pdf        # Explication du chiffre de César (décalage 3)
│   │   ├── TUTO ANGRY IP SCANNER.docx   # Tuto pour trouver l'IP de la caméra
│   │   └── Mail d'achat HIKVISION.docx  # Fausse piste → marque de la caméra
│   │
│   └── inutiles/             # Leurres pour perdre du temps
│       ├── Document inutile 1.pdf
│       └── Document inutile 2.pdf
│
└── VIDEO_NOTE.txt            # Note sur la vidéo d'introduction (IA, non incluse)
```

---

## ⚙️ Technologies

| Composant | Technologie |
|-----------|-------------|
| Interface | HTML5 / JS vanilla |
| Style | Bootstrap 5.3 |
| Chiffrement | César (décalage 3) — implémenté côté JS |
| Vidéo intro | Générée par IA |
| Matériel réel | Caméra IP HIKVISION du réseau du lycée |

---

## 🔒 Note de sécurité

Le mot de passe réel de l'interface caméra a été remplacé par `MOT_DE_PASSE_CAMERA` dans le fichier HTML publié. Le jeu a été utilisé uniquement sur le réseau interne du lycée le jour de la JPO.

---

## 🎓 Contexte

Projet réalisé en autonomie dans le cadre de l'**Atelier JPO** — animation de l'espace BTS CIEL lors de la journée portes ouvertes du Lycée Jean Jaurès. Objectif : présenter le domaine informatique/réseau aux élèves de seconde de manière ludique et interactive.

---

## 👤 Auteur

**Paurtheiv Krishna Laxman**  
BTS CIEL A — Lycée Jean Jaurès, Argenteuil (95)

📧 paurtheiv.laxman.fr@gmail.com  
🔗 [Portfolio](https://paurtheiv.github.io)
