---
title: Vue d'ensemble du projet
---

<style>
    @media screen and (min-width: 76em) {
        .md-sidebar--primary {
            display: none !important;
        }
    }
</style>

# Vue d'ensemble du projet

!!! info "Informations générales"
    **Session**: Été 2026  
    **Auteur(s)**: Oualid Ouakli  
    **Thème(s)**: Navigation intérieure, cartographie participative, développement mobile  
    **Superviseur(s)**: Louis-Édouard Lafontant (DIRO, Université de Montréal)  
    **Collaborateur(s):** Aucun (projet solo)

# Spip — Cartographie progressive et guidage personnalisé par la marche

## Description du projet

### Contexte

L'orientation dans des environnements complexes (bâtiments universitaires, hôpitaux, centres commerciaux) demeure difficile, particulièrement en l'absence de systèmes de navigation intérieurs adaptés. Les outils de cartographie actuels ne permettent pas de représenter de manière simple et progressive un espace tel qu'il est vécu et parcouru par un individu.

### Problématique

Les solutions existantes de navigation intérieure reposent sur des cartes statiques ou des infrastructures coûteuses (balises Bluetooth, calibration Wi-Fi). Elles ne reflètent pas l'expérience réelle de déplacement des usagers et demandent un investissement important de la part des gestionnaires de bâtiments. Il manque une approche légère et participative qui s'appuie directement sur les trajets des utilisateurs.

### Proposition et objectifs

Spip est une application mobile qui permet de **construire une carte en marchant** et de **laisser un parcours à suivre** dans des environnements complexes. L'application adopte une approche participative où les utilisateurs contribuent eux-mêmes aux données de navigation.

Objectifs :
- Permettre à un utilisateur de cartographier un trajet intérieur en temps réel via l'application
- Permettre de suivre un parcours existant créé par un autre utilisateur
- Développer une API REST pour la gestion des données de navigation
- Valider le prototype dans au moins un bâtiment réel (ex. pavillon de l'UdeM)

### Méthodologie

Le projet suit une approche itérative :
1. Conception des maquettes UI (Figma)
2. Développement du backend (Node.js, PostgreSQL)
3. Développement de l'application mobile (React Native + Expo)
4. Tests et validation avec un bâtiment pilote
5. Ajustements selon les retours

### Validation et Évaluation

- Tests fonctionnels sur l'enregistrement et le suivi de parcours
- Test utilisateur dans un pavillon de l'UdeM pour évaluer la facilité d'utilisation
- Comparaison entre les parcours enregistrés et les trajets réels

### Équipe

| Membre | Rôle |
|--------|------|
| Oualid Ouakli | Développeur unique (fullstack) |

**Superviseur** : Louis-Édouard Lafontant (louis.edouard.lafontant@umontreal.ca)

## Échéancier

!!! info
    Le suivi complet est disponible dans la page [Suivi de projet](suivi.md).

| Activités                      | Début   |   Fin   | Livrable                            | Statut      |
|--------------------------------|---------|---------|-------------------------------------|-------------|
| Ouverture de projet            | 4 mai   | 15 mai  | Proposition de projet               | ✅ Terminé  |
| Études préliminaires           | 4 mai   | 22 mai  | Document d'analyse                  | 🔄 En cours |
| Présentation + Rapport         | 7 aout  | 14 aout | Présentation + Rapport              | ⏳ À venir  |
