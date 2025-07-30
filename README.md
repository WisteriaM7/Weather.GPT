# 🌦️ Weather GPT — Your AI-Powered Weather Companion

Welcome to **Weather GPT**, a smart and conversational weather assistant powered by n8n automation and cutting-edge AI. Whether you want a quick weather update or to chat about the climate, this system’s got you covered — seamlessly blending live data with natural language understanding.

---

## 🚀 What’s Inside?

Weather GPT is a duo of dynamic workflows, working together like sunshine and clouds:

### 1️⃣ WeatherAgent.json — The Weather Fetcher & Summarizer ![Weather Agent n8n Workflow](https://github.com/WisteriaM7/Weather.GPT/blob/main/WeatherAgent%20n8n%20Workflow.png)
Your go-to for real-time, localized weather info, transformed into easy-to-understand, friendly summaries.

**How it works:**
- You specify a city (default: New York).
- It taps into OpenWeatherMap for fresh data.
- Ollama’s llama3.2 model spins that data into a cozy, human-like weather briefing.
- Voilà! You get the scoop in plain language, ready to inspire your day.

**Example output:**  
> *“In New York, it's currently 18°C with 65% humidity and partly cloudy skies. A light jacket is recommended if you're heading outside.”*

---

### 2️⃣ Weather Agent.json — The Chatty AI Weather & Knowledge Agent  ![Weather Agent n8n Workflow](https://github.com/WisteriaM7/Weather.GPT/blob/main/Weather%20Agent%20n8n%20Workflow.png)
Chat with it like a friend. Ask about weather, temperature, humidity — or even throw in some general trivia questions.

**Features:**
- Natural, flowing conversations with memory to keep context.
- Calls the WeatherAgent workflow when weather questions pop up.
- Consults Wikipedia for everything else you’re curious about.
- Powered by Ollama’s llama3.2 for smooth, human-like replies.

---

## 🔧 How to Use

1. **Import** both `WeatherAgent.json` and `Weather Agent.json` into your n8n environment.  
2. **Set up** your credentials:  
   - OpenWeatherMap API key (for weather data)  
   - Ollama API access with the llama3.2 model (for AI responses)  
3. **Start chatting**! Trigger the chat agent or call the workflows directly as your needs dictate.

---

## 🗂️ Included Files

- `WeatherAgent.json` — Weather data fetch & summarization  
- `Weather Agent.json` — Conversational AI agent for weather & general knowledge

---

## 🧩 System Architecture at a Glance

User (chat)
│
▼
Weather Agent (chat workflow)
│
├─► Wikipedia (for general knowledge)
│
└─► WeatherAgent (for weather queries)
│
└─► OpenWeatherMap + Ollama LLM (llama3.2)


---

## ⚙️ Requirements

- n8n automation platform  
- OpenWeatherMap API key  
- Ollama API access (llama3.2 model)  

---

## 📜 License

This project is licensed under the MIT License.  
See the [LICENSE](./LICENSE) file for details.

---

# Ready to Bring Weather to Life?

Dive in and let Weather GPT turn raw data into meaningful conversation — because weather talk should feel like a breeze. 🌤️
