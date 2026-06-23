# VPN inaccessible

**Symptôme :**
L'utilisateur en télétravail ne parvient plus à se connecter au VPN de l'entreprise.

**Cause :**
L'accès distant était refusé dans les propriétés du compte Active Directory.

**Résolution :**
Vérification des paramètres VPN puis modification des autorisations d'accès distant dans Active Directory afin d'autoriser la connexion VPN.

**Outils :**
GLPI, Active Directory Users and Computers (ADUC), RRAS, Windows 10.

**Résultat :**
Connexion VPN rétablie et accès aux ressources de l'entreprise restauré.
