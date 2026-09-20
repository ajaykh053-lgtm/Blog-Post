# 📝 Blog Post

A full-featured blog web application built with Flask and PostgreSQL.
Users can register, log in, read posts, and leave comments.
The admin (first registered user) can create, edit, and delete posts.

## 🌐 Live Demo
[View Live](https://blog-post-u61w.onrender.com)

---

## ✨ Features

- 🔐 User authentication — register, login, logout
- 🛡️ Admin-only controls — create, edit, delete blog posts
- 💬 Comment system — logged-in users can comment on posts
- ✍️ Rich text editor (CKEditor) for writing posts
- 📬 Contact form with email notification
- 📱 Responsive UI with Bootstrap 5

---

## 🛠️ Tech Stack

| Layer      | Technology                        |
|------------|-----------------------------------|
| Backend    | Python, Flask                     |
| Database   | PostgreSQL, Flask-SQLAlchemy      |
| Auth       | Flask-Login, Werkzeug             |
| Frontend   | Bootstrap 5, Flask-CKEditor       |
| Deployment | Render                            |

---

## 🚀 Getting Started (Local Setup)

### 1. Clone the repository
```bash
git clone https://github.com/ajaykh053-lgtm/Blog-Post.git
cd Blog-Post
```

### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate      # Mac/Linux
venv\Scripts\activate         # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Create a `.env` file in the root directory
```env
FLASK_KEY=your_secret_key
DB_URI=postgresql+psycopg2://user:password@localhost/blogdb
HASH_METHOD=pbkdf2:sha256
EMAIL_KEY=your_gmail@gmail.com
PASSWORD_KEY=your_gmail_app_password
EMAIL-WHERE-YOU-WANT-T0-RECEIVE=your_email@gmail.com
```

### 5. Run the app
```bash
python main.py
```

Visit `http://localhost:5000` in your browser.

---

## 🗂️ Project Structure
---

Blog-Post/
│
├── static/ # CSS, JS, images
├── templates/ # HTML templates (Jinja2)
├── main.py # App entry point, routes, models
├── forms.py # WTForms form classes
├── requirements.txt # Python dependencies
├── Procfile # Render/Heroku deployment config
└── .env # Environment variables (not committed)

---

## 🔑 Environment Variables

| Variable                                               | Description                              |
|--------------------------------------------------------|------------------------------------------|
| `FLASK_KEY`                                            | Flask secret key for sessions            |
| `DB_URI`                                               | PostgreSQL connection URI                |
| `HASH_METHOD`                                          | Password hashing method (pbkdf2:sha256)  |
| `EMAIL_KEY`                                            | Gmail address for contact form           |
| `PASSWORD_KEY`                                         | Gmail App Password                       |
| `EMAIL-WHERE-YOU-WANT-T0-RECEIVE=your_email@gmail.com` | Email to receive contact form messages   |

---

## 👤 Admin Access

The **first user to register** on the site automatically
becomes the admin. Only the admin can:
- Create new blog posts
- Edit existing posts
- Delete posts

---

## 📄 License
This project is open source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author
**Ajay** — [GitHub](https://github.com/ajaykh053-lgtm)