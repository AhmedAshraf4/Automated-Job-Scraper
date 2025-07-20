# 📄 Automated Job Scraper

A workflow automation that scrapes, cleans, and delivers personalized job listings via Telegram, tracks interview dates, and logs results to Google Sheets — fully automated with n8n.

---

## 🚀 Overview

This project helps job seekers by:
- ✅ Accepting job search queries through Telegram.
- ✅ Scraping job listings using Apify API.
- ✅ Cleaning and deduplicating job data.
- ✅ Sending curated job results back to Telegram.
- ✅ Tracking interview dates and sending reminders.
- ✅ Logging all jobs & interviews into Google Sheets for record-keeping.

All implemented as a no-code/low-code workflow on **n8n**.

---

## 🧰 Tech Stack

* **n8n** (workflow automation)
* **Telegram Bot API** (chat interface)
* **Apify API** (job scraping)
* **Google Sheets API** (data logging & tracking)
* **JavaScript & Node.js** (custom functions & logic)

---

## 🔗 Features

* 📬 **Telegram Bot**: Accepts `/start` and search queries.
* 🔍 **Job Scraper**: Queries Apify with user-specified job title.
* 🧹 **Data Cleaning**: Removes duplicates and irrelevant content.
* 📄 **Google Sheets Logging**: Saves jobs, company names, links, and interview dates.
* 🗓️ **Interview Reminders**: Sends Telegram reminders for scheduled interviews.

---

## 📦 Setup Instructions

### 1️⃣ Prerequisites

* [n8n](https://n8n.io/) installed (or use cloud version)
* A Telegram Bot Token ([create one here](https://core.telegram.org/bots))
* Apify API token ([create account](https://apify.com/))
* A Google Sheet set up for logging

---

### 2️⃣ Install / Import Workflow

* Clone this repo or download the workflow JSON file.
* Import the `.json` file into your n8n instance.
* Replace credentials with your own (Telegram, Apify, Google Sheets).

---

### 3️⃣ Environment Variables / Secrets

Configure your credentials and spreadsheet IDs in n8n’s **Credentials Manager**:

* Telegram Bot Token
* Apify API Token
* Google Sheet ID

---

### 4️⃣ Run

* Start your n8n instance:

  ```bash
  n8n start
  ```
* Trigger the bot by sending `/start` to your Telegram bot.

---

## 📜 Example Query

> User: `/start`
> Bot: “Enter the job title you want to search for...”
> User: `Data Scientist`
> Bot: sends back 10 curated job listings.
