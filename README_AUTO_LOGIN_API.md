
# Auto-login Registration API

Production-ready Flask API for instant user registration & login with JWT tokens.  
Includes rate-limiting, SQLite, Docker support.  
Perfect for SaaS, MVPs, rapid prototyping, and instant product launch.

---

## 🚀 Features

- **Register & auto-login:** one request, instant JWT token
- **Secure login:** email + password (hashed, never plain)
- **JWT authentication:** stateless, scalable
- **SQLite out of the box:** change DB in 1 line
- **Rate limiting:** brute-force protection for both registration & login
- **Docker-ready:** deploy in seconds
- **.env support:** easy configuration
- **Clean project structure:** easy to scale and maintain
- **Fully tested:** all endpoints verified with Postman

---

## 📦 Endpoints

### POST `/register`

**Request:**
```json
{
  "email": "testuser1@example.com",
  "password": "mysecret123"
}
```

**Response:**
```json
{
  "access_token": "<JWT>"
}
```

---

### POST `/login`

**Request:**
```json
{
  "email": "testuser1@example.com",
  "password": "mysecret123"
}
```

**Response:**
```json
{
  "access_token": "<JWT>"
}
```

---

## ⏱️ Rate Limits

- `/register`: 5 per hour
- `/login`: 10 per hour

---

## ⚡ Quick Start

### Run with Docker (recommended)
```bash
docker build -t auto-auth-api .
docker run -d -p 5000:5000 auto-auth-api
```

### Run locally
```bash
pip install -r requirements.txt
python app.py
```

### .env example
```
JWT_SECRET_KEY=your-jwt-secret-here
DATABASE_URI=sqlite:///users.db
```

---

## 🖼️ Screenshots
- `run_server.png` — API server running
- `register_postman.png` — registration in Postman
- `login_postman.png` — login in Postman

---

## 💡 Use cases
- Quick SaaS/MVP launches
- Instant integration into any backend

---

> 💡 You can see real examples on the Gumroad gallery.

---

## 💼 Ready-to-Use Version

You can get a ZIP version with all files, setup instructions, `.env.example`, and more:

👉 [Buy it on Gumroad](https://talabov.gumroad.com/)

---


## 📬 Contact

**Need this functionality in another language or stack (Node.js, Go, etc)?**  
Contact the author: talabov.ali72@gmail.com  
Telegram: [@talabovali](https://t.me/talabovali)

*Note: Pricing may vary depending on complexity and target stack.*

---

**Production ready. 100% manually tested. Ready for deployment and monetization!**
