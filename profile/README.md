# HealthCare

**🩺 Fiche de TP - Projet CDA : HealthCare**

📌 **Version du Starter Spring Boot :** 3.1.3

**🎯 Objectif du TP :** Ce TP vise à développer une application web permettant la gestion des patients et de leurs consultations dans un cadre hospitalier. Il repose sur une architecture en microservices et inclut une analyse statistique des données pour déterminer les risques de diabète.

---

🌟 **I. Spécifications Fonctionnelles**

1. **📝 Gestion des patients** (CRUD sauf suppression) :
    
    - ✅ Créer un patient
    - 📄 Lire les informations d'un patient
    - 🔄 Mettre à jour un patient
2. **💉 Gestion des consultations** (CRUD complet) :
    
    - ➕ Ajouter une consultation (note médicale)
    - 📖 Lire les consultations d'un patient
    - 🖊️ Mettre à jour une consultation
    - ❌ Supprimer une consultation
3. **📊 Analyse statistique :**
    
    - 📉 Détection du risque de diabète en fonction des notes médicales saisies par le médecin.

---

🛠️ **II. Spécifications Techniques**

#### **1. 🎨 Frontend**

- **Technologies :** Angular (ou autre framework au choix), Tailwind CSS, Bootstrap
- **Pages à développer :**
    - 🔑 Formulaires d'inscription et de connexion (Spring Security)
    - 🏠 Page d'accueil
    - 👥 Liste des patients
    - 📑 Liste des consultations
    - 📈 Page de scoring du diabète

#### **2. 🔗 Backend (Architecture microservices)**

- **Microservices principaux :**
    1. **🌐 Web App** : Interface utilisateur et gestion des requêtes
    2. **🗃️ Service Patient (CRUD - MySQL)**
    3. **🛢️ Base de données Patient (MySQL)**
    4. **📂 Service Consultation (CRUD - MongoDB)**
    5. **🛢️ Base de données Consultation (MongoDB)**
    6. **📊 Service de Scoring Diabète**
    7. **🖧 Eureka Server (Service Discovery)**
    8. **⚙️ Config Server (Gestion de configuration)**

#### **3. 🛠️ Environnements et Outils**

- **IDE :** IntelliJ / Eclipse / VS Code
- **Frameworks Backend :** Spring Boot, Spring Security
- **Base de données :** MySQL (patients), MongoDB (consultations)
- **Authentification :** Spring Security (Sign-up, Sign-in)
- **Containerisation :** Docker, Docker Compose
- **Gestion de version :** Git (commits réguliers pour chaque repository)

---

🚀 **III. Déroulement du TP**

#### **1. 🏗️ Mise en place de l'architecture**

- Créer les microservices avec **Spring Initializr**.
- Implémenter **Config Server** et **Eureka Server**.
- Déployer un **Docker Compose** minimal pour vérifier la mise en route des services.
- 📌 **Bonnes pratiques Git** : Faire des commits réguliers pour chaque avancée majeure.

#### **2. 🔄 Développement des services backend**

- Créer les microservices **Patient** et **Consultation** avec leurs bases de données respectives.
- Ajouter les endpoints REST pour le CRUD.
- Mettre en place l'authentification avec **Spring Security**.
- 📌 **Bonnes pratiques Git** : Créer une branche pour chaque fonctionnalité et faire des commits fréquents.

#### **3. 🎨 Développement du frontend**

- Implémenter les pages essentielles avec Tailwind / Bootstrap.
- Connecter le frontend avec les APIs backend.
- 📌 **Bonnes pratiques Git** : Documenter les commits et utiliser des messages clairs.

#### **4. ✅ Intégration et tests**

- Tester les microservices individuellement.
- Tester l'intégration avec Docker Compose.
- 📌 **Bonnes pratiques Git** : Fusionner régulièrement les branches et effectuer des revues de code.

---

📌 **IV. Critères de validation**

- ✅ Microservices fonctionnels avec endpoints REST.
- 🔐 Authentification et autorisation gérées via Spring Security.
- 💻 Frontend interactif et responsive.
- 🏥 Gestion des patients et consultations avec persistance des données.
- 📊 Détection du risque de diabète opérationnelle.
- 📌 **Validation Git** : Historique propre avec commits réguliers et messages explicites.

---

💡 **V. Bonnes pratiques**

- 🧪 **Tester** chaque fonctionnalité individuellement avant l'intégration.
- 📦 **Utiliser Docker Compose** régulièrement pour valider l'infrastructure.
- 📜 **Commenter le code** et suivre une architecture claire.
- 🔄 **Utiliser Git efficacement** : commits fréquents, branches pour chaque fonctionnalité, messages clairs.
