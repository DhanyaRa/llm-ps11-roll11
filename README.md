# Roll No. 11 — College Enquiry Chatbot

A Streamlit chatbot for college course, fee and admission enquiries. It uses Gemini 2.5 Flash and answers only from `college_info.txt`.

## Files
- `app.py` — Streamlit application and chat-history logic
- `college_info.txt` — information sheet supplied to the model
- `requirements.txt` — Python dependencies
- `.gitignore` — excludes secrets and local environments

## Setup
1. Install Python 3.10 or later.
2. Open a terminal in this project folder.
3. Create and activate a virtual environment (recommended).
4. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Create `.streamlit/secrets.toml` and add:

   ```toml
   GEMINI_API_KEY = "YOUR_GEMINI_API_KEY"
   ```

   Alternatively, set the `GEMINI_API_KEY` environment variable. Never commit the key.

6. Start the app:

   ```bash
   streamlit run app.py
   ```

## Testing prompts
1. Which programmes are offered by the School of Computing?
2. What is the first-year Indian Resident fee for B.Tech CSE in 2026–27?
3. What is the published four-year total for B.Tech CSE?
4. What are the steps in the admission process?
5. What is the School of Computing admission coordinator's published contact number?
6. What is the hostel fee? (Expected behaviour: the bot says this information is not available in the supplied sheet.)

## Important
This is a student demonstration, not an official university service. Fee and admission details are time-sensitive. Verify them on the official university website. Update `college_info.txt` when official information changes.
