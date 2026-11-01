# Atelier 3 : Gestion des paquetages et des processus

**Réalisé par :** NAIT HADDOU MALAK

**Environnement :** Ubuntu Server (Machine Virtuelle)  

**Date :** Novembre 2026

## 📝 Description du projet
Ce dépôt contient le rapport complet et les manipulations effectuées lors de l'Atelier 3. L'objectif de ce TP était de maîtriser deux aspects fondamentaux du système d'exploitation Linux :
1. **La gestion des processus** : contrôle, hiérarchie, priorités et signaux.
2. **La gestion des paquetages** : installation et maintenance via `dpkg` et le système `APT`.

## 📂 Contenu du dépôt
*   `rapport_tp.pdf` (ou `.tex`) : Le rapport complet détaillant les réponses, les commandes exécutées et les observations.
*   `README.md` : Ce fichier descriptif.

## 🛠️ Résumé des manipulations (Partie 1 : Processus)
*   **Observation :** Utilisation de `ps`, `pstree` et `top` pour visualiser la hiérarchie (relations parent/enfant).
*   **Contrôle :** Utilisation des signaux `SIGTERM` (15) pour un arrêt propre et `SIGKILL` (9) pour un arrêt forcé.
*   **Priorités :** Modification de la priorité (valeur *nice*) avec `nice` (au lancement) et `renice` (en cours d'exécution).
*   **Jobs :** Gestion des tâches en arrière-plan avec `Ctrl+Z`, `bg`, `fg` et `jobs`.
*   **Persistance :** Utilisation de `nohup` pour détacher un processus du terminal et le faire survivre à sa fermeture.

## 📦 Résumé des manipulations (Partie 2 : Paquetages)
*   **Bas niveau (`dpkg`) :** Installation manuelle d'un paquet `.deb` (`ttf-mscorefonts-installer`). Mise en évidence de l'incapacité de `dpkg` à gérer les dépendances (résolu avec `apt-get -f install`).
*   **Haut niveau (`APT`) :** Recherche, installation et suppression de paquets (`zsh`) avec gestion automatique des dépendances.
*   **Maintenance :** Nettoyage du cache système avec `apt-get clean` pour libérer de l'espace disque.

