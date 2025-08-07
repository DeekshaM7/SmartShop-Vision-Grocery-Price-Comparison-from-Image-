# SmartShop-Vision-Grocery-Price-Comparison-from-Image-
Helps users shop smart by showing lowest prices per item across platforms in one view. 

## 📌 Project Objective

To help users shop smarter by providing a **side-by-side price comparison** for each item in their grocery list based on the latest online prices.

---

## 🔧 Tech Stack

| Component         | Tools/Tech Used                    |
|------------------|------------------------------------|
| OCR              | Tesseract, OpenCV                  |
| Web Scraping     | BeautifulSoup, Selenium (or APIs)  |
| Backend          | Python, Flask (or Django)          |
| Frontend         | HTML/CSS/JS or React               |
| Data Cleaning    | Python (regex, fuzzy matching)     |
| Deployment       | Heroku / Render / AWS (optional)   |

---

## 🚀 Features

- Upload a grocery list image (printed/handwritten)
- Automatic text extraction using OCR
- Real-time price scraping from multiple platforms
- Display of price comparison table with product links
- (Optional) Price drop notifications

---

## 📁 Folder Structure
smartshop-vision/
├── backend/
│ ├── app.py
│ ├── ocr/
│ │ └── ocr_processor.py
│ ├── scraping/
│ │ ├── amazon_scraper.py
│ │ ├── bigbasket_scraper.py
│ │ └── jiomart_scraper.py
│ ├── utils/
│ │ ├── preprocessing.py
│ │ ├── normalizer.py
│ │ └── fuzzy_match.py
│ └── requirements.txt
│
├── frontend/
│ ├── public/
│ └── src/
│ ├── components/
│ ├── pages/
│ ├── App.js
│ └── index.js
│ └── package.json
│
├── samples/
│ ├── sample_grocery_lists/
│ └── test_outputs/
│
├── docs/
│ ├── presentation.pdf
│ ├── report.pdf
│ └── architecture_diagram.png
│
├── README.md
└── .gitignore
