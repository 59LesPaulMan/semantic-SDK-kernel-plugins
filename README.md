# ✈️ Semantic Kernel Flight Booking Plugin

This lab project demonstrates how to build a plugin-enabled AI assistant using the [Microsoft Semantic Kernel SDK](https://github.com/microsoft/semantic-kernel) and Azure OpenAI.

## 🚀 Features
- Searches for available flights using sample data
- Books flights with confirmation messaging
- Uses Semantic Kernel `@kernel_function` decorators
- Supports plugin access filtering (e.g. search-only mode)

## 🧰 Tech Stack
- Python 3.10+
- Azure OpenAI GPT-4o via Azure AI Foundry
- Semantic Kernel SDK (`semantic-kernel[azure]`)
- Sample flight data from `flights.json`

## 📁 Files
| File | Description |
|------|-------------|
| `flight_booking_plugin.py` | Plugin with `search_flights()` and `book_flight()` |
| `plugins.py` | Main app that adds plugin to Semantic Kernel |
| `.env.example` | Template for Azure API keys and endpoint |
| `requirements.txt` | Python dependencies |
| `screenshots/` | Key screenshots from lab demo |

## 🛠️ Setup
```bash
python -m venv labenv
source labenv/bin/activate  # or Activate.ps1 on Windows
pip install -r requirements.txt