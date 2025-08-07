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

smartshop-vision/
├── backend/                       # Backend logic (Flask/Django, OCR, Scraping)
│   ├── app.py                    # Main backend server entry point
│   ├── ocr/                      # OCR-related modules
│   │   └── ocr_processor.py      # Image preprocessing and text extraction logic
│   ├── scraping/                 # Web scraping logic for each platform
│   │   ├── amazon_scraper.py
│   │   ├── bigbasket_scraper.py
│   │   └── jiomart_scraper.py
│   ├── utils/                    # Helper functions
│   │   ├── preprocessing.py      # Image preprocessing functions
│   │   ├── normalizer.py         # Unit normalization (e.g., 1L vs 1000ml)
│   │   └── fuzzy_match.py        # Item name matching using fuzzy logic
│   └── requirements.txt          # Python dependencies for the backend

├── frontend/                     # Frontend interface (React or plain JS)
│   ├── public/                   # Static assets (HTML, icons, etc.)
│   └── src/
│       ├── components/           # Reusable React components
│       ├── pages/                # Pages/views for the app
│       ├── App.js                # Main React app file
│       └── index.js              # Entry point for rendering React
│   └── package.json              # Frontend project dependencies and scripts

├── samples/                      # Sample input/output
│   ├── sample_grocery_lists/     # Example grocery list images
│   └── test_outputs/             # OCR and scraping result samples

├── docs/                         # Project documentation and reports
│   ├── presentation.pdf
│   ├── report.pdf
│   └── architecture_diagram.png

├── README.md                     # Project overview and usage guide
└── .gitignore                    # Files/folders to ignore in version control


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
