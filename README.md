## 🤖 💱 🔗 Automated Exchange Rate Data-Collection via API
  Objective of this project is to get the exchange rates on a daily basis. Rather than checking exchange rates manually every day, I have set up an automation process to pull the latest USD rates through an API and log them directly into Google Sheets.

---
### 🎯 Use Case:
  Instead of manually searching for exchange rates each day, I designed an automation in Make that fetches the latest USD exchange rates through an API and logs them into Google Sheets.

### 🔑 Approach:
- Replace repetitive tasks (search → copy → paste).
- Automate daily data collection with timestamps for accurate reporting.
- Build once, let it run automatically in the background.

### ⚙️ Workflow:
- 1️⃣ Trigger → Schedule the flow to run each morning.
- 2️⃣ API Call → Fetch USD exchange rates via HTTP GET request.
- 3️⃣ Google Sheets → Append results to a connected sheet.

### 📝 Execution Steps:
-  Create an account in  Make.com  (gmail account).
-  Add an HTTP Module to call the exchange rate API (e.g., app.exchangerate-api.com) via GET request and retrieve JSON data.
-  Set a Schedule → Run daily at 10 AM.
-  Send the data to Google Sheets (using the same Gmail account linked to Make.com) and map the headers as follows: Result, Base Code, Last Updation Date,
   Next Updation Date, Base Currency, Value, AED, SAR, OMR, INR, MYR, SGD.)
- Run the workflow and verify that the latest rates are automatically added as a new row.
  
### ✅ Outcome: 
- An Automated job runs every morning at 10 AM, fetching exchange rate data from the API and recording it in the Google Sheets
- Power BI automatically picks up the data → dashboards remain accurate and up to date.

<img width="1797" height="803" alt="image" src="https://github.com/user-attachments/assets/703d5cd5-9084-4368-b41f-9841889aee88" />

