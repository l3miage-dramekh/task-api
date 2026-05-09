# 📋 API de Gestion de Tâches
API REST complète développée en Java avec Spring Boot.

## 🎯 Description

Cette API permet de gérer des tâches avec les opérations suivantes :
- Créer une tâche
- Consulter toutes les tâches
- Consulter une tâche par son id
- Modifier une tâche
- Supprimer une tâche
- Filtrer les tâches par statut (TODO / DONE)

## 🛠️ Technologies utilisées

- Java 17
- Spring Boot
- Spring Data JPA
- H2 Database (base de données en mémoire)
- Maven
- Postman (tests)

## 🧱 Architecture du projet
com.khoyane.taskapi
│
├── controller
│   └── TaskController.java
│
├── model
│   └── Task.java
│
└── repository
└── TaskRepository.java

## 📌 Les Endpoints

| Méthode | URL | Description |
|---|---|---|
| GET | /tasks ->  Récupérer toutes les tâches |
| GET | /tasks/{id} -> Récupérer une tâche par son id |
| POST | /tasks ->  Créer une nouvelle tâche |
| PUT | /tasks/{id} -> Modifier une tâche |
| DELETE | /tasks/{id} -> Supprimer une tâche |
| GET | /tasks/status/{status} -> Filtrer par statut |

## 💡 Exemple d'utilisation

Créer une tâche (POST /tasks) :

```json
{
  "title": "Faire mon CV",
  "description": "Ajouter mes projets et mon stage",
  "status": "TODO"
}
```

Réponse :

```json
{
  "id": 1,
  "title": "Faire mon CV",
  "description": "Ajouter mes projets et mon stage",
  "status": "TODO",
  "createdAt": "2026-05-03T15:46:52"
}
```

## 🚀 Lancer le projet

1. Cloner le repository
2. Ouvrir dans IntelliJ IDEA
3. Lancer `TaskapiApplication.java`
4. L'API est accessible sur `http://localhost:8080`

## 👩‍💻 Auteure

Khoyane DRAME — Licence 3 MIAGE
