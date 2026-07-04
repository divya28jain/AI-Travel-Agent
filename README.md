"# AI-Travel-Agent" 

# 🌍 AI Travel Planner

An AI-powered travel planning application that generates personalized travel itineraries by combining real-time flight information with AI-driven destination research, hotel recommendations, restaurant suggestions, and customized travel plans.

Built using **Streamlit**, **Gemini AI**, **Agno Agents**, and **SerpAPI**, the application helps users plan complete trips based on their destination, travel preferences, budget, and interests.

---

## 🚀 Features

- ✈️ Fetches the top cheapest flights using Google Flights (SerpAPI)
- 🤖 AI-powered destination research using Gemini
- 🏨 Recommends hotels and restaurants based on user preferences
- 🗺️ Generates a personalized multi-day travel itinerary
- 💰 Supports multiple budget options (Economy, Standard, Luxury)
- 🎭 Multiple travel themes
  - Couple Getaway
  - Family Vacation
  - Adventure Trip
  - Solo Exploration
- 🛂 Travel essentials checklist
- 🎒 Packing checklist
- ✈️ Flight booking links
- 📱 Interactive Streamlit interface

---

# 🖥️ Application Preview

## Home Page

![Home](images/home.png)

---

## Travel Preferences

![Preferences](images/preferences.png)

---

## Generated Travel Plan

![Results](images/results.png)

---

# 🏗️ System Architecture

```
                         User

                           │

                    Streamlit Frontend

                           │

        ┌──────────────────┼──────────────────┐
        │                  │                  │

  Flight Search      Research Agent     Hotel Agent
   (SerpAPI)         (Gemini + Agno)   (Gemini + SerpAPI)

        └──────────────────┼──────────────────┘
                           │

                    Planner Agent

                           │

             Personalized Travel Plan
```

---

# 🤖 AI Agent Workflow

### 🔍 Research Agent

Responsible for

- Destination research
- Tourist attractions
- Culture
- Climate
- Safety tips
- Activity recommendations

---

### 🏨 Hotel & Restaurant Agent

Responsible for

- Hotel recommendations
- Restaurant suggestions
- Nearby attractions
- User preference matching

---

### 🗺️ Planner Agent

Responsible for

- Multi-day itinerary generation
- Cost estimation
- Travel scheduling
- Transportation suggestions

---

# ⚙️ Tech Stack

### Frontend

- Streamlit

### AI

- Google Gemini 2.5 Flash
- Agno AI Agents

### APIs

- Google Flights (SerpAPI)

### Backend

- Python

### Libraries

- Streamlit
- Agno
- Google GenAI
- SerpAPI
- python-dotenv

---

# 📂 Project Structure

```
travel-planner/

│── travelagent.py
│── requirements.txt
│── .env.example
│── README.md
│── images/
│     ├── home.png
│     ├── preferences.png
│     └── results.png
```

---

# ⚡ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/ai-travel-planner.git

cd ai-travel-planner
```

Create a virtual environment

```bash
python -m venv venv
```

Activate the environment

Windows

```bash
venv\Scripts\activate
```

Linux / Mac

```bash
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file

```env
GOOGLE_API_KEY=YOUR_GOOGLE_API_KEY

SERPAPI_KEY=YOUR_SERPAPI_KEY
```

---

# ▶️ Run the Application

```bash
streamlit run travelagent.py
```

---

# 💡 How It Works

1. User enters

- Departure Airport
- Destination Airport
- Travel Dates
- Budget
- Travel Theme
- Activity Preferences

2. Google Flights API fetches the cheapest flights.

3. Research Agent gathers destination insights.

4. Hotel Agent recommends hotels and restaurants.

5. Planner Agent combines all information and generates a personalized itinerary.

6. Results are displayed with flight options, hotel recommendations, restaurants, and a complete travel plan.

---

# ✨ Future Improvements

- 🌦️ Weather integration
- 🗺️ Interactive maps
- 💬 Conversational travel assistant
- 💾 Save previous itineraries
- ❤️ Wishlist/Favorites
- 📄 PDF itinerary download
- 🌍 Multi-language support
- 💳 Travel budget tracker
- 📱 Mobile responsive UI
- 🔐 User Authentication

---

# 📈 Challenges

- Handling multiple API integrations
- Managing API compatibility across library versions
- Optimizing response time from multiple AI agents
- Prompt engineering for itinerary generation
- Secure API key management using environment variables

---

# 📚 Learning Outcomes

- Building AI-powered applications using LLMs
- Working with multi-agent AI systems
- API integration
- Prompt engineering
- Streamlit application development
- Environment variable management
- AI workflow orchestration

---

# 👩‍💻 Author

**Divya Jain**

B.Tech Computer Science & Engineering

Jaypee University of Engineering & Technology

GitHub: https://github.com/yourusername

LinkedIn: https://linkedin.com/in/yourprofile

---

⭐ If you found this project useful, consider giving it a star.
