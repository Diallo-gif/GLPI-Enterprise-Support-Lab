# Impossible de modifier le fond d'écran du bureau

**Symptôme :**
L'utilisateur ne peut pas changer son arrière-plan de bureau.

**Cause :**
Une stratégie de groupe de personnalisation empêchait la modification du fond d'écran.

**Résolution :**
Vérification de la GPO "Ma-GPO", ajout du groupe RH au filtrage de sécurité puis modification des paramètres de personnalisation afin d'autoriser le changement de l'arrière-plan du bureau.

**Outils :**
GPMC, Active Directory, Windows Server.

**Résultat :**
L'utilisateur a retrouvé la possibilité de modifier son fond d'écran et a confirmé le retour à la normale.
