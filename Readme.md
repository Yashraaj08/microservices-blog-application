## Microservices Journey — Node.js & React

### About This Project

This repository marks the **beginning of my journey into building microservices** using **Node.js** on the backend and **React** on the frontend.

To get hands-on experience, I’m starting with a **simple blog application** where users can:

* Create posts
* Add comments to posts
* See updates in real-time (eventually with event-based communication between services)

This project will grow step by step as I explore **service communication**, **event-driven design**, **API gateways**, **Dockerization**, **deployment**, and more.

---

### Project Structure

Initially, the system will have:

* **posts-service** → Handles creating and listing blog posts
* **comments-service** → Manages comments on posts
* **event-bus** → (coming soon) for inter-service communication
* **client** → React app for interacting with the backend

Example (future directory layout):

```
/microservices-blog
├── server/
|    └── posts/
|         ├── index.js
|         ├── package.json
|         └── package-lock.json
|    └── comments/
|         ├── index.js
|         ├── package.json
|         └──  package-lock.json
|    └── event-bus/
|         ├── index.js
|         ├── package.json
|         └──  package-lock.json
│
├── client/
│   ├── src/
│   └── package.json
│
└── README.md
```

---

### 🛠️ Tech Stack

* **Backend:** Node.js, Express
* **Frontend:** React
* **Database:** (to be added — possibly MongoDB or PostgreSQL)
* **Containerization:** Docker (coming soon)
* **Event Communication:** Custom Event Bus / Kafka / NATS (to explore)

---

### ⚙️ Setup Instructions

To run the services locally:

1. Clone the repository:

   ```bash
   git clone https://github.com/yashraaj08/microservices-blog.git
   cd microservices-blog
   ```

2. Install dependencies for each service:

   ```bash
   cd posts && npm install
   cd ../comments && npm install
   cd ../client && npm install
   ```

3. Start the services (in separate terminals):

   ```bash
   npm start
   ```

4. Open the client in your browser:
   👉 [http://localhost:3000](http://localhost:3000)

---

### 🧠 Learning Goals

* Understand the **fundamentals of microservice architecture**
* Learn how services **communicate asynchronously**
* Implement **event-driven communication**
* Manage **service discovery** and **data isolation**
* Deploy using **Docker & Kubernetes**