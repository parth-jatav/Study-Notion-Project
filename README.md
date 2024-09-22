
# StudyNotion

**StudyNotion** is a fully functional ed-tech platform built using the **MERN stack** (MongoDB, ExpressJS, ReactJS, NodeJS). The platform enables users to create, consume, and rate educational content, offering an immersive learning experience for students and a space for instructors to share their expertise globally.

## Features

### For Students:
- **Homepage**: Provides a brief introduction to the platform with links to available courses and user account details.
- **Course List**: Displays a list of courses along with descriptions and ratings.
- **Wishlist**: Allows students to add and view courses in their wishlist.
- **Cart & Checkout**: Facilitates course purchase and payment processing.
- **Course Content**: Provides access to course materials, including videos, documents, and other media.
- **User Details**: Allows users to view and edit account information.

### For Instructors:
- **Dashboard**: Offers an overview of courses, ratings, and feedback.
- **Insights**: Detailed insights into course performance, including views, clicks, and other metrics.
- **Course Management**: Enables instructors to create, update, and delete courses and manage content.
- **Profile Management**: Allows instructors to view and update their account information.

### For Admin (Future Scope):
- **Dashboard**: Provides a summary of platform metrics, including courses, users, and revenue.
- **Instructor Management**: Allows admins to manage instructor accounts, courses, and ratings.

## Tech Stack

- **Front-end**: Built using **ReactJS** with state management handled by **Redux**. Styling is done using **CSS** and **TailwindCSS**.
- **Back-end**: Powered by **NodeJS** and **ExpressJS** for scalable and robust server-side functionality.
- **Database**: **MongoDB**, a NoSQL database, is used for flexible data storage.
- **Authentication**: Utilizes **JWT** (JSON Web Token) for secure user authentication and **bcrypt** for password hashing.
- **Payment Integration**: Payments are processed via **Razorpay**.
- **Media Management**: Media files (images, videos, documents) are stored and managed using **Cloudinary**.

## Installation

To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/StudyNotion.git
   ```
   
2. Navigate to the project directory:
   ```bash
   cd StudyNotion
   ```

3. Install dependencies for both the server and client:
   ```bash
   # Install server dependencies
   cd backend
   npm install

   # Install client dependencies
   cd ../frontend
   npm install
   ```

4. Create a `.env` file in the `backend` directory and add your environment variables (e.g., MongoDB URI, JWT secret, Razorpay API key, Cloudinary credentials).

5. Run the application:
   ```bash
   # Run the backend
   cd backend
   npm run dev

   # Run the frontend
   cd ../frontend
   npm start
   ```

6. Open your browser and visit `http://localhost:3000`.

## API Documentation

StudyNotion follows RESTful API design, enabling seamless communication between the front end and back end. Below are some key API endpoints:

- `POST /api/auth/signup`: Create a new user account.
- `POST /api/auth/login`: Log in and generate a JWT token.
- `POST /api/auth/verify-otp`: Verify the OTP sent to the user's email.
- `GET /api/courses`: Fetch all available courses.
- `POST /api/courses`: Create a new course (for instructors).
- `PUT /api/courses/:id`: Update an existing course by its ID.
- `DELETE /api/courses/:id`: Delete a course by its ID.
- `POST /api/courses/:id/rate`: Add a rating to a course.

## Deployment

The platform can be deployed using cloud-based services:

- **Front-end**: Hosted on **Vercel**.
- **Back-end**: Hosted on **Render** or **Railway**.
- **Database**: Managed via **MongoDB Atlas**.
- **Media**: Media files stored and managed through **Cloudinary**.

## Future Enhancements

- **Gamification Features**: Add badges, points, and leaderboards to increase user engagement.
- **Personalized Learning Paths**: Create custom learning paths based on students' interests.
- **Social Learning Features**: Include peer-to-peer discussions, group projects, and collaborative tools.
- **Mobile App**: Develop a mobile app for better accessibility.
- **Machine Learning Recommendations**: Implement personalized course recommendations using ML algorithms.
- **Virtual Reality (VR) and Augmented Reality (AR) Integration**: Enhance the learning experience with immersive technologies.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.
