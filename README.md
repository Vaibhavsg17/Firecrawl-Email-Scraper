# AI Email Scraper

## Overview

**AI Email Scraper** is an automated tool that scrapes team pages to extract structured information, such as team member names, positions, and emails. The tool uses **Firecrawl API** to perform web scraping, identifies key decision-makers, and saves the collected data into a CSV file.

This tool is useful for gathering contact details of professionals, particularly those in decision-making roles, by searching for team pages related to specific keywords, such as "real estate agents" or "marketing managers."

## Features

- **Automated Web Search**: Performs a web search using custom queries to find relevant team pages (e.g., "meet the team").
- **Data Extraction**: Extracts structured team member details such as first name, last name, position, location, and image URL.
- **Email Collection**: Collects email addresses where available. If an email is missing, it intelligently guesses the email based on a name and company domain.
- **Key Person Identification**: Only extracts information for key decision-makers, as identified by their roles.
- **CSV Export**: Outputs the scraped data in a CSV file for easy access and further processing.
  
## Use Cases

- **Real Estate Agencies**: Gather email addresses of real estate agents in specific locations.
- **Marketing Teams**: Collect contact information for marketing managers and other key team members in tech companies.
- **Company Teams**: Extract emails of executives and key personnel from company team pages.

## Installation

Install required libraries
```
pip install firecrawl-py pydantic pandas unidecode
```

Set up your Firecrawl API Key (first 300 credits are free)
```
export FIRECRAWL_API_KEY='your_api_key_here'
```
Add this line to your `.bash_profile` or `.zshrc` to make the setting persist across sessions.

## Usage
Update the `query` var to target the desired industry/location and run the script 
```
python app.py
```