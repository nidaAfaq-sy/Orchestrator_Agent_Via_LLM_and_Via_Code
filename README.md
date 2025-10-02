# 🧠 LLM Orchestrator with Multi-Agents

Ye project ek **multi-agent orchestration system** hai jo `Chainlit` aur Google **Gemini API** ka use karta hai.  
System user ke diye gaye topic ke liye automatically teen agents ko coordinate karta hai:

- **WebSearchAgent** → topic ke baare mein web se information collect karta hai  
- **DataAnalysisAgent** → collected information ko analyze karke insights banata hai  
- **WriterAgent** → insights ko ek formal aur structured report mein convert karta hai  

Orchestration ka kaam **Main Orchestrator Agent** karta hai jo in sab tools ko sequence mein chalata hai.

---

## 🚀 Features
- Multi-agent orchestration pipeline: **Search → Analysis → Report**
- Powered by **Gemini-2.0-Flash**
- Interactive chatbot interface with **Chainlit**
- Easily customizable for any topic (sirf climate-related nahi)

---

## 🛠️ Installation

1. **Clone repository**
```bash
git clone <your-repo-url>
cd <your-repo-folder>

Install dependencies

bash
Copy code
pip install -r requirements.txt
Environment setup
.env file banayein aur apna Gemini API key add karein:

ini
Copy code
GEMINI_API_KEY=your_api_key_here
▶️ Run the App
bash
Copy code
chainlit run app.py -w
Default UI: http://localhost:8000

💡 Example Usage
Chat box mein type karein:

nginx
Copy code
Make a report on AI in education
System automatically:

Web se information fetch karega

Usko analyze karega

Ek detailed formal report banayega

📂 Project Structure
bash
Copy code
.
├── app.py              # Main orchestrator code
├── requirements.txt    # Dependencies
├── .env                # API key config
└── README.md           # Documentation
