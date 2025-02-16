![Proporção para Github](https://github.com/anacartola/re-database/assets/136506553/0b753fe4-1b35-409e-b377-ac6ae9eab23c)
# Resident Evil Database Scraper

This project is a web scraping utility designed to collect and store character information from the Resident Evil Database website. The project uses Python libraries such as `requests`, `BeautifulSoup`, `tqdm`, and `pandas` to gather, process, and store the data in various formats.

ATTENTION: This project do not have complete clean data, as the purpose was testing webscrapping on beautifulsoup!

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)](https://github.com/anacartola/FeVias-Stellantis/actions)


## Project Overview

The Resident Evil Database Scraper automates the extraction of character details from the Resident Evil Database website. It collects basic character information and appearances, organizing the data into a structured format for analysis or further use.

## Features

- **Web Scraping**: Utilizes `requests` and `BeautifulSoup` to parse HTML content and extract character information.
- **Data Collection**: Gathers character details such as name, basic information, and appearances.
- **Data Storage**: Saves the collected data into multiple formats, including CSV, Parquet, and Pickle.
- **Progress Tracking**: Uses `tqdm` to provide a progress bar for the scraping process.

## Requirements

- Python 3.x
- `requests`
- `beautifulsoup4`
- `tqdm`
- `pandas`

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/residentevil-database-scraper.git
   cd residentevil-database-scraper
2. **Install dependencies:**:
   ```bash
   pip install requests beautifulsoup4 tqdm pandas
## Usage

1. **Run the Scraper**:
   ```bash
   python scrape_residentevil_database.py
2. **Access Data**:
The script saves the data in Dados_re.parquet and dados_Re.pkl formats. You can load these files using pandas for further analysis.

## Functions
- get_content(url): Fetches the content of a webpage.
- get_basic_infos(soup): Extracts basic information about a character from the HTML soup.
- get_aparicoes(soup): Extracts the appearances of a character from the HTML soup.
- get_personagem_infos(url): Combines information extraction functions to get complete character data from a given URL.
- get_links(): Retrieves all character page links from the main character listing page.

## Data Export
- CSV: Uncomment the to_csv line in the script to export data to a CSV file.
- Parquet: Data is saved in Parquet format for efficient storage and retrieval.
- Pickle: Data is serialized to a Pickle file for Python-specific storage.

### Contact

For questions or support, please contact [anacarolina.cartola@gmail.com](mailto:anacarolina.cartola@gmail.com).
