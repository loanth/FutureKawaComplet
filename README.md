# FutureKawa

## 📖 Présentation

FutureKawa est une plateforme complète de gestion de distributeurs automatiques de café connectés.

Le projet est organisé sous forme de plusieurs dépôts Git intégrés grâce aux **Git Submodules**, permettant de séparer les différents domaines fonctionnels tout en conservant un dépôt principal unique.

---

# 🏗️ Architecture du projet

```
FutureKawa
│
├── MSPR1              → API REST
├── FutureKawaFront    → Front-end + Backend Siège
├── futurekawa         → Application IoT
└── mspr_bloc4         → Déploiement & CI/CD
```

---

# 📦 Sous-modules

## MSPR1

API principale de la plateforme.

### Contenu

- API REST
- Authentification JWT
- Gestion des utilisateurs
- Gestion des machines
- Gestion des consommations
- Gestion des stocks
- Base de données

Technologies :

- ASP.NET Core
- Entity Framework
- SQL Server

---

## FutureKawaFront

Application utilisée par les utilisateurs et le siège.

### Contenu

- Interface web
- Tableau de bord
- Administration
- Gestion des machines
- Gestion des utilisateurs
- Backend du siège

Technologies :

- React
- Node.js
- Express

---

## futurekawa

Application embarquée sur les machines à café connectées.

### Contenu

- Communication avec l'API
- Gestion des capteurs
- Envoi des données
- Télémaintenance
- Synchronisation

Technologies :

- Python
- MQTT
- Raspberry Pi

---

## mspr_bloc4

Infrastructure du projet.

### Contenu

- Docker
- Kubernetes
- Pipeline CI/CD
- Déploiement automatique
- Monitoring
- Scripts d'installation

Technologies :

- Docker
- Kubernetes
- GitHub Actions / GitLab CI (à adapter)
- Ansible

---

# 🚀 Installation

Cloner le dépôt avec tous les sous-modules :

```bash
git clone --recurse-submodules <url-du-repo>
```

Si le dépôt est déjà cloné :

```bash
git submodule update --init --recursive
```

Pour récupérer les dernières versions :

```bash
git submodule update --remote --merge
```

---

# 📂 Structure

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
│   └── IoT
│
└── mspr_bloc4/
    └── Déploiement + Pipeline CI/CD
```

---

# 👥 Équipe

Projet réalisé dans le cadre du **MSPR**.

Les différents modules ont été développés de manière indépendante afin de faciliter la maintenance, le développement collaboratif et les déploiements.

---

# 📜 Licence

Projet réalisé dans un cadre pédagogique.
