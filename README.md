# Mini Social Media Posting App 

A backend-focused mini-project demonstrating **Data Association in MongoDB**. This application allows authenticated users to log in, access a protected profile, create posts, and view their specific posts. 

This project was built following the **Sheryians Coding School** Backend Development series (Part 18), but the styling has been refactored from Tailwind CSS to standard Vanilla CSS.

## 🚀 Features

* **User Authentication:** Secure login, register, and logout functionality using `bcrypt` and `jsonwebtoken` (JWT).
* **Protected Routes:** The profile dashboard cannot be accessed without a valid JWT cookie.
* **Data Association (MongoDB):** Implements a One-to-Many relationship where a Single `User` can have multiple `Posts`.
* **Create & View Posts:** Users can write posts that are saved to the database and immediately populated on their profile page in reverse chronological order.
* **Custom Styling:** Fully styled using a standard, custom `style.css` file instead of utility classes.

## 🛠️ Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MongoDB, Mongoose (Object Data Modeling)
* **View Engine:** EJS (Embedded JavaScript templates)
* **Styling:** Vanilla CSS
* **Security/Auth:** `cookie-parser`, `jsonwebtoken`, `bcrypt`

## 📁 Folder Structure

```text
├── app.js                 # Main application entry point and routes
├── models/
│   ├── post.js            # Mongoose schema for Posts
│   └── user.js            # Mongoose schema for Users
├── public/
│   └── stylesheets/
│       └── style.css      # Custom CSS file
└── views/
    ├── index.ejs          # Register page (assumed)
    ├── login.ejs          # Login page (assumed)
    └── profile.ejs        # User dashboard and post creation
