# 🚀 MERN Stack Deployment Guide (Render & Netlify)

This guide outlines the steps used to deploy a MERN stack application with the backend on **Render** and the frontend on **Netlify**.

---

## 🌐 Deployed Application
- **Frontend URL:** [https://deploymentproject4.netlify.app/](https://deploymentproject4.netlify.app/)

---

## 1️⃣ Backend Deployment (Render)

### Prerequisites
- Completed Express.js backend
- GitHub repository with backend code
- MongoDB Atlas database
- Render account

### Steps
1. **Push your backend code to GitHub.**
2. **Create a MongoDB Atlas cluster** and get your connection string.
3. **Sign in to [Render](https://render.com/)** and click "New Web Service".
4. **Connect your GitHub repository** and select your backend repo.
5. **Configure environment variables** (e.g., `MONGODB_URI`, `JWT_SECRET`, etc.) in the Render dashboard.
6. **Set the build and start commands** (e.g., `npm install` and `npm start`).
7. **Deploy the service.** Render will build and deploy your backend.
8. **Copy the Render backend URL** for use in your frontend.

---

## 2️⃣ Frontend Deployment (Netlify)

### Prerequisites
- Completed React frontend
- GitHub repository with frontend code
- Netlify account

### Steps
1. **Push your frontend code to GitHub.**
2. **Sign in to [Netlify](https://netlify.com/)** and click "Add new site" > "Import an existing project".
3. **Connect your GitHub repository** and select your frontend repo.
4. **Configure build settings:**
   - Build command: `npm run build`
   - Publish directory: `build`
5. **Set environment variables** (e.g., `REACT_APP_API_URL` pointing to your Render backend URL).
6. **Deploy the site.** Netlify will build and deploy your frontend.
7. **Copy the Netlify site URL** (see above).

---

## 3️⃣ Documentation & CI/CD
- Both Render and Netlify support automatic deployments from GitHub on push.
- Ensure your `.env.example` files are included in your repo for reference.
- Document all environment variables and deployment steps in your main `README.md`.

---

## 4️⃣ Screenshots
- See `Screenshot.docx` in this repository for deployment and CI/CD pipeline screenshots.

---

## 5️⃣ Useful Links
- [Render Documentation](https://render.com/docs)
- [Netlify Documentation](https://docs.netlify.com/)
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)

---

**Happy Deploying!** 