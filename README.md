Perfect 👍 — here’s your **cleaned-up `README.md`** version with all screenshot sections removed but still following the submission format and professional tone.
You can paste this directly into your repo; later, just add your screenshot links where you see the comments.

---

```markdown
# 🚀 Task 3 - Kaiburr Internship Assignment  
**Candidate:** Akshay  
**Date:** October 20, 2025  

---

## 📘 Overview
This repository contains **Task 3** of the Kaiburr internship assignment.  
In this task, I worked with **Docker, Docker Compose, and containerized applications** to demonstrate my understanding of container orchestration and service linking.

I’ve completed:
- **Task 1:** Basic Docker Compose setup with Nginx and MySQL  
- **Task 2:** Multi-service Compose setup (API + PostgreSQL)  
- **Task 4:** Dockerfile for a Python Flask app  

Each setup was built and tested individually using Docker Compose.

---

## 🧱 Folder Structure
```

Task 3 kaiburr/
│
├── Task1docker-compose/
│   └── docker-compose.yml
│
├── Task2docker-compose/
│   └── docker-compose.yml
│
├── Task4Dockerfile/
│   └── Dockerfile
│
├── DockerContainerLogs.txt
└── README.md  ← (this file)

````

---

## 🧩 Task 1 – Nginx + MySQL Setup

### Description
In this task, I created a simple **docker-compose.yml** file that launches:
- A **web service** using Nginx  
- A **database service** using MySQL  

The services share a custom Docker network and use persistent volumes.

### How to Run
```bash
cd Task1docker-compose
docker compose up
````

This will start both containers and make the web app available at
👉 [http://localhost:8080](http://localhost:8080)

---

## ⚙️ Task 2 – Backend API + PostgreSQL Setup

### Description

Task 2 demonstrates a more complex **multi-service Docker Compose** configuration.
It includes:

* A **Flask-based backend** (Python API)
* A **PostgreSQL database** connected via environment variables

### How to Run

```bash
cd Task2docker-compose
docker compose up
```

If you get a port conflict (for example `27017 already in use`), change the port mapping in the `docker-compose.yml` file:

```yaml
ports:
  - "27018:27017"
```

---

## 🐳 Task 4 – Building a Python App with Dockerfile

### Description

This task focuses on creating a **Dockerfile** for a simple Flask web application.
The file installs dependencies, exposes port `5000`, and runs `app.py`.

### How to Run

```bash
cd Task4Dockerfile
docker build -t myapp .
docker run -p 5000:5000 myapp
```

Then open the app at 👉 [http://localhost:5000](http://localhost:5000)

---

## 🧾 DockerContainerLogs.txt

This file contains container logs generated while testing the Docker Compose setups.
It includes timestamps, container startup messages, and connection logs — proving that containers were successfully executed locally.

---

## 🧠 Learnings

* Understood how **Docker Compose** links multiple containers via shared networks.
* Learned to debug **port conflicts** and fix them by editing mappings.
* Created and modified a **Dockerfile** to containerize Python applications.
* Practiced capturing logs and generating reproducible builds.

---

## ✅ Submission Compliance

* Each task is submitted in a **separate GitHub repository**.
* Each repository includes:

  * A detailed `README.md`
  * Working source code for all tasks
* No `.zip`, `.pdf`, or `.doc` files are included.
* AI assistance was used for learning and formatting purposes only — I personally understood, ran, and modified all code before submission.

---

## 📹 Optional (Extra Credit)

A short video walkthrough of the project can be recorded showing:

* Running containers in VS Code Terminal
* The date/time and my name visible on screen
* Brief explanation of how each task works

---


This submission was created by **Akshay** for evaluation purposes only.

```

---

Would you like me to now make a short **GitHub repository description + commit message template** (so your repo looks neat and consistent when you push it)?
```
