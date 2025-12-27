# 🟦 Fullstack Social Media App

A fullstack social media application with a **React frontend** and a **Node.js + Express backend**, fully containerized with Docker.
Users can create profiles, post content, like and comment on posts, and switch to dark mode. Images are uploaded using **Cloudinary**.

---

## 🛠️ Technology Stack

* **Frontend:** React, JavaScript, Sass, served via **Nginx**
* **Backend:** Node.js + Express in TypeScript, **Prisma** ORM, **JWT** authentication
* **Database:** PostgreSQL
* **File Uploads:** Cloudinary
* **Containerization:** Docker & Docker Compose

---

## ⚡ Features

* User registration and authentication
* Profile creation and editing
* Create, edit, and delete posts
* Like and comment system
* Dark mode theme
* Image uploads with Cloudinary
* Fully containerized setup with Docker

---

## 🚀 Getting Started

### Requirements

* [Docker](https://www.docker.com/) & [Docker Compose](https://docs.docker.com/compose/) installed

### Setup

1. Clone the repository:

```bash
git clone https://github.com/yourusername/squad-social-media.git
cd squad-social-media
```

2. Create a `.env` file with your environment variables (example):

```env
DATABASE_URL=postgresql://postgres:postgres@db:5432/squad
JWT_SECRET=supersecretkey
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

3. Run Docker Compose:

```bash
docker compose up --build
```

* Frontend will be available at [http://localhost:3000](http://localhost:3000)
* Backend will run on [http://localhost:4000](http://localhost:4000)

---

## 🗂️ Project Structure

```
squad-social-media/
├─ front/       # React frontend
├─ api/         # Express backend with TypeScript & Prisma
├─ docker-compose.yml
└─ .env
```

---

## ✅ Notes

* Frontend served via **Nginx** for production-ready static hosting
* Backend is fully **RESTful** and communicates with frontend through Docker network
* Images uploaded via **Cloudinary**
* Database runs in a separate **PostgreSQL Docker container**
