# Weather-Forecast
Data Prediction About Weather Forecasting

🌦️ Weather Forecasting System - Hackathon Project

🧠 Problem Statement
Accurate weather forecasting is essential for agriculture, city planning, disaster management, and day-to-day activities. The objective of this project is to build a predictive weather forecasting system using historical weather data, machine learning, and real-time dashboards to help users access forecast data efficiently.

---

📁 Dataset Used

Dataset Name: ` weatherHistory.csv`
This dataset contains historical weather data including features like:

•	- `Temperature`
•	- `Humidity`
•	- `Wind Speed`
•	- `Wind Direction`
•	- `Pressure`
•	- `Precipitation`
•	- `Cloud Cover `
•	- `Visibility`
•	- `Daily Summary`
•	- `Timestamp`

---



🔧 Features Predicted
For a selected location, the following features are predicted:

•	- Temperature (°C)
•	- Humidity (%)
•	- Wind Speed (kph)
---

⚙️ Tech Stack

•	- **Backend:** Python (Jupyter Notebook)
•	- **Machine Learning:** Scikit-learn
•	- **Database:** Supabase (PostgreSQL backend)
•	- **Dashboard:** SupaBoard
•	- **Data Source:** Google Sheets (via `gspread`)

---

🧠 Machine Learning
•	- Model: RandomForestRegressor
•	- Trained separately for each feature using historical weather data
•	- Forecasts for a specific location and date



---







🔁 Automation Flow

`update_and_predict()` function:
1.	 Fetches the latest available historical data
2.	 Makes weather predictions using trained models
3.	 Can Predict temperature, wind speed and humidity as per Future Date
4.	 Appends the predictions into:
   - Supabase database table (`forecast`)
   - Google Sheet (for SupaBoard integration)

Scheduling:
•	- Runs every 10 seconds using `schedule` (customizable)

---

📊 Dashboard (SupaBoard)
1. Data from Google Sheets is added as a datasource to SupaBoard
2. Widgets are created for visualization:
   - Forecast Temperature (Line chart)
   - Forecast Humidity (Donut Chart)
   - Forecast Wind Speed (Line chart)
3. Dashboard auto-refreshes via the sync option or by manually clicking the refresh icon (↻)

If data appears stuck: Check that the Google Sheet has the latest entries. SupaBoard will fetch what's visible there.

---






✅ Achievements
•	- Built a working weather forecasting system
•	- Real-time predictions every 10s
•	- Visualized seamlessly on SupaBoard(https://app.supaboard.ai/dashboard/finaldashboard)
•	- Integrated with Supabase + Google Sheets
   - Google Sheet(https://docs.google.com/spreadsheets/d/1gswCQPle1BrD0NY2VspkwuwJHv6-gTrEcTCi84QX3Q0/edit?gid=0#gid=0)

---

🚀 Future Improvements
•	- Use LSTM models for better time-series predictions
•	- Add authentication for private dashboards
•	- Include more cities dynamically
•	- Deploy the system as a web app


---

👨‍💻 Contributors
•	- Om Pandey (Developer)
•	- Darshan Chhatbar (Developer)
•	- Aditi Jha (Developer)

---









📸 Screenshots

WINDSPEED

 ![image](https://github.com/user-attachments/assets/431296c6-3003-4f6c-b868-7af3f41e8836)



HUMIDITY

 ![image](https://github.com/user-attachments/assets/0d30e6d8-338f-4433-9e57-877cbc0d3a8e)






TEMPERATURE


![image](https://github.com/user-attachments/assets/719aa6d8-5903-4500-a0a6-a151de1431e2)
