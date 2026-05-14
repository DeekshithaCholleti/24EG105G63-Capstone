# Frontend - Blog Application

The frontend of the Blog Application is a modern React application built with Vite and Tailwind CSS. It provides a seamless and interactive user interface for reading and writing blog posts.

## 🛠️ Technologies

- **React 19**: Library for building user interfaces.
- **Vite**: Next-generation frontend tooling.
- **Tailwind CSS v4**: Utility-first CSS framework.
- **Zustand**: Lightweight state management.
- **React Router 7**: For declarative routing.
- **React Hook Form**: For performant form management.
- **React Hot Toast**: For beautiful notifications.

## 📂 Key Components

- **Home**: Landing page showing featured articles.
- **Login/Register**: Authentication pages.
- **Articles**: List of all published articles.
- **ArticleById**: Detailed view of a single article with comments.
- **WriteArticles**: Form for authors to create new content.
- **AuthorProfile/AdminProfile**: Dashboards for different user roles.
- **ProtectedRoute**: Middleware component to protect authenticated routes.

## 🏗️ State Management

The application uses **Zustand** to manage global state, specifically user authentication data and UI preferences. The store is located in `src/store/`.

## 🚀 Installation & Setup

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Configuration**:
   Update `src/config.js` with your backend URL if necessary.

3. **Run Development Server**:
   ```bash
   npm run dev
   ```

4. **Build for Production**:
   ```bash
   npm run build
   ```

## 🎨 Styling
The project uses **Tailwind CSS v4**. Custom styles and configurations can be found in `src/index.css` and `vite.config.js`.
