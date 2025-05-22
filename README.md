# Coffee Data Scraping Project

## Overview
This project analyzes high-rated coffee data from Coffee Review. It involves scraping coffee review data, cleaning it, and preparing it for analysis. The dataset contains information about coffee ratings, origins, roast levels, prices, and more.

## Files
- **[`scrape.ipynb`](scrape.ipynb)**: Web scraping script that collects coffee review data
- **[`cleaning.ipynb`](cleaning.ipynb)**: Data cleaning notebook that processes and transforms the raw data
- **[`top-rated-coffee.csv`](top-rated-coffee.csv)**: Raw coffee review data
- **[`top-rated-coffee-clean.csv`](top-rated-coffee-clean.csv)**: Cleaned and processed dataset

## Data Collection
The project scrapes coffee review data from [Coffee Review](https://www.coffeereview.com) using:
- Python's `requests` library to fetch web pages
- `BeautifulSoup` for HTML parsing
- Rate limiting to avoid overloading the server

## Data Features
The dataset contains information about 2,217 highly-rated coffees including:
- Coffee name
- Total score (typically ranging from 94-98)
- Roaster location
- Coffee origin (country or region)
- Roast level
- Agtron measurements (roast color measurements)
- Price

## Data Cleaning
The cleaning process includes:
- Converting score to numeric type
- Splitting Agtron values into ground and roast measurements
- Standardizing roast level descriptions
- Extracting origin country information
- Normalizing price data to per ounce
- Handling missing values

## Insights
The dataset provides insights into:
- Geographic distribution of coffee origins (Ethiopia, Colombia, Kenya, etc.)
- Price variations across regions and quality levels
- Relationship between roast levels and ratings
- Popular coffee varieties and processing methods

## Usage
To run the notebooks:
1. Install required libraries: `pandas`, `numpy`, `requests`, `beautifulsoup4`, `missingno`
2. Run [`scrape.ipynb`](scrape.ipynb) to collect new data or use the provided CSV files
3. Run [`cleaning.ipynb`](cleaning.ipynb) to process the data for analysis

## Next Steps
This cleaned dataset can be used for:
- Visualizing coffee trends
- Building recommendation systems
- Analyzing price-quality relationships
- Exploring regional coffee characteristics