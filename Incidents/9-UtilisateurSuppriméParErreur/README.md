# Utilisateur supprimé par erreur

## Symptôme

Au cours de mes manipulations dans Active Directory, j'ai supprimé par erreur l'utilisateur **Marion**.

À ce moment-là :

- aucune sauvegarde d'Active Directory n'avait été réalisée ;
- la fonctionnalité **Corbeille Active Directory (AD Recycle Bin)** n'avait pas encore été activée.

Par conséquent, l'utilisateur a été perdu définitivement et n'a pas pu être restauré.

## Cause

L'absence de sauvegarde et l'absence d'activation de la Corbeille Active Directory empêchaient toute restauration d'un objet supprimé.

## Résolution

Afin d'éviter que cette situation ne se reproduise :

1. Activation de la fonctionnalité **Active Directory Recycle Bin** à l'aide de PowerShell.
2. Vérification de l'activation de la fonctionnalité.
3. Suppression d'un utilisateur de test (**Aissatou**) afin de valider le fonctionnement de la Corbeille Active Directory.
4. Vérification de la présence de l'utilisateur dans le conteneur **Deleted Objects**.
5. Restauration de l'utilisateur supprimé.
6. Contrôle de son retour dans son unité d'organisation d'origine.

## Outils

- Active Directory Users and Computers (ADUC)
- Active Directory Administrative Center
- Windows PowerShell

## Résultat

La perte définitive de Marion a permis de comprendre l'importance :

- des sauvegardes Active Directory ;
- de l'activation préalable de la Corbeille Active Directory ;
- des tests de restauration avant un incident réel.

Après activation de la Corbeille AD, un utilisateur supprimé peut désormais être restauré sans avoir recours à une sauvegarde complète.
