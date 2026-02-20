# IntelliSQL: Intelligent SQL Querying with Gemini Pro

IntelliSQL is a revolutionized database querying tool that bridges the gap between natural language and structured data. By leveraging Google's Gemini Pro model, it allows non-technical users to extract insights from a SQLite database using plain English.

## 🚀 Features

- **Text-to-SQL Translation:** Converts English questions into precise SQL queries using LLMs.
- **Regex Sanitization:** A custom logic layer that cleans AI responses to ensure only valid SQL is executed.
- **Interactive Dashboard:** A professional Streamlit interface with dark-mode support and sidebar navigation.
- **Secure Configuration:** API keys are managed safely via `.env` files and `python-dotenv`.
- **Real-time Results:** Instant rendering of database records in structured data tables.

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **Backend**: Python, Google Generative AI SDK
- **Database**: SQLite3
- **AI Model**: Gemini Pro

## 📂 Project Structure

```text
SQL-LLM/
├── .env                            # Secure API Key storage
├── app.py                          # Streamlit UI & AI Logic
├── data.db                         # SQLite Database
├── requirements.txt                # Project Dependencies
└── sql.py                          # DB Engineering & Seeding
```

## ⚙️ Setup & Installation

**1. Clone the Repository:**
```bash
git clone <repository_url>
cd SQL-LLM
```

**2. Set up Environment:**
```bash
python -m venv .venv
# On Windows:
.venv\Scripts\activate
# On Mac/Linux:
source .venv/bin/activate

pip install -r requirements.txt
```

**3. Configure API Key:**
Create a `.env` file in the root directory and add your key:
```plaintext
GOOGLE_API_KEY="your_google_gemini_api_key"
```

**4. Initialize Database:**
Run the following command to generate the dummy database:
```bash
python sql.py
```
*Note: This will create `data.db`.*

**5. Run Application:**
```bash
streamlit run app.py
```

## Team ID: **LTVIP2026TMIDS65923**

## 👥 Team Members

1. **CHODA DURGA BHAVANI**
2. **SRIHARI DEVALLA**
3. **MANIKANTA GILLA**
4. **PAVANKUMAR HANUMANTHU**

## ⚠️ Known Issues

- Occasional hallucinations on complex multi-table joins if not specified in the schema.
- Requires an active internet connection to reach the Gemini API.
