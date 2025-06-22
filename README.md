# 🕵️‍♀️ Ad Finder – Contextual Advertising Search Platform

Ad Finder is a web application built with **Python**, **Django**, **Tailwind CSS**, and **BeautifulSoup**, designed to help identify advertising tags relevant to the content of any webpage URL you submit. The platform allows you to match common keywords from a webpage with predefined advertising tags stored in the Django admin portal.

---

## 🚀 Features

- 🔎 **URL Search Bar** — Paste any webpage URL and extract its meaningful text content.
- 🧠 **Keyword Extraction** — Uses `RAKE` (Rapid Automatic Keyword Extraction) to find relevant keywords.
- 📑 **Tag Matching** — Compares extracted keywords with tags saved in the Django Admin Panel.
- 🧵 **Tailwind CSS Styling** — Clean, responsive UI using Tailwind CSS.

---

## 🛠️ Tech Stack

- **Backend**: Python, Django
- **Frontend**: Tailwind CSS, HTML
- **Web Scraping**: BeautifulSoup
- **Keyword Analysis**: RAKE (`rake_nltk`)

---

## 📸 Screenshot

![Ad Finder Screenshot]
![image](https://github.com/user-attachments/assets/7de4e9ae-3402-4fe9-9a6c-d454f1477eee)
![image](https://github.com/user-attachments/assets/9057dc25-7cf5-4832-ba72-465d92afdafe)


---

## ⚙️ How It Works

1. User enters a **webpage URL** in the search bar.
2. The app scrapes the page’s content using **BeautifulSoup**.
3. Extracts meaningful keywords using **RAKE (nltk)**.
4. Compares these keywords against **predefined ad tags** in your Django database.
5. Displays any **matching ad tags** found in the content.

---

## 🧰 Installation

```bash
git clone https://github.com/your-username/ad-finder.git
cd ad-finder
python -m venv env
source env/bin/activate  # or env\Scripts\activate on Windows
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
