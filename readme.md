
# API REST avec Node.js, Express et Mongoose

Ce projet est une API REST simple construite avec Node.js, Express et Mongoose. Elle permet de gérer des utilisateurs en effectuant des opérations CRUD (Create, Read, Update, Delete) sur une base de données MongoDB.

## Prérequis

Avant de commencer, assurez-vous d'avoir installé les éléments suivants sur votre machine :

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)

## Installation

1. Clonez le dépôt :

```bash
git clone https://github.com/anse-dev/mini-api-tutorial.git
cd mini-api-tutorial
```

2. Installez les dépendances :

```bash
npm install
```

3. Créez un fichier `.env` dans le dossier `config` et ajoutez votre URI MongoDB :

```env
MONGO_URI='votre_uri_mongodb_atlas'
```

## Utilisation

1. Lancez le serveur :

```bash
npm start
```

Le serveur démarrera sur le port 3000.

## Routes

- **GET** `/users` - Retourner tous les utilisateurs
- **POST** `/users` - Ajouter un nouvel utilisateur
- **PUT** `/users/:id` - Modifier un utilisateur par ID
- **DELETE** `/users/:id` - Supprimer un utilisateur par ID

### Exemples de requêtes avec Postman

#### GET : Retourner tous les utilisateurs

- URL : `http://localhost:3000/users`
- Méthode : GET

#### POST : Ajouter un nouvel utilisateur

- URL : `http://localhost:3000/users`
- Méthode : POST
- Body (JSON) :
```json
{
  "name": "John Doe",
  "age": 30,
  "email": "john.doe@example.com"
}
```

#### PUT : Modifier un utilisateur par ID

- URL : `http://localhost:3000/users/:id`
- Méthode : PUT
- Body (JSON) :
```json
{
  "name": "Jane Doe",
  "age": 25,
  "email": "jane.doe@example.com"
}
```

#### DELETE : Supprimer un utilisateur par ID

- URL : `http://localhost:3000/users/:id`
- Méthode : DELETE

## Structure des dossiers

```
project-root/
│
│
├── src/models/
│   └── User.js
│
└── server.js
```

## Liens utiles

- [.env](https://www.npmjs.com/package/dotenv)
- [Express.js](https://expressjs.com/)
- [Req.params & req.query](https://coursework.vschool.io/express-params-and-query/)
- [Mongoose](https://mongoosejs.com/)
- [REST API](https://www.youtube.com/watch?v=SLwpqD8n3d0)

## Auteur

- [Votre Nom](https://github.com/anse-dev)

