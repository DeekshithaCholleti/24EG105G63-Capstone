# Backend - Blog Application

The backend of the Blog Application is a RESTful API built with Node.js, Express, and MongoDB. It handles authentication, user roles, article management, and file uploads.

## 🛠️ Technologies

- **Express**: Web framework for Node.js.
- **Mongoose**: ODM for MongoDB.
- **JWT**: For secure user authentication.
- **Bcryptjs**: For hashing passwords.
- **Cloudinary**: For hosting images.
- **Multer**: For handling multipart/form-data.

## 📂 Directory Structure

- `APIs/`: Contains route-specific logic for Users, Authors, Admins, and Common authentication.
- `models/`: Mongoose models for User and Article entities.
- `middlewares/`: Custom middlewares for authentication (verifyToken) and error handling.
- `config/`: Configuration files for external services like Cloudinary.
- `server.js`: The main entry point of the application.

## 🚀 API Endpoints

### Auth (Common)
- `POST /auth/login` - User login
- `POST /auth/register` - New user registration

### User API
- `GET /user-api/articles` - Get all articles
- `PUT /user-api/comment/:articleId` - Add a comment to an article

### Author API
- `POST /author-api/article` - Create a new article
- `PUT /author-api/article/:articleId` - Update an existing article
- `GET /author-api/articles/:username` - Get articles by a specific author

### Admin API
- `GET /admin-api/users` - Get all users
- `DELETE /admin-api/user/:userId` - Delete a user

## 🔧 Installation & Setup

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Environment Variables**:
   Create a `.env` file in the `Backend` directory:
   ```env
   PORT=4000
   DB_URL=mongodb://localhost:27017/blogdb
   SECRET_KEY=your_secret_key
   CLOUDINARY_CLOUD_NAME=your_name
   CLOUDINARY_API_KEY=your_key
   CLOUDINARY_API_SECRET=your_secret
   ```

3. **Run the Server**:
   - Development: `npm run dev`
   - Production: `npm start`

## 🧪 Testing APIs
You can use the provided `.http` files (`user-req.http`, `author-req.http`, `admin-req.http`) with the REST Client extension in VS Code to test the endpoints.
