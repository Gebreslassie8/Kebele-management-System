---

# 🏛️ Kebele Management System

A complete kebele management system with separate front-end and back-end repositories, managed together using Docker.

---

## 🚀 How to Run the Project

```bash
# 1. Clone the main project (including submodules)
git clone --recurse-submodules https://github.com/birekassa/Kebele-management-System.git

# 2. Move into the project folder
cd Kebele-management-System

# 3. Build and run the containers
docker-compose up --build
```

The client will be available at:
👉 **[http://localhost:3000](http://localhost:3000)**

The server will be available at:
👉 **[http://localhost:5000](http://localhost:5000)**

---

## 🧱 Project Structure

```
Kebele-management-System/
├── client/   → Front-end (React)
├── server/   → Back-end (Express + Supabase)
└── docker-compose.yml
```

---
