Tinder-AI — Full-Stack AI-Powered Dating App

Built by Saransh Padmaker | Java • Spring Boot • GPT-4 • Stable Diffusion • MongoDB

📌 About The Project
Tinder-AI is a full-stack AI-powered dating application that simulates a modern dating experience enriched with artificial intelligence. Users can browse AI-generated profiles, interact with intelligent chatbots, and experience dynamic conversations — all powered by GPT-4 and Stable Diffusion.
This project was built to deepen my understanding of:

Integrating Large Language Models (LLMs) into real-world applications
Building production-grade RESTful APIs with Spring Boot
Connecting AI-generated content (text + images) via RESTful APIs


✨ Features

🤖 AI Profile Generation — Dynamically generates realistic user profiles using GPT-4
🖼️ AI Profile Images — Custom profile pictures generated via Stable Diffusion
💬 AI Chatbots — Each profile has a personalized conversational AI for realistic interactions
🔗 15+ RESTful APIs — Robust backend APIs managing 500+ user profiles
🗄️ MongoDB Integration — Efficient NoSQL data storage for profiles and conversations


🛠️ Tech Stack
LayerTechnologyBackendJava, Spring Boot, REST APIsDatabaseMongoDBAI - TextOpenAI GPT-4AI - ImagesStable DiffusionDevOpsDocker, Git, GitHub

🏗️ Architecture Overview
├── src/
│   ├── controllers/          # REST API Controllers (15+ endpoints)
│   ├── services/             # Business Logic + GPT-4 Integration
│   ├── models/               # MongoDB Data Models
│   ├── repositories/         # MongoDB Repositories
│   └── config/               # App Configuration
│
└── docker-compose.yaml       # Container Orchestration

🚀 Getting Started
Prerequisites

Java 17+
MongoDB (local or Atlas)
OpenAI API Key
Stable Diffusion API Key

Setup
bash# Clone the repository
git clone https://github.com/saransh123p/tinder-ai-app.git
cd tinder-ai-app

# Add your API keys in application.properties
# openai.api.key=YOUR_KEY_HERE

# Run the Spring Boot application
./mvnw spring-boot:run
Using Docker
bash# Run everything with Docker Compose
docker-compose up --build

📡 API Endpoints
MethodEndpointDescriptionGET/api/profilesFetch all AI-generated profilesPOST/api/profiles/generateGenerate a new AI profileGET/api/profiles/{id}Get a specific profilePOST/api/chat/{profileId}Send a message to AI chatbotGET/api/chat/{profileId}/historyGet conversation historyDELETE/api/profiles/{id}Delete a profile

💡 Key Learnings
Working on this project helped me understand:

LLM Integration — How to craft effective prompts for GPT-4 to generate consistent, realistic persona data
AI + Backend — Connecting generative AI APIs within a Spring Boot service layer cleanly
Async Operations — Managing AI API response times without blocking the backend
NoSQL Design — Modeling flexible conversation and profile data in MongoDB
API Design — Building clean, scalable RESTful APIs with Spring Boot and MongoDB


🙋‍♂️ Author
Saransh Padmaker
📧 saransh123p@gmail.com
🔗 LinkedIn
💻 GitHub

📄 License
This project is open source and available under the MIT License.
