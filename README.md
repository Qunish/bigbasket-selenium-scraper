# BigBasket Web Scraping and MongoDB Integration

This Jupyter Notebook (`bigbasket_lv.ipynb`) contains a Python script that utilizes the Selenium library to scrape product data from various categories on the BigBasket website. The scraped data is then stored in a MongoDB database for further analysis and use.

## Prerequisites

- Python 3.x
- Jupyter Notebook
- MongoDB installed and running

## Setup

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/bigbasket-web-scraping.git
   ```

2. Install the required Python packages using the following command:

   ```bash
   pip install selenium pymongo
   ```

3. Download the appropriate [chromedriver](https://sites.google.com/chromium.org/driver/) for your operating system and update the `DRIVER_FILE_PATH` variable in the script with the path to the downloaded driver.

## Usage

1. Open Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Open the `bigbasket_lv.ipynb` notebook.

3. Run the cells in the notebook sequentially to execute the web scraping and data extraction process.

## Configuration

- You can modify the `USER_AGENT_LIST` to include different user agents for simulating different web browsers.
- Adjust the URLs and collection names in the `collection_urls` list to scrape data from different categories.

## Script Structure

- `get_chrome_driver`: Function to set up a Chrome WebDriver for Selenium with customizable options.
- `get_product_data`: Placeholder function for scraping product data from the BigBasket website.
- Main Execution:
  - Establish a connection to the MongoDB database.
  - Fetch product URLs from the database.
  - Iterate through each product URL, scrape data, and upsert it into the MongoDB database.# bigbasket-selenium-scraper
