# Hydro - Smart Hydration Tracker

A web application that helps users track their daily water intake, set reminders, and maintain optimal hydration based on their BMI and local weather conditions.

## Features

- User registration and authentication
- BMI calculator with personalized water intake recommendations
- Daily water intake tracking with visual progress indicators
- Customizable water intake reminders with SMS notifications via Twilio
- Real-time weather integration to adjust hydration recommendations
- Streak tracking to motivate consistent hydration habits
- Responsive design for all devices

## Tech Stack

- Frontend: HTML, CSS, JavaScript
- Backend: Python Flask
- Database: SQLite (via SQLAlchemy)
- APIs: Twilio for SMS, OpenWeatherMap for weather data

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hydration-tracker.git
   cd hydration-tracker
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r backend/requirements.txt
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory with the following variables:
   ```
   TWILIO_ACCOUNT_SID=your_twilio_account_sid
   TWILIO_AUTH_TOKEN=your_twilio_auth_token
   TWILIO_PHONE_NUMBER=your_twilio_phone_number
   WEATHER_API_KEY=your_openweathermap_api_key
   ```

4. Run the application:
   ```bash
   python backend/app.py
   ```

5. Access the application at `http://localhost:5000`

## Usage

1. Create an account or log in
2. Fill out your profile information including weight, height, age, and gender
3. Calculate your BMI and recommended water intake
4. Set up reminders for drinking water throughout the day
5. Track your daily water intake by adding entries each time you drink
6. Monitor your hydration progress and build streaks

## Project Structure

```
hydration-tracker/
├── backend/
│   ├── app.py              # Main Flask application
│   └── requirements.txt    # Python dependencies
├── static/
│   ├── css/
│   │   └── styles.css      # Main stylesheet
│   ├── js/
│   │   ├── main.js         # Landing page JS
│   │   ├── auth.js         # Authentication JS
│   │   ├── dashboard.js    # Dashboard functionality
│   │   └── bmi-calculator.js # BMI calculator JS
│   └── images/             # Image assets
├── templates/
│   ├── index.html          # Landing page
│   ├── login.html          # Login page
│   ├── register.html       # Registration page
│   ├── dashboard.html      # Main user dashboard
│   └── bmi_calculator.html # BMI calculator page
└── README.md               # Project documentation
```

## License

This project is licensed under the MIT License.