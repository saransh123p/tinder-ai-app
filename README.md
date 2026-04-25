 Tinder-AI — Full-Stack AI-Powered Dating App

Built by Saransh Padmaker | Java • Spring Boot • React.js • GPT-4 • Stable Diffusion • MongoDB

📌 About The Project
Tinder-AI is a full-stack AI-powered dating application that simulates a modern dating experience enriched with artificial intelligence. Users can browse AI-generated profiles, interact with intelligent chatbots, and experience dynamic conversations — all powered by GPT-4 and Stable Diffusion.
This project was built to deepen my understanding of:

Integrating Large Language Models (LLMs) into real-world applications
Building production-grade RESTful APIs with Spring Boot
Connecting AI-generated content (text + images) into a seamless UI


✨ Features

🤖 AI Profile Generation — Dynamically generates realistic user profiles using GPT-4
🖼️ AI Profile Images — Custom profile pictures generated via Stable Diffusion
💬 AI Chatbots — Each profile has a personalized conversational AI for realistic interactions
📱 Responsive UI — Built with React.js for a smooth, mobile-friendly experience
🔗 15+ RESTful APIs — Robust backend APIs managing 500+ user profiles
🗄️ MongoDB Integration — Efficient NoSQL data storage for profiles and conversations


🛠️ Tech Stack
LayerTechnologyBackendJava, Spring Boot, REST APIsFrontendReact.js, JavaScript, HTML, CSSDatabaseMongoDBAI - TextOpenAI GPT-4AI - ImagesStable DiffusionDevOpsDocker, Git, GitHub

🏗️ Architecture Overview
├── backend/                  # Spring Boot Application
│   ├── controllers/          # REST API Controllers (15+ endpoints)
│   ├── services/             # Business Logic + GPT-4 Integration
│   ├── models/               # MongoDB Data Models
│   ├── repositories/         # MongoDB Repositories
│   └── config/               # App Configuration
│
├── frontend/                 # React.js Application
│   ├── components/           # Reusable UI Components
│   ├── pages/                # App Pages (Home, Chat, Profile)
│   └── services/             # API Integration Layer
│
└── docker-compose.yaml       # Container Orchestration

🚀 Getting Started
Prerequisites

Java 17+
Node.js 18+
MongoDB (local or Atlas)
OpenAI API Key
Stable Diffusion API Key

Backend Setup
bash# Clone the repository
git clone https://github.com/saransh123p/tinder-ai-app.git
cd tinder-ai-app

# Add your API keys in application.properties
# openai.api.key=YOUR_KEY_HERE

# Run the Spring Boot application
./mvnw spring-boot:run
Frontend Setup
bashcd frontend

# Install dependencies
npm install

# Start the development server
npm start
Using Docker
bash# Run everything with Docker Compose
docker-compose up --build

📡 API Endpoints
MethodEndpointDescriptionGET/api/profilesFetch all AI-generated profilesPOST/api/profiles/generateGenerate a new AI profileGET/api/profiles/{id}Get a specific profilePOST/api/chat/{profileId}Send a message to AI chatbotGET/api/chat/{profileId}/historyGet conversation historyDELETE/api/profiles/{id}Delete a profile

💡 Key Learnings
Working on this project helped me understand:

LLM Integration — How to craft effective prompts for GPT-4 to generate consistent, realistic persona data
AI + Backend — Connecting generative AI APIs within a Spring Boot service layer cleanly
Async Operations — Managing AI API response times without blocking the UI
NoSQL Design — Modeling flexible conversation and profile data in MongoDB
Full-Stack Flow — End-to-end data flow from React UI → Spring Boot → MongoDB → AI APIs


🙋‍♂️ Author
Saransh Padmaker
📧 saransh123p@gmail.com
🔗 LinkedIn
💻 GitHub

📄 License
This project is open source and available under the MIT License.
