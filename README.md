# expense-tracker
Local AI Expense Tracker

### 🚀 AI-Powered Local Expense Tracker

A fully automated, zero-cost expense tracking system that uses natural language processing to log daily spending. Built specifically to handle mixed-language inputs (English and Tagalog), the AI extracts financial data from simple chat messages and automatically archives it into a spreadsheet.

### 🛠️ Tech Stack

*   **Automation Engine:** n8n (Local Community Edition)
*   **AI Agent:** Google Gemini (Stable 3.6 Flash)
*   **Database:** Google Sheets (via Google Cloud OAuth2 API)

### ✨ Key Features

*   **Natural Language Processing:** Parses conversational text to extract Date, Amount, Category, and Description.
*   **Secure Credential Management:** API keys and OAuth secrets are safely isolated in n8n's encrypted vault, keeping the workflow code public-safe.
*   **Zero-Cost Architecture:** Runs entirely locally while utilizing free-tier AI and cloud database APIs.

### ⚙️ How to Setup

1.  Import the `expense_tracker_workflow.json` file into your local n8n instance.
2.  Add your Google Gemini API key to the n8n credential vault.
3.  Set up a Google Cloud Console project to generate an OAuth2 Client ID/Secret, and connect it to the Google Sheets node.
4.  Create a blank Google Sheet with the exact headers: `Date`, `Amount`, `Category`, and `Description`.
5.  Execute the workflow, open the n8n chat UI, and type an expense to test the automation!
