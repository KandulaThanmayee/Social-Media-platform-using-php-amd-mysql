# 🧑‍🤝‍🧑 Social Media platform using php and mysql

A PHP-MySQL based social networking site built as a database project. Users can register, post content, like posts, send/accept friend requests, and search profiles. This project demonstrates core CRUD functionality and AJAX-driven interactivity in a traditional LAMP stack.

## 📁 Project Structure

- `index.php`, `register.php`, `login_handler.php`: Entry point and authentication.
- `config.php`: Database configuration.
- `User.php`, `Post.php`, `Notification.php`: Core backend classes.
- `post.php`, `profile.php`, `edit.php`, `friends.php`: Main UI views.
- `like.php`, `search.php`, `requests.php`, `logout.php`, `delete_post.php`: Interaction logic.
- `ajax_*.php`: AJAX endpoints for loading posts, notifications, and search suggestions.
- `demosocial.sql`: Database schema and seed data.
- `Report.pdf`: Project documentation with ER diagram, pseudocode, and feature overview.

## ✅ Features

- User registration with encrypted passwords (MD5)
- Login/logout system
- Post creation (text, image, or both)
- Like system
- Friend request system (send/accept/reject)
- Notification system for likes
- Full-text and filter-based search across profiles and posts
- User profile management

## 🛠️ Tech Stack

- Frontend: HTML, CSS, JavaScript
- Backend: PHP (procedural + OOP), AJAX
- Database: MySQL (via phpMyAdmin)
- Server: Apache (suggested via XAMPP or LAMP stack)

## 🗃️ Database

Import the SQL dump via phpMyAdmin or MySQL CLI:

```bash
mysql -u your_user -p your_database < demosocial.sql
```

The database name is `demosocial`. Make sure to update `config.php` with your credentials.

## 👥 Author: Thanmayee Kandula

## 🚀 Setup Instructions

1. Clone the repo or copy the files into your local server directory (e.g., `htdocs` for XAMPP).
2. Set up the MySQL database using `demosocial.sql`.
3. Adjust database credentials in `config.php`.
4. Start Apache and MySQL.
5. Navigate to `http://localhost/index.php` to begin.

## 📌 Notes

- Ensure PHP >= 7.3 and MySQL >= 10.4
- Image upload and display requires proper folder permissions
- Passwords use MD5 (for demo purposes only; avoid in production)
