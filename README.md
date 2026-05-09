# Atlas Talents 🎯

[![PHP Version](https://img.shields.io/badge/PHP-8.x-777BB4?style=flat&logo=php&logoColor=white)](https://php.net)
[![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat&logo=mysql&logoColor=white)](https://mysql.com)
[![OpenAI](https://img.shields.io/badge/OpenAI-API-412991?style=flat&logo=openai&logoColor=white)](https://openai.com)

> **Plateforme SaaS de détection de talents sportifs par intelligence artificielle**  
> *La première plateforme marocaine qui connecte professeurs d'EPS, recruteurs et clubs grâce à l'IA*

---

## 📸 Aperçu de la plateforme

| Page d'accueil | Fonctionnalités |
|----------------|-----------------|
| ![Landing](1-landing-page.png) | ![Features](2-features.png) |

| Connexion | Dashboard Professeur |
|-----------|---------------------|
| ![Login](3-login-page.png) | ![Professeur](4-teacher-dashboard.png) |

| Upload vidéo | Dashboard Élève |
|--------------|-----------------|
| ![Upload](5-upload-modal.png) | ![Élève](6-student-dashboard.png) |

| Dashboard Manager | Dashboard Recruteur |
|-------------------|---------------------|
| ![Manager](7-manager-dashboard.png) | ![Recruteur](8-recruiter-dashboard.png) |

| Dashboard Coach | Messagerie |
|-----------------|------------|
| ![Coach](9-coach-dashboard.png) | ![Chat](10-chat-panel.png) |

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
| 👨‍🏫 **Professeur** | Upload vidéo, analyse IA, suivi élèves, export PDF |
| 👟 **Élève** | Dashboard personnel, scores, progression |
| 🧭 **Manager** | Pipeline talents, shortlist, messagerie fédérée |
| 🏢 **Recruteur** | Filtres avancés, favoris, messagerie |
| 🏅 **Coach** | Suivi athlètes, graphiques Chart.js, radar IA |
| 🔧 **Admin** | Supervision plateforme, monitoring |

---

## 🛠️ Stack technique

| Catégorie | Technologies |
|-----------|--------------|
| **Backend** | PHP 8, PDO, MySQL, sessions sécurisées |
| **Frontend** | HTML5/CSS3, JavaScript vanilla, Design System custom |
| **IA / Vision** | OpenAI API (GPT-4.1-mini), extraction keyframes navigateur |
| **Graphiques** | Chart.js (line, bar, radar, doughnut) |
| **Sécurité** | CSRF, CSP, en-têtes HTTP, stockage hors webroot |
| **API** | REST endpoints (JSON) |

---

## 🚀 Installation rapide

```bash
git clone https://github.com/Idriss-23/atlas-talents.git
cd atlas-talents
cp .env.example .env
# Configurez votre base de données et clé OpenAI
mysql -u root -p < schema.sql
php -S localhost:8000
