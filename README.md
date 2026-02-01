# Trading Card Inventory Pricer

An automated tool that leverages the eBay Browse API to find current market "Sold" prices for trading cards stored in Google Sheets.

## Features
- Multi-Sheet Support: Iterates through all sheets in a Google Workbook (e.g., Bowman, Topps, Racing, MMA).
- Intelligent Search: Automatically formats search queries using player names, card numbers, and years.
- Outlier Protection: Uses Z-Score statistical filtering to remove overpriced graded cards from raw card averages.
- Error Tracking: Generates a failed_searches.csv for any cards that couldn't be priced automatically.

## Setup Instructions

### 1. Requirements
Ensure you have Python 3.x installed. This project uses a virtual environment (.venv) for dependency management.

### 2. Installation
Clone the repository and install the necessary libraries:
```bash
pip install requests pandas gspread oauth2client scipy python-dotenv