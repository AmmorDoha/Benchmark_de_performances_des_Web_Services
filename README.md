## 📝 Architecture Microservices : Benchmark de Performances des Web Services REST

### Introduction

Ce projet de recherche et développement a pour objectif principal d'évaluer et de comparer les **performances brutes** de différentes approches d'implémentation d'API REST dans l'écosystème Java. Face à la popularité croissante des architectures microservices, il est crucial de comprendre l'impact des choix technologiques sur la latence, le débit et la fiabilité des services.

Ce benchmark fournit une analyse objective permettant d'éclairer les décisions techniques lors de la conception de systèmes distribués à haute performance.

---

### Objectifs du Benchmark

Nous avons comparé trois approches majeures d'implémentation de Web Services REST, en évaluant leur comportement sous forte charge :

* **Jersey (JAX-RS) :** Une implémentation légère et standard de la spécification JAX-RS.
* **Spring MVC (@RestController) :** L'approche classique d'API REST dans le framework Spring Boot.
* **Spring Data REST :** L'approche basée sur la convention qui expose automatiquement les repositories de données.

Les indicateurs de performance clés (KPIs) analysés incluent :

* **Latence (p50, p95, p99) :** Pour mesurer le temps de réponse moyen et les valeurs extrêmes.
* **Débit (Throughput) :** La capacité maximale de requêtes par seconde traitées.
* **Taux d'erreur :** L'évaluation de la fiabilité des services sous contrainte.

---

### Architecture et Technologies Utilisées

| Catégorie | Outils & Technologies |
| :--- | :--- |
| **Langage/Frameworks** | Java, Spring Boot, Jersey (JAX-RS) |
| **Base de Données** | [Nom de la BDD utilisée, ex: PostgreSQL, H2] |
| **Outil de Test de Charge** | JMeter |
| **Monitoring & Visualisation** | Prometheus, Grafana |
| **Conteneurisation** | Docker / Kubernetes (si applicable) |

---

### Résultats Clés (Synthèse)

* **Jersey** a généralement affiché la **latence la plus faible** (ex: p50 à **7.52 ms**), confirmant l'avantage des solutions légères JAX-RS dans certains scénarios.
* **Spring MVC & Spring Data REST** ont montré des performances très compétitives et équilibrées, soulignant l'efficacité de l'écosystème Spring même avec des niveaux d'abstraction plus élevés.
* Le projet conclut que tous les frameworks étudiés offrent une **excellente fiabilité** (<0.05% d'erreurs), le choix final dépendant du compromis souhaité entre performance brute, rapidité de développement et fonctionnalités d'écosystème.

---

### Réalisé par

* **Ammor Doha**
* **Aily Lina**

*Dans le cadre du projet d'Architecture Microservices, Date: 14-11-2025.*
