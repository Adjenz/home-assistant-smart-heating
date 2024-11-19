# Configuration Home Assistant - Contrôle de Chauffage Intelligent

Ce projet est une configuration Home Assistant pour un système de chauffage intelligent, optimisé pour une chambre d'enfant. Il combine un radiateur électrique et une vanne thermostatique Netatmo pour un contrôle précis de la température.

## Fonctionnalités

- Contrôle de température précis (18.5°C - 19.5°C)
- Mode Boost temporisé (30 minutes)
- Détection d'ouverture de fenêtre
- Intégration avec Tempo EDF pour l'optimisation des coûts
- Suivi du temps de chauffe quotidien
- Dashboard détaillé avec graphiques de température
- Mode absence avec température réduite (16.5°C)

## Composants

- Radiateur électrique sur prise connectée
- Vanne thermostatique Netatmo
- Capteurs de température
- Intégration Tempo EDF
- Node-RED pour la gestion du mode absence

## Configuration

Le projet inclut :
- Configuration du dashboard (chambre_dashboard.yaml)
- Automatisations pour le compteur de chauffage (chauffage_compteur.yaml)
- Configuration principale (configuration.yaml)
- Autres fichiers de configuration et d'automatisation

## Installation

1. Copiez les fichiers dans votre dossier Home Assistant
2. Ajoutez les intégrations nécessaires (HACS, Mushroom, ApexCharts)
3. Redémarrez Home Assistant
4. Accédez au dashboard "Chambre - Contrôle Température"

## Dépendances

- Home Assistant
- HACS
- Mushroom Cards
- ApexCharts Card

## Fonctionnement

### Gestion de la Température
- La vanne Netatmo est réglée à 19°C pour le contrôle principal
- Le radiateur électrique sert de boost quand nécessaire
- Mode absence réglé à 16.5°C pour économiser l'énergie

### Optimisation Énergétique
- Intégration avec Tempo EDF pour la gestion des coûts
- Compteur de temps de chauffe quotidien
- Estimation de la consommation

### Sécurité
- Détection d'ouverture de fenêtre
- Mode boost limité à 30 minutes
- Température maintenue dans une plage sécurisée
