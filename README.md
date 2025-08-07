# SmartShop-Vision-Grocery-Price-Comparison-from-Image-
Helps users shop smart by showing lowest prices per item across platforms in one view. 

## Project Objective

To help users shop smarter by providing a **side-by-side price comparison** for each item in their grocery list based on the latest online prices.

---

## Tech Stack

| Component         | Tools/Tech Used                    |
|------------------|------------------------------------|
| OCR              | Tesseract, OpenCV                  |
| Web Scraping     | BeautifulSoup, Selenium (or APIs)  |
| Backend          | Python, Flask (or Django)          |
| Frontend         | HTML/CSS/JS or React               |
| Data Cleaning    | Python (regex, fuzzy matching)     |
| Deployment       | Heroku / Render / AWS (optional)   |

---

## Features

- Upload a grocery list image (printed/handwritten)
- Automatic text extraction using OCR
- Real-time price scraping from multiple platforms
- Display of price comparison table with product links
- (Optional) Price drop notifications

---

## Folder Structure
<pre> smartshop-vision/ ├── backend/ # Backend logic (Flask/Django, OCR, Scraping) │ ├── app.py # Main backend server entry point │ ├── ocr/ # OCR-related modules │ │ └── ocr_processor.py # Image preprocessing and text extraction │ ├── scraping/ # Web scraping logic for each platform │ │ ├── amazon_scraper.py │ │ ├── bigbasket_scraper.py │ │ └── jiomart_scraper.py │ ├── utils/ # Helper functions │ │ ├── preprocessing.py # Image cleaning utilities │ │ ├── normalizer.py # Normalize item names/units │ │ └── fuzzy_match.py # Fuzzy matching for item comparison │ └── requirements.txt # Python dependencies for backend ├── frontend/ # Frontend interface (React or HTML/CSS/JS) │ ├── public/ # Static assets │ └── src/ │ ├── components/ # Reusable UI components │ ├── pages/ # UI pages/views │ ├── App.js # React root component │ └── index.js # Entry point for rendering │ └── package.json # Frontend dependencies ├── samples/ # Sample images and test data │ ├── sample_grocery_lists/ # Input examples (handwritten/printed) │ └── test_outputs/ # OCR + price results for testing ├── docs/ # Project reports and resources │ ├── presentation.pdf │ ├── report.pdf │ └── architecture_diagram.png ├── README.md # Project overview and usage guide └── .gitignore # Git ignore rules </pre>


## Sample Workflow
1. User uploads grocery list image.
2. OCR extracts text: ["Amul Milk 1L", "Parle-G 200g"]
3. Scrapers/APIs fetch real-time prices.
4. UI displays comparison table:
| Item         | Amazon | BigBasket | JioMart |
| ------------ | ------ | --------- | ------- |
| Amul Milk 1L | ₹62    | ₹60       | ₹58     |
| Parle-G 200g | ₹25    | ₹22       | ₹23     |

## Team Members
1. Deeksha Mandal
2. Anshul Shinde
3. Dhruvi Ranwala
4. Mannan Singh Khanka
