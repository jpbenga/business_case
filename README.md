# Parasol

Ceci est ce qu'on appel chez Human Booster un projet fil-rouge. Ce projet à pour but de couvrir l'ensemble des modules abordés tout au long de la formation au cas où le stage de fin d'année ne permet de couvrir l'ensemble des CCP pour valider le diplôlme.
Ce projet à pour but de réaliser un site de réservation de parasol, en suivant un cahier des charges précis.

## Table des matières

- [Description](#description)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Structure du projet](#structure-du-projet)
- [Contributions](#contributions)
- [Licence](#licence)

## Description

Les plages italiennes sont découpées en concessions privées. Chaque concession est divisée en plusieurs files. Un ensemble de parasols est aligné au cordeau sur chaque file. L'emplacement des parasols est fixe.
La concession contient 8 files, chaque file contient 36 parasols. La concession possède une allée centrale pour faciliter l'accès aux parasols.
La première file est la plus proche de la mer.
Un parasol est identifié par son numéro de file et par un numéro dans la file, exemple: 15F4, représenté sur la matrice de la page 1 par un X.
Chaque année la saison estivale débute le 01 Juin et se termine le 15 Septembre.
Dans le cadre d’une réservation, un client peut louer un ou plusieurs parasols aux mêmes dates.
Il n’est pas possible de louer un parasol pour quelques heures ou une demi-journée. Un parasol est loué pour une durée minimale d’une journée.
Sous chaque parasol, il faut louer au choix :
 unlit
 deux lits
 un fauteuil de réalisateur
 un fauteuil de réalisateur et un lit
 deux fauteuils de réalisateur
Sur chaque équipement placé sous un parasol, on écrit le numéro du parasol.
Le montant de la location est fonction :
 du nombre de jours de location
 du nombre d'années de location du client concerné
 de la proximité avec la mer
 du lien de parenté avec le gérant de la concession (exemples : 50 % de réduction pour les
frères et sœurs du concessionnaire, 25 % de réduction pour les cousins et cousines du concessionnaire).

Pour le concessionnaire, il est nécessaire de pouvoir :
 s’authentifier en précisant son email et son mot de passe
 voir le planning (présentant l’occupation des parasols, cette feature est la plus complexe du
business case, dans l’idéal le planning pourra afficher l’occupation sur un jour, un semaine,
un mois ou sur une période choisie par le concessionnaire)
 voir les réservations
 voir le détail d’une réservation
 voir les réservations à traiter
 traiter une réservation : soit en validant la réservation soit en refusant la réservation. Le
refus d’une réservation inclut un paiement vers la sandbox de Paypal d’un montant égal à
celui réglé par le client au moment de la réservation
 modifier les parasols alloués à une réservation (cette feature peut utiliser un système de
glisser-déposer sur le planning)
 voir les clients (avec une possibilité de filtrer les clients par pays de résidence et/ou de les
trier par date d’inscription)
 supprimer un client (uniquement si aucune de ses réservations n’a déjà été validée)
 se déconnecter

Pour un client de la concession, il est nécessaire de pouvoir :
 s’inscrire (en précisant son nom, son prénom, son email, son pays de résidence et un mot de
passe contenant au minimum 8 caractères)
 s’authentifier en précisant son email et son mot de passe
 voir ses réservations (en attente de traitement, acceptées et refusées)
 ajouter une réservation (cette feature inclut un paiement vers la sandbox de Paypal)
 modifier ses informations
 se déconnecter

## Installation

Les étapes requises pour installer et configurer le projet localement. Incluez les dépendances, les prérequis système et toute autre information pertinente.

```bash
Exemple de commandes à exécuter pour l'installation
