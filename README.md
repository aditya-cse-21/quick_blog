# 🚀 QuickBlog – AI-Enhanced Blogging Platform

> A sleek, intelligent, and full-featured blogging system built with the MERN stack. QuickBlog empowers writers and admins with seamless tools, modern design, and AI-assisted content creation.

---

## 🔗 Live Preview

🌐 [Click here to view the live website](https://quick-blog-sncf.vercel.app/)

---

## 🌟 Highlights

### ✍️ Blog Features

- 📰 **Create Rich Blogs** – Write posts with a Quill.js-powered editor  
- 🤖 **AI Integration** – Generate content using Google Gemini AI  
- 🧠 **Instant Search** – Real-time filtering through blog posts  
- 📂 **Category Organization** – Group posts under categories  
- 💬 **Comment Section** – Engage readers with moderated comments  
- 📱 **Fully Responsive** – Optimized for all screen sizes  
- ⚡ **Performance Focused** – Fast load times and clean UI  

### 🔐 Admin Dashboard

- 🔐 **JWT Authentication** – Secure login for admins  
- 📈 **Analytics Overview** – View blog statistics and insights  
- ✍️ **Content Tools** – Add, edit, and delete blogs with ease  
- 📋 **Publish Control** – One-click publish/unpublish toggle  
- 🗨️ **Comment Moderation** – Approve or delete reader comments  
- 🖼️ **Image Management** – ImageKit integration for optimized visuals  

---

## 👨‍💻 Developer Stack

### Frontend

- ⚛️ React + Tailwind CSS  
- 🔀 React Router  
- 📝 Quill.js for WYSIWYG editing  
- 💨 Framer Motion for animations  
- 🔔 React Hot Toast for notifications  
- ⏱️ Moment.js for date formatting  

### Backend

- 🟢 Node.js + Express.js  
- 🍃 MongoDB (via Mongoose)  
- 🔐 JWT for authentication  
- 📁 Multer for file uploads  
- 🌐 CORS setup  

### AI + Cloud Services

- 🤖 Google Gemini AI for text generation  
- 🖼️ ImageKit for image CDN + optimization  
- ☁️ Vercel for frontend/backend deployment  

---

## ⚙️ Getting Started

### 📋 Requirements

- Node.js v16+  
- MongoDB Atlas or Local MongoDB  
- Environment variable configuration for both client & server  

### 🚀 Setup Guide

1. **Clone the repository**

```bash
git clone https://github.com/aditya-cse-21/quick_blog.git
cd quick_blog
```

2. **Install server dependencies**

```bash
cd server
npm install
```

3. **Install client dependencies**

```bash
cd ../client
npm install
```

4. **Setup environment variables**

Create a `.env` file in both `client` and `server` directories:

#### Server `.env`

```env
PORT=3000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
ADMIN_EMAIL=admin@example.com
ADMIN_PASSWORD=your_password
GEMINI_API_KEY=your_gemini_api_key
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url
```

#### Client `.env`

```env
VITE_BASE_URL=http://localhost:3000
```

5. **Start the servers**

```bash
# Start backend
cd server
npm start

# Start frontend (in a new terminal)
cd client
npm run dev
```

Open `http://localhost:5173` in your browser.

---

## 🗂️ Project Structure

```
QuickBlog/
├── client/            # React frontend
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── assets/
│   │   └── main.jsx
│   └── package.json
├── server/            # Node.js backend
│   ├── configs/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   └── server.js
└── README.md
```

---

## 📡 API Overview

### Blog APIs

- `GET /api/blog/all` – Fetch all blogs  
- `GET /api/blog/:blogId` – View a single blog  
- `POST /api/blog/add` – Create new blog (admin)  
- `POST /api/blog/delete` – Delete a blog (admin)  
- `POST /api/blog/toggle-publish` – Change publish status  
- `POST /api/blog/add-comment` – Submit a comment  
- `POST /api/blog/comments` – Get blog comments  
- `POST /api/blog/generate` – AI-generated blog content  

### Admin APIs

- `POST /api/admin/login` – Admin login  
- `GET /api/admin/blogs` – View all blogs  
- `GET /api/admin/comments` – View all comments  
- `GET /api/admin/dashboard` – View analytics  
- `POST /api/admin/approve-comment` – Approve comment  
- `POST /api/admin/delete-comment` – Delete comment  

---

## 🧠 Smart AI Content Generation

QuickBlog integrates Gemini AI to help you:

- Auto-generate entire blog posts from titles  
- Create catchy introductions and summaries  
- Save time and avoid writer’s block  

---

## 🖼️ Image Optimization with ImageKit

- CDN-delivered image assets  
- Smart compression and resizing  
- Faster load times, WebP format support  

---

## 🚀 Deployment Guide

### Frontend (Vercel)

1. Link GitHub repo to Vercel  
2. Add environment variables in the Vercel dashboard  
3. Deploy directly with CI/CD support  

### Backend (Vercel)

1. Add `vercel.json` for serverless setup  
2. Set backend env vars on Vercel  
3. Deploy with Vercel CLI or GitHub integration  

---

## 🤝 Contributions Welcome

Open a PR if you'd like to contribute! Follow these steps:

```bash
# Fork the repo
# Create a new branch
git checkout -b feature/NewFeature

# Commit and push
git commit -m "Add: NewFeature"
git push origin feature/NewFeature

# Submit a Pull Request
```

---

## 🙌 Credits

- Google Gemini AI for smart content generation  
- ImageKit for blazing-fast media delivery  
- Tailwind + React for a clean, modern UI  
- Community-driven libraries and tools ❤️  

---

<div align="center">
Made with 💻 and ☕ by **Aditya**

⭐️ Don’t forget to star the repo if you like it!
</div>
