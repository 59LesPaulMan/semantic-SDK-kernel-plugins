# ✈️ Semantic Kernel Flight Booking Plugin

This project demonstrates how to build plugin-based AI capabilities using the [Microsoft Semantic Kernel SDK](https://github.com/microsoft/semantic-kernel) and Azure OpenAI GPT-4o. It supports flight search and booking functions using sample JSON data.

---

## 🚀 Features
- ✅ Search for flights by destination and date
- ✅ Book flights with confirmation
- ✅ Plugin functions are annotated with `@kernel_function`
- ✅ Fine-grained function control using `FunctionChoiceBehavior`
- ✅ Uses `flights.json` for simulated data

---

## 🧰 Tech Stack
- Python 3.10+
- Semantic Kernel SDK (`semantic-kernel[azure]`)
- Azure OpenAI (via Azure AI Foundry)
- dotenv for secure credential management

---

## 📁 Project Files

| File | Purpose |
|------|---------|
| `flight_booking_plugin.py` | Defines plugin functions for flight search/booking |
| `plugins.py` | Main application entry point |
| `flights.json` | Sample flight data |
| `.env.example` | Environment variable template (no secrets) |
| `requirements.txt` | Python dependencies |
| `output_1.png` | Screenshot of initial assistant interaction |
| `output_2.png` | Screenshot of booking response |

---

## 🛠️ Setup & Run

1. Create a virtual environment and install dependencies:
```bash
python -m venv labenv
source labenv/bin/activate  # or Activate.ps1 on Windows
pip install -r requirements.txt


PROJECT_ENDPOINT=https://<your-endpoint>.openai.azure.com/
PROJECT_KEY=sk-<your-api-key>
PROJECT_NAME=gpt-4o

python plugins.py