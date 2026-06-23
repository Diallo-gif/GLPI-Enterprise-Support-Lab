# Wi-Fi connecté sans Internet

**Symptôme :**
L'utilisateur est connecté au réseau mais ne parvient pas à accéder à Internet.

**Cause :**
L'étendue DHCP du serveur était désactivée, empêchant l'attribution d'une adresse IP valide au poste client.

**Résolution :**
Diagnostic à l'aide des commandes ipconfig et ping.
Réactivation de l'étendue DHCP sur le serveur, puis renouvellement de l'adresse IP du poste avec `ipconfig /renew`.
Vérification de la connectivité vers la passerelle, Internet (8.8.8.8) et la résolution DNS.

**Outils :**
GLPI, Invite de commandes, DHCP, Windows Server.

**Résultat :**
Adresse IP obtenue correctement et accès Internet rétabli.
