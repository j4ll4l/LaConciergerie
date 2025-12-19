# 🚗 La Conciergerie Auto

Plateforme web d'intermédiation automobile permettant d'acheter et vendre des véhicules d'occasion en toute confiance avec l'accompagnement d'un concierge automobile.

## 📋 À propos du projet

La Conciergerie Auto est une application fullstack développée dans le cadre du **Titre Professionnel Développeur Web et Web Mobile** (Novembre 2025).

Cette plateforme agit comme un tiers de confiance pour faciliter les transactions automobiles entre particuliers, en offrant :
- 🤝 Un accompagnement personnalisé par des concierges automobiles
- 🔍 Des véhicules inspectés et garantis
- 📝 Une gestion administrative simplifiée
- 🛡️ Des transactions sécurisées

## 🛠️ Technologies utilisées

### Backend
- **Framework** : Symfony 6.4 (API REST)
- **ORM** : Doctrine
- **Base de données** : MySQL
- **Authentification** : JWT (LexikJWTAuthenticationBundle)
- **Stockage fichiers** : AWS S3 (avec conversion WebP automatique)
- **Email** : Symfony Mailer

### Frontend
- **Framework** : Vue.js 3 (Composition API)
- **Langage** : TypeScript
- **State Management** : Pinia
- **Routing** : Vue Router
- **HTTP Client** : Axios
- **Styling** : CSS personnalisé (thème dark mode)

### Outils & DevOps
- **IDE** : Visual Studio Code
- **Version Control** : Git & GitHub (repository privé)
- **Gestion de projet** : Trello (méthode Agile)
- **Hébergement** : o2switch
- **API Testing** : Bruno/Postman

## ✨ Fonctionnalités principales

### Pour les Clients
- ✅ Inscription et authentification sécurisée (vérification email)
- 📸 Demande d'estimation de véhicule avec upload de photos
- 🚙 Consultation du catalogue de véhicules avec filtres avancés
- 💳 Processus d'achat sécurisé avec gestion des transactions
- 📅 Prise de rendez-vous (visite ou récupération)
- 📄 Upload de documents (pièce d'identité, assurance)

### Pour les Concierges
- 📋 Pool d'estimations disponibles
- 💰 Soumission de prix d'estimation
- ➕ Création et gestion des annonces véhicules
- 🖼️ Upload multiple de photos (conversion WebP automatique)
- 🔄 Gestion complète des transactions
- 📆 Gestion de l'agenda des rendez-vous

### Pour les Administrateurs
- 👥 Gestion complète des utilisateurs
- 🚗 Supervision de tous les véhicules et estimations
- 💼 Vue d'ensemble des transactions
- 🔐 Accès sécurisé aux documents privés (URLs S3 pré-signées)

## 🗄️ Architecture

### Base de données (Méthode Merise)
- Modèle normalisé avec relations complexes
- Entités principales : User, Vehicle, Brand, Model, EstimationRequest, Transaction, Appointment
- Gestion des statuts via énumérations (LISTED/RESERVED/SOLD, etc.)
- Contraintes d'intégrité référentielle

### API REST
- Architecture RESTful avec endpoints organisés par fonctionnalité
- Authentification JWT avec système de rôles hiérarchiques
- Validation des données avec Symfony Validator
- Gestion des erreurs standardisée (codes HTTP appropriés)

### Frontend SPA
- Application Single Page responsive (mobile-first)
- Navigation Guards pour le contrôle d'accès par rôle
- Interfaces adaptatives (desktop/tablet/mobile)
- Gestion d'état centralisée avec Pinia

## 🔒 Sécurité

- ✅ Authentification JWT avec tokens signés
- ✅ Système de rôles hiérarchiques (CLIENT → CONCIERGE → ADMIN)
- ✅ Mots de passe hashés (bcrypt)
- ✅ Vérification email obligatoire
- ✅ Navigation Guards côté frontend
- ✅ Validation multi-niveaux (HTML5, JS, Backend)
- ✅ Documents privés protégés (URLs S3 temporaires)
- ✅ HTTPS obligatoire en production

## 🌱 Écoconception

- Conversion automatique des images en WebP (-25% à -35% de poids)
- CSS personnalisé léger (pas de framework lourd)
- Lazy loading des images
- Optimisation des requêtes API avec filtres côté serveur
- Police système (pas de téléchargement externe)

## 🔒 Accès au code source

**Ce projet est privé.**

Pour toute demande d'accès, de collaboration ou d'information complémentaire, contactez-moi :

📧 **jallaldevweb@gmail.com**

## 🚀 Roadmap

- [ ] Système de messagerie interne (chat temps réel)
- [ ] Notation et avis sur les concierges
- [ ] Historique de maintenance des véhicules
- [ ] Recherche géographique avec carte interactive
- [ ] Notifications push en temps réel
- [ ] Dashboard analytics avec KPI

## 👨‍💻 Développeur

**Jallal En Naour**  
Titre professionnel visé : Développeur Web et Web Mobile  
Novembre 2025

---

© 2025 La Conciergerie Auto. Tous droits réservés.
