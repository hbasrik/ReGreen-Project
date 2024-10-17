# ReGreen Project

ReGreen is a fullstack web application designed to encourage sustainable living by providing a platform where users can share content, engage in discussions, chat with each other, and form communities around sustainability issues. This application functions similarly to social media platforms like Instagram, allowing users to post about sustainability topics, interact with others, and build communities to promote sustainable practices.

## Features

- **User Authentication**: Register, login, and manage user profiles.
- **Content Sharing**: Users can post about sustainability topics, including images and text, similar to Instagram.
- **Chat Functionality**: Users can chat with each other in real time.
- **Community Building**: Create and join communities focused on sustainability topics.
- **Notifications**: Stay updated with notifications for posts, messages, and community activities.
- **Responsiveness**: The app is built to be responsive, ensuring a seamless experience across different devices.

### Backend

The backend of the application is built using **Node.js**, **Express**, and **MongoDB**. It handles the business logic, routing, and database interactions.

- **src/db/mongoose.js**: Manages the MongoDB connection setup.
- **src/middleware/**: Contains middleware to handle tasks like authentication.
- **src/models/**:
  - **otp.js**: Handles the One-Time Password (OTP) logic for verification purposes.
  - **user.js**: Defines the user schema and manages user-related database interactions.
- **src/routers/**:
  - **user.js**: Defines the API routes for user-related operations (register, login, profile management).
- **src/utils/**: Utility functions that are reused across different parts of the backend.
- **app.js**: The main entry point for the Express server.
- **index.js**: The main entry file to initialize and run the backend server.
- **package.json**: Lists all the dependencies for the backend project, including Express, Mongoose, etc.

### Frontend

The frontend is built using **React.js** and **Context API** for state management. It provides a responsive and interactive user interface where users can browse posts, join communities, and chat with others.

- **context/AuthContext.jsx**: Manages authentication state across the application (login, logout, user sessions).
- **helpers/toast.js**: Helper to show toast notifications for user actions.
- **hooks/useWindowSize.js**: Custom hook for handling responsive behavior.
- **layouts/**: Contains layout components for structuring the UI.
- **pages/**: Contains the main pages of the application:
  - **About**: Information about the ReGreen project.
  - **Contact**: Page for contacting the ReGreen team.
  - **Feed**: Main page where users can see posts related to sustainability.
  - **ForgotPassword**: Page to reset the user password.
  - **Home**: The homepage of the application.
  - **Login**: User login page.
  - **Messages**: Allows users to chat with others.
  - **NotFound**: 404 page for handling incorrect routes.
  - **Notifications**: Displays notifications related to user activity.
  - **Profile**: User profile page where users can view and edit their personal information.
  - **Projects**: Page to browse and join sustainability projects and communities.
  - **Register**: User registration page.
  - **Unauthorized**: Page shown to users who attempt to access restricted content.
 

### Backend Setup

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/repo-name.git
   cd ./backend
   npm install

2. **Set up .env file**:

   ```bash
   MONGODB_URL=mongodb://localhost:27017/your-database-name
   JWT_SECRET=your-jwt-secret
   npm run dev

3. **Navigate to ./frontend**:

   ```bash
   cd ./frontend
   npm install
   npm start


###
![WhatsApp Image 2024-10-17 at 05 43 40_59bd296a](https://github.com/user-attachments/assets/f9327325-ae26-4e90-9830-14439d2e1ea3)
