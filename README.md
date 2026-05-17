# Task 5: Automated Bulk Email Sender with Templates 🚀

A robust, CLI-based Python application designed to automate bulk email marketing and notification workflows securely. It supports dynamic personalization using templates, contact management via CSV/JSON, secure SMTP authentication, and automated transaction logging.

---

## 📺 Project Demo Video
A complete 1-minute walkthrough demonstrating the application's execution and functionality is available. 
- **Watch the Video:** `Check automated bulk mail demo video.mp4` 

*Note: For security and presentation purposes during the video demonstration, the App Password field utilizes a secure background fallback token mechanism to prevent exposing sensitive Google account credentials on screen.*

---

## ✨ Core Features

- **Secure SMTP Integration:** Direct connection via Gmail SMTP using Google App Passwords.
- **Bulk Email Processing:** Loads and parses recipient details dynamically from both `CSV` and `JSON` data sheets.
- **Smart Personalization:** Automatically replaces text placeholders like `{name}` and `{company}` with the recipient's real data.
- **Fail-Safe Retry Mechanism:** Automatically attempts to re-send a failed email up to **2 additional times** before skipping.
- **Bonus Capabilities Included:** - **File Attachments:** Native support to attach documents, PDFs, or images.
  - **HTML Templates:** Supports stylized rich-text HTML email delivery.
- **Transaction History Ledger:** Automatically maintains an `email_history.json` file tracking the exact timestamp, subject, and status (Sent/Failed) of every email.

---

## 🛠️ Requirements & Setup

This utility is built entirely using Python's native standard library suite, requiring **zero external dependencies** (no `pip install` required!).

### Prerequisites
- Python 3.x installed on your operating system.
- A Google Account with **2-Step Verification** enabled to generate an **App Password** for SMTP dispatch.

---

## 🚀 How to Run the Application

1. **Prepare Your Contacts Data:**
   Create a `contacts.csv` file in the root directory formatted like this:
   ```csv
   name,email,company
   Ali,ali123@gmail.com,Google
   Zainab,zainab456@gmail.com,Microsoft
