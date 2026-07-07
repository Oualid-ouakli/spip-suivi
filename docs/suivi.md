---
title: Suivi du projet
---

<style>
    @media screen and (min-width: 76em) {
        .md-sidebar--primary {
            display: none !important;
        }
    }
</style>

# Suivi de projet

> :bulb: Cette page documente l’évolution du projet dans le temps.
> Elle sert à rendre visibles les décisions, ajustements et apprentissages.
> Les entrées peuvent être hebdomadaires ou bi-hebdomadaires.  
> N'oubliez pas d’effacer ou de mettre en commentaires les notes (`>`) avant la remise finale.

---


## Semaines récentes — Interface, backend et précision

### Objectifs de la période
- Refaire l'interface de l'application selon les maquettes
- Mettre en place le partage de parcours entre utilisateurs
- Améliorer la précision de la navigation

### Travail réalisé
!!! abstract "Avancement"
    - [x] Refonte complète des 6 écrans selon les maquettes (style Mapbox/Figma)
    - [x] Suivi multi-étages avec vibration et pop-up de transition
    - [x] Nommage et catégorisation des parcours (bâtiment + catégorie)
    - [x] Backend : API REST (Node.js + Express)
        - Migration vers PostgreSQL
        - Déploiement en ligne sur Render
    - [x] Cycle participatif complet : publier, télécharger et suivre un parcours partagé
    - [x] Calibration guidée de la foulée par utilisateur
    - [x] Recalage de la position sur des repères connus (correction de la dérive)
    - [x] Filtre des parcours partagés par bâtiment
    - [x] Graphe du profil des étages pendant le suivi

### Décisions et ajustements
!!! info "Décisions"
    - Base de données : abandon de better-sqlite3 (incompatible Windows/Node 24), puis choix de PostgreSQL pour la production
    - Localisation des parcours par bâtiment plutôt que par GPS, pour rester cohérent avec le principe de navigation sans GPS
    - Calibration de la foulée par distance marchée (validée avec le superviseur)

### Difficultés rencontrées
!!! warning "Difficultés"
    - Installation de better-sqlite3 impossible sur Windows (nécessitait des outils de compilation C++) : résolu en changeant de base de données
    - Tunnel Expo (ngrok) instable au démarrage : contourné en relançant ou en passant en mode local
    - Gestion de la proximité sans GPS : résolu en regroupant les parcours par bâtiment

## Semaine 1 (12–18 janvier)

### Objectifs de la période
- Clarifier la problématique
- Explorer les solutions existantes
- Produire un premier prototype conceptuel

### Travail réalisé

!!! abstract "Avancement"
    - [x] Analyse de solutions existantes
        - Comparaison de trois outils similaires
    - [x] Prototype basse fidélité (Figma)
    - [ ] Validation utilisateur
        - Reportée à la semaine suivante

### Décisions et ajustements

> À compléter uniquement si des choix structurants ont été faits
> ou si l’orientation du projet a évolué.

!!! info "Décisions"
    - Abandon de l’approche X jugée trop complexe
    - Reformulation de la problématique suite aux premières analyses

### Difficultés rencontrées

> À compléter uniquement si des obstacles ont eu un impact réel
> sur l’avancement du projet.

!!! warning "Difficultés"
    - Problème de configuration du plugin Mermaid
        - Confusion entre `mkdocs-mermaid2-plugin` (pip)
          et `mermaid2` (nom du plugin)
        - Résolu après nettoyage et configuration correcte dans `mkdocs.yml`
