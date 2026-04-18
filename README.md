# E-Commerce Price Tracker

Real-time price monitoring across Flipkart and Amazon India — tracks product prices, detects drops, and delivers structured data ready for alerts or dashboards.

## What it does
- Tracks prices for any product across Flipkart and Amazon India
- Detects price drops and percentage changes
- Handles dynamic JS-rendered product pages via Playwright
- Scheduled runs via cron — daily or hourly tracking
- Outputs to CSV, JSON, or Google Sheets

## Tech stack
- `Python 3.11` `Playwright` `lxml` `XPath` `Pandas` `Streamlit`

## Project structure

```text
ecommerce-price-tracker/
├── scrapers/
│   ├── flipkart_scraper.py    # Flipkart price extractor
│   └── amazon_scraper.py      # Amazon India price extractor
├── output/
│   └── price_history.csv
├── app.py                     # Streamlit demo
├── scheduler.py               # Cron-based scheduler
├── requirements.txt
└── README.md
```
## Sample output

| Product | Platform | Price (₹) | Previous (₹) | Change |
|---------|----------|-----------|---------------|--------|
| iPhone 15 128GB | Flipkart | 72,999 | 75,999 | -3.9% |
| iPhone 15 128GB | Amazon | 73,499 | 73,499 | 0% |
| Sony WH-1000XM5 | Flipkart | 24,990 | 27,990 | -10.7% |

## Live demo
🔗 Coming soon (Streamlit)

## Use cases
- Personal price drop alerts before buying
- Competitor pricing intelligence for e-commerce sellers
- Market research and trend analysis
