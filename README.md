# Atlas Talents 🎯

[![PHP Version](https://img.shields.io/badge/PHP-8.x-777BB4?style=flat&logo=php&logoColor=white)](https://php.net)
[![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat&logo=mysql&logoColor=white)](https://mysql.com)
[![OpenAI](https://img.shields.io/badge/OpenAI-API-412991?style=flat&logo=openai&logoColor=white)](https://openai.com)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

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