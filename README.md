📚 Books Scraping Project

A complete web-scraping project that extracts book information—such as titles, prices, ratings, categories, and availability—from an online books website.
The project includes scraping scripts, structured output (CSV/JSON), optional database storage, and analysis-ready datasets.

🚀 Features

🔍 Automated scraping of all books across multiple pages

🏷️ Extracts title, price, rating, stock availability, category, and image URL

🧭 Pagination handling to scrape entire catalog

🧹 Cleaned & structured data output in CSV and JSON

🗄️ Optional storage in SQLite / MySQL / PostgreSQL

🧰 Modular, readable Python code (BeautifulSoup + Requests / Selenium)

📦 Ready for data analysis, ML pipelines, or dashboarding

🏗️ Project Structure
books-scraping-project/
│
├── src/
│   ├── scrape.py              # Main scraper
│   ├── utils.py               # Helper functions
│   ├── parser.py              # HTML parsing logic
│   └── database.py            # DB insertion (optional)
│
├── data/
│   ├── raw/                   # Raw HTML or JSON dumps
│   └── processed/books.csv    # Final cleaned dataset
│
├── notebooks/
│   └── analysis.ipynb         # Example EDA notebook
│
├── requirements.txt
└── README.md

🧪 Technologies Used

Python 3.8+

Requests – HTTP requests

BeautifulSoup4 – HTML parsing

Selenium (optional for JS-rendered sites)

pandas – data cleaning & exporting

SQLite / MySQL (optional)

▶️ How to Run the Project
1️⃣ Clone the repository
git clone https://github.com/yourusername/books-scraping-project.git
cd books-scraping-project

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Run the scraper
python src/scrape.py

4️⃣ View output

Processed data → data/processed/books.csv

Raw dumps → data/raw/

📊 Data Fields Collected
Field	Description
title	Book title
price	Price in site currency
rating	Rating (e.g., One–Five stars)
stock	Availability status
category	Book genre
product_page_url	Full URL
image_url	Book cover URL
📄 Example CSV Output
title,price,rating,stock,category,image_url
"A Light in the Attic",£51.77,Three,"In stock","Poetry","http://...jpg"
"Tipping the Velvet",£53.74,One,"In stock","Historical Fiction","http://...jpg"

⚙️ Customization

You can easily modify:

Base URL of the site

Fields extracted

Output file format

Database integration

Request frequency (to avoid blocking)
