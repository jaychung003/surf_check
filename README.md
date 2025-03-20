# 🌊 Surf Check

**Surf Check** is an intelligent assistant that helps surfers find the best time to hit the waves by integrating Google Calendar availability with real-time surf conditions from Surfline. 

## 🚀 Features
- 📅 **Google Calendar Integration**: Fetches free time slots for the next 72 hours.
- 🌊 **Surf Conditions Scraper**: Scrapes Surfline to gather wave height, conditions, and ratings for favorite surf spots.
- 🏄 **Personalized Surf Recommendations**: Suggests the best time to surf based on availability, wave conditions, and travel time.

## 🛠️ Installation

1. **Clone the repository**
   ```sh
   git clone https://github.com/jaychung003/surf_check.git
   cd surf_check

2. **Create and activate a virtual environment**
    ```sh
    python -m venv venv
    source venv/bin/activate  # Mac/Linux
    venv\Scripts\activate      # Windows

3. **Install dependencies**
    ```sh
    pip install -r requirements.txt

4. **Set up environment variables in .env**
   
   SERVICE_ACCOUNT_FILE: Path to your Google Calendar API service account JSON file. Details: https://developers.google.com/workspace/guides/create-credentials
   EMAIL_ADDRESS: Your gmail email address to access Google Calendar.
   OPENAI_API_KEY: your OpenAI api key

## 📊 How It Works
	1.	Check free time slots using the Google Calendar API.
	2.	Scrape Surfline for surf forecasts at selected spots.
	3.	Filter conditions based on user preferences (wave height, quality).
	4.	Match available time slots with ideal surf conditions, considering travel time.
	5.	Recommend the best surf session.

## 🏝️ Surf Spots Supported
	•	Linda Mar
	•	Linda Mar North
	•	North Ocean Beach

## 🔗 Dependencies
	•	crewai
	•	google-auth, google-api-python-client
	•	beautifulsoup4
	•	undetected-chromedriver
	•	pandas
	•	pytz

## 🏗️ Future Improvements
	•	Nearby surf spots detected based on user location
	•	Allow users to input preferred surf conditions.
    •	Automatically calculate estimated time to surf spots

Author: Jay Chung
