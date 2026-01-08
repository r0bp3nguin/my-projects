# FCI Comparator

## Description

Application web de comparaison d'images de matériaux développée pour un contexte B2B permettant de trouver des matériaux similaires parmi une base de données de fournisseurs. Le système utilise l'intelligence artificielle et l'analyse de couleurs pour identifier les meilleures correspondances.

## Projet

Projet développé en équipe de 2 personnes, dans lequel je me suis particulièrement intéressé au déploiement Docker et à l'infrastructure de containerisation.

 
## Architecture technique

Application développée avec un backend Python et un frontend React/TypeScript.

### Infrastructure et déploiement Docker

- **Containerisation** : Docker avec support multi-architecture (amd64/arm64)
- **Orchestration** : Docker Compose pour la gestion des services
- **Build multi-architecture** : Scripts de build permettant de créer des images pour différentes architectures

#### Déploiement chez le client

L'application a été déployée en production chez le client sur un serveur Linux dédié. Le déploiement s'est effectué via Docker, permettant une installation simple et reproductible :

- **Environnement de production** : Serveur Linux avec Docker et Docker Compose
- **Déploiement containerisé** : Backend et frontend déployés dans des conteneurs Docker isolés
- **Gestion des données** : Volumes Docker pour la persistance des données et du cache
- **Configuration** : Variables d'environnement pour la configuration spécifique au client
- **Maintenance** : Mise à jour simplifiée via pull des nouvelles images Docker

Cette approche containerisée facilite le déploiement, la maintenance et la mise à jour de l'application en environnement client, tout en garantissant la reproductibilité et l'isolation des services.
