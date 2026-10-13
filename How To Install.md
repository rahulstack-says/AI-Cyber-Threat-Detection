💻 System Requirements

The project can run on a normal personal computer.

Recommended:

Python 3.10+
RAM: 8 GB or more recommended
Storage: At least 5 GB free
Operating System: Windows / Linux / macOS

The project was also developed and tested on a system with limited RAM by using a reduced training dataset.

⚙️ Installation
1. Clone the Repository
git clone https://github.com/rahulstack-says/AI-Cyber-Threat-Detection.git
cd AI-Cyber-Threat-Detection
2. Create a Virtual Environment

Windows:

python -m venv .venv

Activate:

.venv\Scripts\activate

If PowerShell prevents activation, the environment's Python executable can be used directly.

3. Install Dependencies
pip install -r requirements.txt
4. Configure Generative AI

Create a local .env file:

GROQ_API_KEY=your_api_key_here

Do not upload the .env file to GitHub.

5. Run the Application
streamlit run app.py

Then upload a network-flow CSV file and click:

🔍 Detect Threats

☁️ Deploy on Streamlit Community Cloud

1. Upload the files from this flat package to the repository root. Keep `app.py`, `genai_analyzer.py`, both `.pkl` files and `requirements.txt` together in the root.
2. Open https://share.streamlit.io/ and sign in with GitHub.
3. Select the repository, branch and `app.py` as the main file.
4. Deploy the app and share the generated `streamlit.app` URL.

The `GROQ_API_KEY` is optional. If it is needed, add it in the app's Streamlit Secrets settings as:

```toml
GROQ_API_KEY = "your_api_key_here"
```

Never commit `.env`, `secrets.toml` or API keys to GitHub.
