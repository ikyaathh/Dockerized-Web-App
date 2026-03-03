# Docker-containerized-app
📦 Dockerized Node.js Web Application
🚀 Project Overview

dockerweb-app is a simple Node.js web application containerized using Docker.
The project demonstrates containerization best practices, image optimization, and deployment workflow using Docker.

This project was built as part of hands-on DevOps practice to strengthen containerization and cloud deployment skills.

🛠️ Tech Stack

Node.js

Express.js

Docker

📂 Project Structure
dockerweb-app/
│
├── Dockerfile
├── .dockerignore
├── .gitignore
├── package.json
├── package-lock.json
├── index.js
└── README.md

⚙️ Application Features

Simple HTTP server

Uses environment variables

Runs inside a Docker container

Exposes port 3000

Lightweight Alpine-based image

🐳 Dockerfile Explanation

*Uses official node:18-alpine base image

*Sets working directory inside container

*Copies package files separately for better layer caching

*Installs dependencies

*Copies application source code

*Exposes port 3000

*Starts application using npm

🏗️ Build Docker Image
docker build -t dockerweb-app:1.0 .

▶️ Run Container
docker run -p 3000:3000 dockerweb-app:1.0

Open in browser:

http://localhost:3000

🌍 Using Environment Variables

You can override the default message:

docker run -p 3000:3000 -e MESSAGE="Hello Sai 🚀" dockerweb-app:1.0

🧪 Development Workflow

Build the image

Run the container

Test locally

Push image to Docker Hub (optional)

Integrate with CI/CD pipeline (future enhancement)

📈 Skills Demonstrated

>Dockerfile creation

>Image layering & caching

>Container networking (port mapping)

>Environment variable usage

>Docker CLI usage

>Git & GitHub version control

🔮 Future Enhancements

>Multi-stage Docker build

>GitHub Actions CI pipeline

>Push image to Docker Hub automatically

>Deploy to Kubernetes (Minikube / AKS)

>Deploy to Azure App Service

👨‍💻 Author

Poojitha Soma
DevOps Engineer
