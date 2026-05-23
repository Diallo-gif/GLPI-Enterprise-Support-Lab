# Documentation d’infrastructure

## Objectif
Simulation d’un environnement Helpdesk entreprise avec GLPI et Windows Server afin de reproduire des incidents Support IT N1/N2 réalistes.

---

## Infrastructure

| Machine | Rôle |
|---|---|
| DC-ALPHA | AD DS, DNS, DHCP |
| SERVER-GLPI | GLPI, Apache, MariaDB |
| CLIENT02 | Poste utilisateur |

---

## Technologies utilisées

- Windows Server 2019
- Active Directory
- DNS
- DHCP
- GPO
- GLPI
- Apache (XAMPP)
- MariaDB
- VirtualBox

---

## Fonctionnement

1. L’utilisateur accède à GLPI depuis sa VM cliente
2. Il crée un ticket
3. Le serveur GLPI reçoit la demande
4. Le technicien analyse et résout l’incident

---

## Adresse GLPI Saisi sur le post client pour accéder à l'interface GLPI

```text
http://192.168.56.50:80/glpi
```
(Il faut savoir que: cette Ip correspond à l'adresse Ip du serveur DC-ALPHA
