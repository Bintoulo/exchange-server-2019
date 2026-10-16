# Installation et configuration de Microsoft Exchange Server 2019 sur Windows Server 2019

Projet de laboratoire réalisé à l'Institut Supérieur d'Informatique (ISI), année académique 2024-2025.

## Description
Déploiement d'un serveur de messagerie d'entreprise Microsoft Exchange 2019 (Mise à jour cumulative 14) dans un domaine Active Directory (`bilo.sn`), avec création de boîtes aux lettres et test d'envoi de courriels via le webmail.

## Environnement
- Windows Server 2019 (machine virtuelle, 2 cartes réseau : réseau interne + NAT pour Internet)
- Services préexistants : AD DS et DNS
- Ressources recommandées : 8 Go de RAM, 100 Go de disque

## Étapes réalisées
1. Installation des prérequis : .NET Framework 4.8, Visual C++ 2013 Redistributable (x86 et x64), UCMA 4.0 Runtime, module URL Rewrite pour IIS
2. Installation des composants Windows Server et IIS avec `Install-WindowsFeature` (PowerShell)
3. Mise à jour du système et redémarrage
4. Installation d'Exchange 2019 CU14 depuis l'ISO (`setup.exe` en administrateur)
5. Connexion au Centre d'administration Exchange (`/ecp`)
6. Création de deux utilisateurs dans une unité d'organisation Active Directory, puis création des boîtes aux lettres associées
7. Test : connexion à Outlook Web App (`/owa`) et envoi d'un message entre deux utilisateurs

## Compétences mises en œuvre
Windows Server, Active Directory, Exchange Server, IIS, PowerShell, messagerie d'entreprise

## Contenu du dépôt
- `docs/RAPPORT_MICROSOFT_EXCHANGE.pdf` : rapport complet avec captures d'écran

## Auteur
Bintou LO
