# Inspire Blog API

A clean, lightweight REST API for blog posts, users, comments, and favorites built with Node.js,
TypeORM, MySQL, and Docker.



## 🔧 Features

-    CRUD operations for posts, users, comments, and favorites
-    Authentication (e.g. JWT or Sessions)
-    Fully Dockerized setup (backend + MySQL)
-    ORM using TypeORM with automatic migrations
-    Easy configuration via `.env`
-    Email notifications via SMTP (optional)


## 🚀 Prerequisites

-    Docker and Docker Compose
-    Node.js (v18+)
-    `.env` file with MySQL and SMTP credentials



## 📅 Installation & Setup

```bash
git clone https://github.com/yourusername/Inspire-Blog-API.git
cd Inspire-Blog-API
cp .env.example .env
docker compose up -d
npm install
npm run dev
```

API should now be accessible at `http://localhost:3000`



## 📚 API Endpoints

-    `POST /auth/register` – Register a new user
-    `POST /auth/login` – User login
-    `GET /posts` – List all posts
-    `POST /posts` – Create new post
-    `GET /posts/:id` – Get specific post
-    `POST /posts/:id/comments` – Add comment
-    `POST /favorites/:postId` – Mark favorite

_(Provide request-response examples where applicable)_



## ⚙️ Configuration (from `.env`)

| Key             | Description                         | Default           |
| --------------- | ----------------------------------- | ----------------- |
| `DB_HOST`       | Database host (Docker service name) | `mysql`           |
| `DB_PORT`       | Database port                       | `3306`            |
| `DB_NAME`       | Name of database                    | `blog_orm`        |
| `DB_USERNAME`   | MySQL username                      | `root`            |
| `DB_PASSWORD`   | MySQL password                      | _(empty)_         |
| `SMTP_SERVER`   | Email SMTP server                   | `smtp.google.com` |
| `SMTP_USER`     | SMTP login email                    | your email        |
| `SMTP_PASSWORD` | SMTP password or app-password       | your secret       |



## 🔪 Running Tests

```bash
npm test
```



## 📄 License

MIT © Sai Lin Htut
