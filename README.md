# FutureKawa

## 📖 Présentation

FutureKawa est une plateforme complète de gestion d'exploitation de café.

Le projet est organisé sous forme de plusieurs dépôts Git intégrés grâce aux **Git Submodules**, permettant de séparer les différents domaines fonctionnels tout en conservant un dépôt principal unique.

Chaque sous-module possède son propre historique Git. Pour consulter les commits d'un module, il suffit d'ouvrir son dépôt GitHub.

---

# 🏗️ Architecture du projet

```
FutureKawa
│
├── MSPR1              → API REST
├── FutureKawaFront    → Front-end + Backend Siège
├── futurekawa         → Application IoT
└── mspr_bloc4         → Déploiement & Infrastructure
```

---

# 📦 Sous-modules

## 📌 MSPR1

API principale de la plateforme.

### Contenu

- API REST
- Authentification JWT
- Gestion des utilisateurs
- Gestion des pays
- Gestion des lots
- Gestion des stocks
- Gestion des exploitations
- Base de données

### Technologies

- Python
- Flask
- SQLAlchemy

---

## 📌 FutureKawaFront

Application web destinée aux exploitants ainsi qu'au siège.

### Contenu

- Interface utilisateur
- Tableau de bord
- Gestion des exploitations
- Gestion des entrepôts
- Gestion des lots
- Gestion des utilisateurs
- Backend du siège

### Technologies

- React
- TypeScript

---

## 📌 futurekawa

Application IoT chargée de la collecte des données environnementales.

### Contenu

- Communication MQTT
- Relevé de température
- Relevé d'humidité
- Détection des anomalies
- Envoi d'alertes par e-mail
- Communication avec l'API

### Technologies

- Python
- MQTT

---

## 📌 mspr_bloc4

Infrastructure complète du projet.

### Contenu

- Déploiement automatisé
- Docker
- Pipeline CI/CD
- Monitoring
- Scripts d'installation
- Infrastructure réseau

### Technologies

- Docker
- Jenkins
- Ansible
- Kubernetes
- Vagrant

---

# 🚀 Installation

## Cloner le dépôt avec tous les sous-modules

```bash
git clone --recurse-submodules https://github.com/loanth/FutureKawaComplet.git
```

## Si le dépôt est déjà cloné

```bash
git submodule update --init --recursive
```

## Mettre à jour tous les sous-modules

```bash
git submodule update --remote --merge
```

---

# 📂 Structure du projet

```
FutureKawa/
│
├── MSPR1/
│   └── API REST
│
├── FutureKawaFront/
│   └── Front-End + Backend Siège
│
├── futurekawa/
│   └── Application IoT
│
└── mspr_bloc4/
    └── Déploiement & Infrastructure
```

---

# 📄 Documentation & Livrables

L'ensemble des livrables du projet est disponible dans le dossier Google Drive suivant :

**📁 Drive :**
https://drive.google.com/drive/folders/1cFSDXxpxDLyMFDlM6HvAx3KyfGEDO_SU?usp=drive_link

## Documents disponibles

### Documentation technique:
https://docs.google.com/document/d/1qHNEnTYuvaGlVSpqo95JWb6ERUWzOa1F/edit?usp=drive_link&ouid=118407143009922199261&rtpof=true&sd=true

- Documentation Fonctionnelle
- Documentation Technique API
- Documentation MQTT / IoT
- Documentation Front-End
- Documentation de Déploiement

### Documentation utilisateur:
https://docs.google.com/document/d/1nkkXznevjtu_qED20DM3ZW3qzvPKrPfn/edit?usp=sharing&ouid=118407143009922199261&rtpof=true&sd=true

### Questionnaire phase 2:
https://docs.google.com/document/d/1C5xYHLuIQycntoGMV8gny4ufbK5c1ILo/edit?usp=sharing&ouid=118407143009922199261&rtpof=true&sd=true

### Plan de Formation
https://docs.google.com/document/d/1dFEkcoPwkcmm2D8nfQM3rzLi4pNQeYZc/edit?usp=sharing&ouid=118407143009922199261&rtpof=true&sd=true

### Plan de maintenance
https://docs.google.com/document/d/1gcYtMYdGcbh_RZjiMnJq6dQn4_shAq10/edit?usp=sharing&ouid=118407143009922199261&rtpof=true&sd=true

### Prototype schéma Iot phase 2:
https://drive.google.com/file/d/1xW3_DViSalOsT0gXs9VdKICoSPoQKD4e/view?usp=sharing

# 👥 Organisation du projet

Le projet est composé de quatre dépôts Git indépendants reliés grâce aux **Git Submodules**.

Cette architecture permet :

- une séparation claire des responsabilités ;
- un développement parallèle des différents modules ;
- une maintenance facilitée ;
- des déploiements indépendants ;
- un historique Git propre pour chaque composant.

---

# 👥 Équipe

Projet réalisé dans le cadre du **MSPR (Mise en Situation Professionnelle)**.

Les différents composants ont été développés de manière indépendante afin de respecter une architecture modulaire proche d'un contexte professionnel.

---

# 📜 Licence

Projet réalisé dans un cadre pédagogique.
