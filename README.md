# Scraping-Emails-of-Amazon-sellers-from-Twitter-and-Facebook

## Project Overview
This project provides a Python-based solution to scrape and extract email addresses of Amazon sellers from social media platforms like Twitter and Facebook. Using the Twitter API and Selenium for Facebook, it automates the process of fetching user replies, extracting emails, and handling Facebook group members' data.

## Features
- **Twitter Integration:** Uses the Twitter API to fetch replies to a specific tweet and extract email addresses using regex.
- **Facebook Scraping:** Automates the scraping of Facebook group member profiles to collect emails.
- **Regex-Based Email Extraction:** Identifies and extracts email addresses from text using a regex pattern.
- **CSV Export:** Saves extracted emails to a CSV file for easy access.

## Technologies Used
- **Programming Language:** Python
- **APIs and Tools:**
  - Twitter API (via `tweepy`)
  - Selenium for Facebook automation
- **Libraries:**
  - `tweepy` for Twitter API interaction
  - `selenium` for web scraping
  - `re` for regex-based email extraction
  - `csv` for saving results

## Installation
### Prerequisites
- Python 3.8 or higher
- Twitter API credentials (Bearer Token, API Key, API Secret Key, Access Token, Access Token Secret)
- ChromeDriver installed for Selenium

## Usage
### Twitter Scraper
1. Open `Twitter_scraper.ipynb` or run the Python script for Twitter scraping.
2. Provide the Tweet ID and username for which replies should be fetched.
3. The script will:
   - Fetch replies to the given tweet.
   - Extract emails from the replies using regex.
   - Print and save the extracted emails to `scraped_emails.csv`.

### Facebook Scraper
1. Open `Facebook_scraper.ipynb` or run the Python script for Facebook scraping.
2. Provide the URL of the Facebook group members page.
3. The script will:
   - Scrape member profile links.
   - Attempt to extract emails from each profile.
   - Save the results (user ID and email) to `scraped_emails.csv`.

## Key Files
- `Twitter_scraper.ipynb`: Script for scraping emails from Twitter.
- `Facebook_scraper.ipynb`: Script for scraping emails from Facebook group members.
- `config.py`: Contains Twitter API credentials.
- `scraped_emails.csv`: File to store extracted email addresses.
