# 🌾 Bharat Farming Assistant AI

An **AI-powered smart farming assistant** designed to help farmers make better decisions about crops, soil, weather, markets, government schemes, and farming practices.

The application combines a web-based dashboard with AI-powered assistance and agriculture-related information to provide farmers with useful, easy-to-understand recommendations.

---

## 🚀 Features

### 🤖 AI Farming Assistant

* AI-powered farming guidance
* Natural-language interaction
* Answers agriculture-related questions
* Provides recommendations and suggestions for farming activities

### 🌱 Soil Information

Provides information about different soil types, including:

* Suitable crops
* Fertilizer recommendations
* Organic soil improvement methods
* Soil-specific farming guidance

Supported soil types include:

* Alluvial Soil
* Black Cotton Soil
* Red Soil
* Laterite Soil
* Sandy Soil
* Clay Soil
* Loamy Soil

### 🌾 Crop Assistance

* Crop-related recommendations
* Farming guidance
* Crop suitability based on soil information
* Agriculture decision support

### 🌦️ Weather Integration

Uses weather API services to provide weather-related information that can help farmers plan agricultural activities.

### 💰 Karnataka Mandi Prices

Includes mandi price information for selected agricultural commodities and locations.

Example locations:

* Bengaluru
* Mysuru
* Belagavi

Example crops:

* Tomato
* Onion
* Rice
* Ragi
* Maize
* Groundnut
* Sugarcane

### 🏛️ Government Schemes

Provides information about important agricultural schemes such as:

* PM-KISAN
* Pradhan Mantri Fasal Bima Yojana
* Kisan Credit Card
* PM Krishi Sinchayee Yojana
* Rashtriya Krishi Vikas Yojana
* Soil Health Card Scheme
* Paramparagat Krishi Vikas Yojana
* Pradhan Mantri Matsya Sampada Yojana

Each scheme includes information such as:

* Description
* Eligibility
* Application website
* Helpline information

### 🔐 User Authentication

The application provides:

* Login
* User registration
* Session-based authentication
* Password confirmation
* Password-strength indication

### 📊 Farmer Dashboard

A centralized dashboard provides access to the major farming assistance modules through a user-friendly interface.

---

## 🛠️ Technologies Used

| Technology   | Purpose                   |
| ------------ | ------------------------- |
| Python       | Core programming language |
| Flask        | Backend web framework     |
| HTML/CSS     | Frontend interface        |
| JavaScript   | Client-side interactions  |
| Groq         | AI-powered responses      |
| Requests     | API communication         |
| Gunicorn     | Production WSGI server    |
| Font Awesome | UI icons                  |

---

## 📂 Project Structure

```text
farming-assistant-main/
│
├── final.py
│       └── Main Flask application
│
├── requirements.txt
│       └── Python dependencies
│
└── requirement.txt
        └── Dependency list
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/farming-assistant-main.git
cd farming-assistant-main
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**Linux/macOS**

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 API Configuration

The application uses external APIs for AI, weather, and plant-related services.

For security, API keys should **not be hard-coded in the source code**.

Set them as environment variables:

```bash
GROQ_API_KEY=your_groq_api_key
OPENWEATHER_API_KEY=your_openweather_api_key
PLANT_ID_API_KEY=your_plant_id_api_key
SESSION_SECRET=your_secure_secret
```

For Windows PowerShell:

```powershell
$env:GROQ_API_KEY="your_api_key"
$env:OPENWEATHER_API_KEY="your_api_key"
$env:PLANT_ID_API_KEY="your_api_key"
$env:SESSION_SECRET="your_secret"
```

---

## ▶️ Running the Application

Run the Flask application using:

```bash
python final.py
```

The application can then be accessed through the local server shown in the terminal.

For production deployment with Gunicorn:

```bash
gunicorn final:app
```

---

## 🧠 How It Works

```text
             ┌─────────────────────────┐
             │        Farmer           │
             └────────────┬────────────┘
                          │
                          ▼
             ┌─────────────────────────┐
             │   Farming Assistant UI  │
             └────────────┬────────────┘
                          │
          ┌───────────────┼────────────────┐
          ▼               ▼                ▼
     ┌─────────┐    ┌──────────┐    ┌───────────┐
     │   Soil  │    │  Weather │    │   Mandi   │
     │  Data   │    │   API    │    │   Prices  │
     └────┬────┘    └────┬─────┘    └─────┬─────┘
          │              │                 │
          └──────────────┼─────────────────┘
                         ▼
                ┌─────────────────┐
                │   AI Assistant  │
                │      Groq       │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Recommendations │
                │   for Farmer    │
                └─────────────────┘
```

---

## 🎯 Objective

The main objective of Bharat Farming Assistant AI is to make agricultural information **accessible, understandable, and useful for farmers** through a single digital platform.

Instead of farmers having to search different sources for soil information, weather conditions, market prices, government schemes, and farming advice, the application brings these functionalities together.

---

## 🔮 Future Enhancements

Possible improvements include:

* 📡 IoT-based soil monitoring
* 🌡️ Real-time temperature and humidity sensors
* 🧪 NPK sensor integration
* 🌾 ML-based crop recommendation
* 📈 Crop yield prediction
* 🦠 Plant disease detection using computer vision
* 💧 Smart irrigation recommendations
* 📍 GPS-based farm location
* 📊 Advanced farming analytics
* 🌐 Multi-language support including Kannada
* 📱 Mobile application
* 🗄️ Database-based farmer and crop records
* 🔐 Secure password hashing and database authentication

---

## 🔒 Security Note

API keys and passwords should never be committed directly to GitHub.

Use environment variables or a `.env` file and add it to `.gitignore`:

```text
.env
venv/
__pycache__/
*.pyc
```

If an API key has already been exposed publicly, **revoke and regenerate it** before publishing the repository.

---

## 📜 License

This project is intended for educational, research, and agricultural technology development purposes.

---

## 👨‍💻 Project

**Bharat Farming Assistant AI**

An AI-driven platform for smarter and more accessible farming.
