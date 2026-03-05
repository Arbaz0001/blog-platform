# 📝 Modern Blog Platform

A full-stack **Blog Platform** built with **Next.js (Frontend)** and **Strapi CMS (Backend)**.
This project allows users to read blogs, like posts, comment on articles, reply to comments, and explore related posts based on categories.

---

## 🚀 Features

* 📰 Dynamic blog posts
* ❤️ Like system for posts
* 💬 Comment system with replies
* 🔗 Share blog posts
* 👤 Author name display after blog content
* 📂 Category-based blog filtering
* 🧠 Related blog recommendations
* 📱 Fully responsive UI
* ⚡ Fast performance with Next.js
* 🛠 Headless CMS powered by Strapi

---

## 🏗 Tech Stack

### Frontend

* **Next.js**
* **React**
* **Tailwind CSS**
* **Axios / Fetch API**

### Backend

* **Strapi CMS**
* **Node.js**

### Database

* SQLite (Development)
* PostgreSQL (Recommended for Production)

---

## 📁 Project Structure

```
blog-platform
│
├── client (Next.js frontend)
│   ├── components
│   ├── app
│   ├── pages
│   └── styles
│
├── server (Strapi backend)
│   ├── api
│   ├── config
│   ├── database
│   └── src
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```
git clone https://github.com/your-username/blog-platform.git
```

```
cd blog-platform
```

---

### 2️⃣ Install Frontend Dependencies

```
cd client
npm install
```

Run development server:

```
npm run dev
```

Frontend will run on:

```
http://localhost:3000
```

---

### 3️⃣ Install Backend (Strapi)

```
cd server
npm install
```

Start Strapi development server:

```
npm run develop
```

Backend will run on:

```
http://localhost:1337
```

---

## 🔐 Environment Variables

Create `.env.local` inside the frontend folder:

```
NEXT_PUBLIC_STRAPI_URL=http://localhost:1337
```

For production you can change it to:

```
NEXT_PUBLIC_STRAPI_URL=https://api.yourdomain.com
```

---

## 📡 API Example

Example request to fetch comments for a post:

```
GET /api/comments?filters[post][id][$eq]=POST_ID&populate=*
```

Create comment:

```
POST /api/comments
```

Body:

```
{
  "data": {
    "text": "This is a comment",
    "post": 1
  }
}
```

---

## 🌍 Deployment

Recommended deployment setup:

Frontend:

* **AWS Amplify**

Backend:

* **AWS EC2**

Database:

* **AWS RDS (PostgreSQL)**

Media Storage:

* **AWS S3**

---

## 📌 Future Improvements

* 🔔 Notification system
* 👍 Like system for comments
* 🧑 User authentication
* ✏️ Edit / delete comments
* 📊 Blog analytics
* 🔍 Advanced search

---

## 👨‍💻 Author

**Arbaz Sheikh**

Full Stack Developer (MERN Stack)

GitHub:
https://github.com/your-username

---

## 📜 License

This project is licensed under the MIT License.
