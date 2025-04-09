# Flask Docker Starter

This project demonstrates how to containerize a simple Flask web application using Docker.

## 🚀 Features

- Minimal Flask-based web app
- Dockerfile for building a custom image
- Environment variable support for dynamic content
- Port mapping (`5000:5000`)

## 🧰 Tech Stack

- Python 3.10
- Flask
- Docker

## ⚙️ Getting Started

Clone the repository and navigate into the project folder:

bash
git clone https://github.com/celiikerenn/flask-docker-starter.git
cd flask-docker-starter 

# 🐳 Build the Docker Image
docker build -t flask-docker-app .

# ▶️ Run the Container with an Environment Variable
docker run -d -p 5000:5000 -e APP_NAME="DockerFlaskApp" flask-docker-app

# ✅ Test the App
curl localhost:5000


# 💬 Example Output
Hello! My name is: DockerFlaskApp

# 📌 Notes
If APP_NAME is not set, it defaults to "VarsayılanUygulama".
This is a beginner-friendly setup ideal for learning Docker + Flask integration.

# 📂 Project Structure
Kopyala
Düzenle
flask-docker-starter/
├── app.py
├── Dockerfile
└── requirements.txt

# ✍️ Author
https://github.com/celiikerenn
