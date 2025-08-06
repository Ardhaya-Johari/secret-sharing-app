# 🔐 Secret Sharing App – Google OAuth & Local Auth

A full-stack authentication app that allows users to register, log in, and share their secrets anonymously. Built to learn how **Google OAuth 2.0**, **Passport.js**, and **bcrypt** work together in a real-world Node.js + PostgreSQL project.

---

## 🚀 Features

- 🔐 Local authentication (email + password)
- 🪪 Google OAuth 2.0 authentication
- 🧂 Password hashing with bcrypt
- 🔄 Session management with Passport.js
- 🗄️ PostgreSQL database integration
- 📝 Submit and view secrets
- 🎨 Clean UI with EJS templating + Bootstrap

---

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** PostgreSQL
- **Authentication:** Passport.js (Local & Google OAuth2)
- **Templating Engine:** EJS
- **Encryption:** bcrypt
- **Styling:** Bootstrap 5
- **Sessions:** express-session
- **Environment Config:** dotenv

---

## 🧪 Getting Started Locally

### 1. Clone the repo
```bash
git clone https://github.com/your-username/secret-sharing-app.git
cd secret-sharing-app
```
### 2. Install dependencies
```bash
npm install
```
### 3. Setup environment variables
Create a .env file in the root folder:
```bash
SESSION_SECRET=your-session-secret
PG_USER=your-db-username
PG_PASSWORD=your-db-password
PG_HOST=localhost
PG_DATABASE=your-db-name
PG_PORT=5432
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret
```
### 4. Setup PostgreSQL database
Create the following table:
```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email TEXT UNIQUE NOT NULL,
  password TEXT,
  secret TEXT
);

```
### 5. Run the server
```bash
node index.js

```
## 📁 Folder Structure
```pgsql
├── index.js
├── views/
│   ├── home.ejs
│   ├── login.ejs
│   ├── register.ejs
│   ├── secrets.ejs
│   ├── submit.ejs
│   └── partials/
│       ├── header.ejs
│       └── footer.ejs
├── public/
│   └── styles.css
├── .env.example
├── .gitignore
└── README.md
```

## 👩‍💻 Author

**Ardhaya Johari** – Full Stack Developer  
📧 ardhayasaxena3897@gmail.com  
🌐 [LinkedIn](https://www.linkedin.com/in/ardhaya-johari-819275321/)  
💻 [GitHub](https://github.com/Ardhaya-Johari)  

## 📄 License

MIT License

## ⭐️ Show Your Support
If you liked this project:

- ⭐️ Star the repo

- 🛠 Try it out locally

- 🗨 Give feedback or raise an issue


