---

# 🏛️ Kebele Management System

A complete kebele management system with separate front-end and back-end repositories, managed together using Docker.

---

## 🚀 How to Run the Project

```bash
install **Docker Engine** and **Docker Compose** safely and easily.

---

## 🧩 Step 1: Uninstall old versions (optional but good)

Run this first (to avoid conflicts):

```bash
sudo apt remove docker docker-engine docker.io containerd runc
```

---

## 🧰 Step 2: Update your package list

```bash
sudo apt update
```

---

## 🧱 Step 3: Install required dependencies

```bash
sudo apt install ca-certificates curl gnupg lsb-release -y
```

---

## 🔑 Step 4: Add Docker’s official GPG key

```bash
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
```

---

## 📦 Step 5: Set up the Docker repository

```bash
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] \
  https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

---

## ⚙️ Step 6: Install Docker Engine and related tools

```bash
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin -y
```

---

## ✅ Step 7: Verify installation

```bash
sudo docker --version
sudo docker compose version
```

If you see version numbers, Docker is installed successfully 🎉

---

## 🔓 Step 8 (optional but important): Run Docker without `sudo`

By default, Docker needs `sudo`. To fix that:

```bash
sudo usermod -aG docker $USER
```

Then **log out and log back in**, or run:

```bash
newgrp docker
```

After this, you can use:

```bash
docker ps
```

without `sudo`.

---

✅ **Done!**
Now you can run your project using:

```bash
git clone --recurse-submodules https://github.com/birekassa/Kebele-management-System.git
cd Kebele-management-System
docker compose up --build
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
