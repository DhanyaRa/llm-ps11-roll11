# Roll No. 11 — MIT-ADT College Enquiry Chatbot

A Streamlit-based college enquiry chatbot developed for Generative AI Mini Project Problem Statement 11. It uses Google Gemini 2.5 Flash to answer questions about MIT-ADT University courses, fees, admission procedures, required documents and admission enquiries.

The chatbot retrieves information from `college_info.txt` and is instructed not to invent information that is missing from the supplied knowledge sheet.

## Technologies Used

- Python
- Streamlit
- Google Gemini 2.5 Flash
- Google GenAI Python SDK

## Project Files

- `app.py` — Streamlit application and conversation-history logic
- `college_info.txt` — MIT-ADT University information supplied to the model
- `requirements.txt` — Python dependencies
- `.gitignore` — excludes API secrets and local environments

## Setup and Installation

1. Install Python 3.10 or later.
2. Open a terminal in the project folder.
3. Create and activate a virtual environment (recommended).
4. Install the required packages:

   `pip install -r requirements.txt`

5. Create `.streamlit/secrets.toml` and add your Gemini API key:

   `GEMINI_API_KEY = "YOUR_GEMINI_API_KEY"`

   Alternatively, set the `GEMINI_API_KEY` environment variable. Never upload your actual API key to GitHub.

6. Start the application:

   `streamlit run app.py`

7. Open the local URL displayed in the terminal.

## Testing

The chatbot was tested using five sample enquiries:

1. What courses does MIT-ADT University offer?
2. What is the fee for B.Tech Computer Science?
3. How can I apply for admission?
4. What documents are required for admission?
5. Who can I contact for admission enquiries?

The chatbot was also designed to respond safely when information is unavailable in the supplied information sheet.

## Important Note

This is a student demonstration project and not an official MIT-ADT University service. Fee and admission details may change. Users should verify important information through the official university website and current admission handbook.

## Author

- Student: Dhanya Rao
- Roll Number: 11
- Class: LY B.Tech CSE AIA 4
- Academic Year: 2026–2027
- Problem Statement: 11
