# Personal Security & Cloud Lab - Infrastructure Hybride 🏠🔒

## 🎯 Présentation
Ce dépôt documente mon laboratoire personnel (Homelab), conçu pour expérimenter des architectures de haute disponibilité, de virtualisation avancée et de sécurité périmétrique stricte.

## 🚀 Stack Technique & Architecture
* **Virtualisation (Proxmox VE) :** * Cluster de 2 nœuds Proxmox (Haute Disponibilité en cours de déploiement).
    * Gestion centralisée via **Proxmox Datacenter Manager** pour le monitoring unifié.
* **Sécurité Périmétrique (Stormshield SNS) :**
    * Filtrage granulaire et inspection protocolaire.
    * **Hardening des accès :** Restriction géographique (France uniquement) sur les flux entrants.
* **Accès Distant Sécurisé :**
    * Mise en place d'un **VPN SSL** avec redirection de port (PAT) sur IP publique.
    * **Politique Zero Trust :** Accès VPN restreint exclusivement à l'IP publique de mon entreprise d'alternance pour une administration sécurisée à distance.
* **Supervision (Zabbix) :**
    * Monitoring complet de l'infrastructure : Switchs, Firewall et serveurs.
    * Alerting en temps réel sur l'état des services et la charge réseau.

## 🛡️ Focus Cybersécurité
* **Segmentation réseau :** Isolation des flux via VLANs dédiés (Management, Lab, IoT, DMZ).
* **Réduction de la surface d'attaque :** Application du principe du moindre privilège sur les règles de filtrage.
