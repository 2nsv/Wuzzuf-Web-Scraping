# Wuzzuf Web Scraping

A Python-based web scraping project that uses **Selenium** to collect real job listings from **Wuzzuf** for multiple data and AI-related positions.

The project automates job searching, pagination, data extraction, and CSV export while handling missing experience information and removing duplicate listings.

---

## 🚀 Features

* 🔎 Search for multiple job positions automatically
* 📄 Scrape jobs from multiple result pages
* 🏢 Extract company and job information
* 📍 Extract job locations
* 💼 Extract required experience
* 🔗 Collect direct job URLs
* 🧹 Handle missing experience data
* ♻️ Remove duplicate jobs using `job_url`
* 📊 Export the final dataset to CSV

---

## 🔍 Search Positions

The scraper searches Wuzzuf for:

* Data Engineer
* Data Science
* AI Developer
* Machine Learning Engineer

---

## 📦 Data Collected

Each job listing contains:

| Field        | Description           |
| ------------ | --------------------- |
| `job_title`  | Job position title    |
| `company`    | Company name          |
| `location`   | Job location          |
| `experience` | Required experience   |
| `job_url`    | Direct URL to the job |

---

## 🔄 Project Workflow

```text
Start
  ↓
Open Wuzzuf
  ↓
Select Job Position
  ↓
Search for Jobs
  ↓
Load Search Results
  ↓
Scrape Job Information
  ↓
Move to Next Page
  ↓
Repeat for Multiple Pages
  ↓
Repeat for All Positions
  ↓
Remove Duplicate Jobs
  ↓
Save Data to CSV
  ↓
wuzzuf_jobs.csv
```

---

## 🛠️ Technologies

* **Python**
* **Selenium**
* **Pandas**
* **Chrome WebDriver**

---

## ⚙️ How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd <repository-folder>
```

### 2. Install dependencies

```bash
pip install selenium pandas
```

### 3. Run the scraper

```bash
python scraper.py
```

Make sure **Google Chrome** is installed. Selenium will use Chrome WebDriver to automate the browser.

---

## 📁 Project Structure

```text
Wuzzuf-Web-Scraping/
│
├── scraper.py
├── wuzzuf_jobs.csv
└── README.md
```

---

## 📊 Output

After running the scraper, the collected data is stored in:

```text
wuzzuf_jobs.csv
```

Example:

```text
job_title,company,location,experience,job_url
Data Engineer,Company Name,Cairo,2+ Yrs of Exp,https://...
```

---

## 🎯 Purpose

This project demonstrates practical experience with:

* Browser automation using Selenium
* Web scraping
* HTML element selection
* Pagination handling
* Data cleaning
* Duplicate removal
* Structured data extraction
* CSV data processing

---

## 👨‍💻 Author

**Anas Ahmed**

Data Engineering Student | Python | SQL | Data Engineering
