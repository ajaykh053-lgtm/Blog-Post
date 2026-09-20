# 📝 Blog Post

A full-featured blog web application built with Flask and PostgreSQL.
Users can register, log in, read posts, and leave comments.
The admin (first registered user) can create, edit, and delete posts.

## 🌐 Live Demo
[View Live](https://blog-post-u61w.onrender.com/post/1)

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
FLASK_KEY=your_secret_key(Type anything that's your falsk key)
DB_URI=postgresql+psycopg2://user:password@localhost/blogdb(You will get this in render when you create database there)
HASH_METHOD="YOURCHOICE"(https://werkzeug.palletsprojects.com/en/stable/utils/#module-werkzeug.security)
YOUR_EMAIL_ID=your_gmail@gmail.com
EMAIL_ID_PASSWORD=your_gmail_app_password
WHICH_EMAIL_YOU_WANT_TO_RECEIVE=Receiver_email@gmail.com
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

| Variable                          | Description                              |
|-----------------------------------|------------------------------------------|
| `FLASK_KEY`                       | Flask secret key for sessions            |
| `DB_URI`                          | PostgreSQL connection URI                |
| `HASH_METHOD`                     | Password hashing method (pbkdf2:sha256)  |
| `YOUR_EMAIL_ID`                   | Gmail address for contact form           |
| `EMAIL_ID_PASSWORD`               | Gmail App Password                       |
| `WHICH_EMAIL_YOU_WANT_TO_RECEIVE` | Email to receive contact form messages   |

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