# 🔐 Kerberos : Le Gardien des Identités Réseau

## 📌 Qu'est-ce que Kerberos ?

**Kerberos** est un protocole d’authentification réseau sécurisé, basé sur un système de **tickets** et utilisant un **tiers de confiance centralisé**. Il a été développé par le **MIT** et est largement utilisé dans les environnements **Windows Active Directory**, **Linux**, etc.

🎯 **Objectif** : Authentifier les utilisateurs et les services sans transmettre de mot de passe en clair sur le réseau.

---

## 🧠 Fonctionnement Simplifié

1. L’utilisateur entre son identifiant + mot de passe.
2. Le serveur Kerberos délivre un **TGT** (Ticket Granting Ticket).
3. Ce TGT est utilisé pour demander des **tickets de service**.
4. Les tickets de service permettent l’accès aux ressources réseau **sans re-saisie des identifiants**.

---

## 📦 Composants Clés

| Composant        | Rôle                                                |
|------------------|-----------------------------------------------------|
| **Client**        | L'utilisateur ou la machine qui demande un service |
| **KDC**           | Key Distribution Center (serveur d’authentification) |
| **AS**            | Authentication Server (partie du KDC)              |
| **TGS**           | Ticket Granting Server (fournit les tickets de service) |
| **Service cible** | Ressource à laquelle le client veut accéder        |

---

## 🔐 Atouts Sécurité

- Aucun mot de passe envoyé en clair
- Utilise le **chiffrement symétrique** (ex : AES)
- Tickets à **durée de vie limitée**
- Authentification **mutuelle** entre client et service

---

## 🖥️ Cas d’utilisation

- **Active Directory** (Windows)
- **Serveurs Linux** (via PAM et Kerberos)
- **Applications web** (ex. : Apache avec mod_auth_kerb)
- **Clusters Big Data** (Hadoop sécurisé)
- **Réseaux d’entreprise**, universités, institutions publiques…

---

## ✅ Avantages

- 🔐 Authentification unique (SSO)
- 📉 Moins de saisie d'identifiants
- 🔄 Intégration avec les systèmes d’entreprise
- 🛡️ Sécurité forte sans révéler les mots de passe

---

## ⚠️ Limites

- 🧠 Complexe à configurer
- 🕒 Sensible à la désynchronisation des horloges
- 📡 Dépendance au **serveur KDC** (point de défaillance unique)

---

## 📚 En résumé

| Élément         | Détail                                          |
|-----------------|-------------------------------------------------|
| 🔐 Protocole    | Authentification par ticket                     |
| 🏢 Composants   | Client, KDC, AS, TGS, service cible              |
| 🛡️ Sécurité     | Chiffrement, tickets, aucune info sensible transmise |
| 🧾 SSO          | Oui                                              |
| ⚠️ Faiblesses   | KDC critique, dépendant de la synchronisation horaire |

---

> Kerberos est un protocole incontournable pour toute infrastructure réseau sécurisée. Comprendre son fonctionnement est essentiel pour les administrateurs systèmes et les spécialistes cybersécurité.




![Image](https://github.com/user-attachments/assets/c05c7ca1-9c82-4d4a-8765-d8aa64e36026)
