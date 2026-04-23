# LearnEdge Edtech Platform

## Project Overview

LearnEdge is a comprehensive Edtech platform designed to provide a seamless learning experience for students and a robust course management system for instructors. It features a wide range of functionalities including course browsing, enrollment, payment integration, user authentication (student, instructor, admin roles), and a personalized dashboard.

## Features

### For Students:
- Browse and search for courses by category.
- Enroll in courses and track progress.
- Secure payment gateway integration.
- Personalized dashboard to manage enrolled courses.
- View course content, lectures, and assignments.
- Submit reviews and ratings for courses.

### For Instructors:
- Create, manage, and publish courses.
- Upload course content (videos, notes, assignments).
- View student enrollments and progress.
- Manage course sections and sub-sections.
- Track earnings and withdrawals.

### General:
- Robust user authentication and authorization.
- Responsive design for various devices.
- Admin panel for overall platform management (e.g., user management, category management).
- Modern UI/UX using Tailwind CSS.

## Technologies Used

- **Frontend:** React.js, Redux Toolkit, Tailwind CSS, React Router DOM
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Authentication:** JWT (JSON Web Tokens)
- **Cloud Storage:** Cloudinary (for media uploads)
- **Payment Gateway:** Razorpay
- **Other:** Swiper.js (for sliders), React Rating Stars Component

## Setup and Installation

To get this project up and running on your local machine, follow these steps:

### Prerequisites

- Node.js (v14 or higher)
- npm or Yarn
- MongoDB Atlas account (or local MongoDB instance)
- Cloudinary account
- Razorpay account

### Backend Setup

1.  **Clone the repository:**
    ```bash
    git clone <your-repo-url>
    cd studynotion-edtech-project-main
    ```
2.  **Navigate to the backend directory (if separate, otherwise assume root):**
    ```bash
    # cd backend (if applicable)
    ```
3.  **Install dependencies:**
    ```bash
    npm install
    # or yarn install
    ```
4.  **Create a `.env` file:**
    Copy the contents of `.env.example` into a new file named `.env` in the root of your project and fill in your credentials:
    ```
    PORT=5000
    MONGO_DB_URL=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret
    CLOUD_NAME=your_cloudinary_cloud_name
    API_KEY=your_cloudinary_api_key
    API_SECRET=your_cloudinary_api_secret
    MAIL_HOST=your_mail_host
    MAIL_USER=your_mail_user
    MAIL_PASS=your_mail_password
    RAZORPAY_KEY_ID=your_razorpay_key_id
    RAZORPAY_KEY_SECRET=your_razorpay_key_secret
    FRONTEND_URL=http://localhost:3000
    ```
5.  **Start the backend server:**
    ```bash
    npm start
    # or node server.js
    ```

### Frontend Setup

1.  **Navigate to the frontend directory (if separate, otherwise assume root):**
    ```bash
    # cd frontend (if applicable)
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    # or yarn install
    ```
3.  **Create a `.env` file:**
    If your frontend also uses environment variables (e.g., for API base URL), create a `.env` file in the frontend root and add them. For React, these typically start with `REACT_APP_`.
    ```
    REACT_APP_BASE_URL=http://localhost:5000/api/v1
    ```
4.  **Start the frontend development server:**
    ```bash
    npm start
    ```

## Usage

Once both frontend and backend servers are running, open your browser and navigate to `http://localhost:3000` (or whatever your `FRONTEND_URL` is set to).

## Contributing

Contributions are welcome! Please feel free to fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
