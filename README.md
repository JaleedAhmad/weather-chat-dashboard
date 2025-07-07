```markdown
🌦️ Weather & Chat Dashboard

A real-time **weather monitoring dashboard** using a DHT11 sensor on Raspberry Pi, with an interactive chat interface powered by **Mistral AI**.

---

🛠️ Features

- 🌡️ Live temperature and humidity charts (updated every 15 seconds)
- 📈 Historical data table of recent sensor readings
- 💬 Chat interface to ask weather-related questions via Mistral API
- 🌓 Responsive, dark-themed UI (HTML, CSS, Chart.js)
- 🐍 Backend powered by Flask and Adafruit CircuitPython libraries

---

🖥️ Project Structure


weather-chat-dashboard/
├── diagrams/
│   ├── api\_structure.png
│   ├── hardware\_circuit\_diagram.png
│   ├── hardware\_workflow\_weather\_monitoring.png
│   └── software\_workflow\_iot\_system.png
├── templates/
│   └── index.html
├── static/
│   ├── style.css
│   └── script.js
├── app.py
├── requirements.txt
└── README.md

````


🔌 Hardware Setup

- Raspberry Pi (any model with GPIO pins)
- DHT11 Temperature & Humidity Sensor connected to GPIO4 (Pin 7)
- Proper wiring using [Adafruit DHT11 guide](https://learn.adafruit.com/dht)


 🗂️ System Diagrams

 📟 Hardware Circuit Diagram
![Hardware Circuit Diagram](diagrams/hardware_circuit_diagram.png)

 🛜 API Structure
![API Structure](diagrams/api_structure.png)

 🔄 Hardware Workflow
![Hardware Workflow](diagrams/hardware_workflow_weather_monitoring.png)

🧩 Software Workflow
![Software Workflow](diagrams/software_workflow_iot_system.png)

---

⚙️ Installation

Step 1: Clone the Repository
```bash
git clone https://github.com/JaleedAhmad/weather-chat-dashboard.git
cd weather-chat-dashboard
````

 Step 2: (Recommended) Create Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```

 Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

 Step 4: Add Your Mistral API Key

In `app.py`:

```python
MISTRAL_API_KEY = "your_api_key_here"
```

---

 🚀 Run the App

```bash
python app.py
```

Visit the app in your browser:
`http://<raspberry-pi-ip>:5050`

 Dashboard Tabs:

* **Dashboard:** Live temperature & humidity updates
* **Chat:** Ask weather-related questions to the AI assistant

---

 🗒️ Notes

* The Raspberry Pi must have GPIO access and required libraries installed.
* Sensor data updates every 15 seconds and stores the last 30 readings.
* Chat functionality uses the Mistral Medium Model API (internet required).

---

📜 License

MIT License

---

🙏 Acknowledgments

* [Adafruit CircuitPython DHT library](https://github.com/adafruit/Adafruit_CircuitPython_DHT)
* [Chart.js](https://www.chartjs.org/)
* [Mistral AI](https://mistral.ai/)

---

 ✍️ Author

Jaleed Ahmad
Weather Monitoring & Chat Dashboard
[GitHub](https://github.com/<JaleedAhmad>)

---

*Feel free to open issues or contribute to the project!*
