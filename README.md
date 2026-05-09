# Atlas Talents 🎯

[![PHP Version](https://img.shields.io/badge/PHP-8.x-777BB4?style=flat&logo=php&logoColor=white)](https://php.net)
[![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat&logo=mysql&logoColor=white)](https://mysql.com)
[![OpenAI](https://img.shields.io/badge/OpenAI-API-412991?style=flat&logo=openai&logoColor=white)](https://openai.com)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

<<<<<<< HEAD
> Plateforme SaaS de détection de talents sportifs par intelligence artificielle

## 🧠 À propos

Atlas Talents connecte professeurs d'EPS, recruteurs et coachs autour d'un objectif commun : détecter les jeunes talents marocains grâce à un **agent IA** qui analyse automatiquement les performances vidéo sur 5 critères physiques.

### 🤖 Agent IA - Analyse vidéo intelligente

- Extraction automatique des keyframes côté navigateur
- Analyse via **OpenAI GPT-4.1-mini** (vision)
- Scoring sur 5 critères : Vitesse, Coordination, Endurance, Force, Souplesse
- Génération de résumés, points forts, axes de progression et recommandations
- Mode démo intelligent si l'API n'est pas configurée

## 👥 Rôles et fonctionnalités

| Rôle | Fonctionnalités |
|------|-----------------|
| 👨‍🏫 Professeur | Upload vidéo + analyse IA, suivi élèves, export PDF |
| 👟 Élève | Dashboard personnel, scores, progression |
| 🧭 Manager | Pipeline recrutement, shortlist, messagerie fédérée |
| 🏢 Recruteur | Filtres avancés, favoris, messagerie |
| 🏅 Coach | Suivi athlètes, graphiques Chart.js, radar IA |
| 🔧 Admin | Supervision plateforme, monitoring |

## 🛠️ Stack technique

| Catégorie | Technologies |
|-----------|--------------|
| Backend | PHP 8, PDO, MySQL, sessions sécurisées |
| Frontend | HTML5/CSS3, JavaScript vanilla, Design System custom |
| IA | OpenAI API (GPT-4.1-mini), vision, extraction keyframes |
| Graphiques | Chart.js (line, bar, radar, doughnut) |
| Sécurité | CSRF, CSP, headers HTTP, stockage hors webroot |
| API | REST endpoints (JSON) |
| Déploiement | Apache / XAMPP, compatible mutualisé/VPS |

## 🚀 Installation rapide

```bash
# 1. Cloner le projet
git clone https://github.com/VOTRE-PSEUDO/atlas-talents.git
cd atlas-talents

# 2. Copier la configuration
cp .env.example .env
# Éditez .env avec vos paramètres (DB, OpenAI, etc.)

# 3. Importer la base de données
mysql -u root -p < schema.sql

# 4. (Optionnel) Importer les données démo
mysql -u root -p atlas_talents < seed_demo.sql

# 5. Créer les dossiers de stockage
mkdir -p storage/uploads storage/private
chmod 755 storage/uploads storage/private

# 6. Lancer le serveur
php -S localhost:8000
# Ou utilisez Apache avec DocumentRoot pointant vers le dossier
=======
> **Plateforme SaaS de détection de talents sportifs par intelligence artificielle**  
> *La première plateforme marocaine qui connecte professeurs d'EPS, recruteurs et clubs grâce à l'IA*

---

## 📸 Aperçu de la plateforme

| Page d'accueil | Connexion |
|----------------|-----------|
| ![Landing](Capture%20d'écran%202026-05-09%20115306.png) | ![Login](Capture%20d'écran%202026-05-09%20115333.png) |

| Dashboard Professeur | Upload vidéo |
|----------------------|--------------|
| ![Professeur](Capture%20d'écran%202026-05-09%20115344.png) | ![Upload](Capture%20d'écran%202026-05-09%20115411.png) |

| Dashboard Élève | Dashboard Manager |
|-----------------|-------------------|
| ![Élève](Capture%20d'écran%202026-05-09%20115444.png) | ![Manager](Capture%20d'écran%202026-05-09%20115501.png) |

| Dashboard Recruteur | Dashboard Coach |
|--------------------|-----------------|
| ![Recruteur](Capture%20d'écran%202026-05-09%20115519.png) | ![Coach](Capture%20d'écran%202026-05-09%20115546.png) |

| Messagerie intégrée |
|---------------------|
| ![Messages](Capture%20d'écran%202026-05-09%20115605.png) |

---

## 🧠 Problématique résolue

**Détection insuffisante des talents sportifs dès le plus jeune âge au Maroc.**

Aujourd'hui, la détection repose sur des méthodes artisanales (observation terrain, bouche-à-oreille). Les professeurs d'EPS manquent d'outils objectifs, et les recruteurs n'ont pas accès facilement aux viviers de talents locaux.

**Atlas Talents industrialise ce processus grâce à l'IA.**

---

## 🤖 Agent IA – Analyse vidéo intelligente

| Fonctionnalité | Description |
|----------------|-------------|
| **Extraction automatique** | Keyframes extraites côté navigateur (6 images clés) |
| **Analyse vision** | via OpenAI GPT-4.1-mini |
| **5 critères physiques** | Vitesse, Coordination, Endurance, Force, Souplesse |
| **Scoring global** | 0-100, pondéré selon le sport |
| **Résumé intelligent** | Points forts, axes de progression, recommandations |
| **Mode démo** | Analyse locale cohérente si clé API manquante |

---

## 👥 6 rôles métiers – Dashboards dédiés

| Rôle | Fonctionnalités clés |
|------|----------------------|
| 👨‍🏫 **Professeur** | Upload vidéo, analyse IA automatique, suivi élèves, scores de classe, export PDF |
| 👟 **Élève** | Dashboard personnel, consultation scores, progression, objectifs, plan d'action |
| 🧭 **Manager recrutement** | Pipeline talents, shortlist prioritaire, messagerie fédérée, couverture géographique |
| 🏢 **Recruteur** | Filtres avancés (sport, ville, score min), système de favoris, messagerie |
| 🏅 **Coach** | Suivi athlètes, graphiques Chart.js, radar de performance, recommandations IA |
| 🔧 **Admin** | Supervision plateforme, monitoring, gestion utilisateurs |

---

## ✨ Fonctionnalités phares

### 🔐 Authentification multi-rôles
- Sessions sécurisées (HttpOnly, SameSite=Lax, Secure)
- CSRF tokens sur tous les formulaires sensibles
- Mot de passe hashés (bcrypt)
- 6 profils distincts avec redirection automatique

### 💬 Messagerie intelligente
- Détection automatique des contacts pertinents (selon étudiants partagés)
- Suggestions de messages contextuelles
- Marquage auto des conversations lues
- Stockage hybride (MySQL + fallback JSON)

### ⭐ Système de favoris
- Persistant (MySQL + fallback JSON)
- Synchronisation temps réel
- Badge de compteur dynamique

### 📊 Graphiques interactifs
- Chart.js : line, bar, radar, doughnut
- Filtrage par période (3, 6, 12 mois)
- Métriques au survol

### 📄 Export PDF
- Génération dynamique de rapports
- Graphiques et tableaux inclus
- Adapté à chaque rôle

### 🔒 Sécurité
- CSP configurable (HTML, API, média)
- Stockage vidéo hors webroot
- Serveur vidéo authentifié (`media.php`)
- En-têtes HTTP (X-Frame-Options, HSTS, Referrer-Policy)

---

## 🛠️ Stack technique

| Catégorie | Technologies |
|-----------|--------------|
| **Backend** | PHP 8, PDO, MySQL, sessions sécurisées |
| **Frontend** | HTML5/CSS3, JavaScript vanilla, Design System custom |
| **IA / Vision** | OpenAI API (GPT-4.1-mini), extraction keyframes navigateur |
| **Graphiques** | Chart.js (line, bar, radar, doughnut) |
| **Sécurité** | CSRF, CSP, en-têtes HTTP, stockage hors webroot |
| **API** | REST endpoints (JSON) – étudiants, progrès, stats, uploads, favoris, chat |
| **PDF** | Génération dynamique via `exportDashboardPdf()` |

---

## 📁 Architecture du projet
>>>>>>> d5dd5ee932a6ea6d3e500678598a990d6bad310b
