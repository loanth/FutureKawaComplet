# FutureKawa

## 📖 Présentation

FutureKawa est une plateforme complète de gestion d'exploitation de café.

Le projet est organisé sous forme de plusieurs dépôts Git intégrés grâce aux **Git Submodules**, permettant de séparer les différents domaines fonctionnels tout en conservant un dépôt principal unique.


Pour voir l'historique de chaque commit, il faut clique sur chaque repo, cela vous redirigera vers son emplacement github et vous pourrez ainsi consulter les modifications.
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
- Gestion des Pays
- Gestion des Lots
- Gestion des stocks
- Base de données

Technologies :


- Python (Flask)
- Sql Alchemy



---

## FutureKawaFront

Application utilisée par les utilisateurs et le siège.

### Contenu

- Interface web
- Tableau de bord
- Gestion des exploitations/entrepôts/lots
- Gestion des utilisateurs
- Backend du siège

Technologies :

- React
- TypeScript

---

## futurekawa

Iot.

### Contenu

- Relève des mesures (humidité et température)
- Gestion des alertes par mail

Technologies :

- Python
- MQTT


---

## mspr_bloc4

Infrastructure du projet.

### Contenu

- Docker
- Pipeline CI/CD
- Déploiement automatique
- Monitoring
- Scripts d'installation

Technologies :

- Docker
- Jenkins

---

# 🚀 Installation

Cloner le dépôt avec tous les sous-modules :

```bash
git clone --recurse-submodules https://github.com/loanth/FutureKawaComplet.git
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
