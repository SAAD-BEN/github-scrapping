# GitHub Scraper

This repository contains a Python script that allows you to scrape GitHub repositories based on specified criteria and extract relevant data. The script interacts with the GitHub API to fetch information about repositories created within a given date range.

## Prerequisites

Before running the script, ensure that you have the following dependencies installed:

- Python 3.x
- `requests` library
- `csv` library
- `pandas` library

You will also need a personal access token from GitHub to authenticate your requests to the GitHub API. Follow the instructions on [GitHub's Personal Access Token documentation](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to generate your access token.

## Usage

1. Clone the repository and navigate to the project directory.

2. Open the `scrape_repositories.py` file in a text editor or IDE.

3. Replace the placeholder values in the script with your GitHub username and personal access token:
```python
# Nom d'utilisateur de GitHub
username = 'YOUR_GITHUB_USERNAME'

# Jeton d'accès personnel
access_token = 'YOUR_PERSONAL_ACCESS_TOKEN'
```

4. Run the script in a Python environment.

5. Enter the requested information when prompted:
   - Start date (YYYY-MM-DD): Specify the start date for the scraping process.
   - End date (YYYY-MM-DD): Specify the end date for the scraping process.
   - Number of repositories per day: Specify the desired number of repositories to scrape per day.

6. The script will begin scraping the repositories based on the provided inputs. The data will be stored in a CSV file named according to the start date, end date, and repositories per day.

7. Once the scraping process is complete, a success message will be displayed, indicating that the repositories have been scraped and saved successfully.

## Analyzing the Data

To analyze the scraped data, you can make use of the provided Jupyter notebook (`analysis.ipynb`). This notebook utilizes the `pandas` library to read the CSV file and perform basic data analysis and exploration.

1. Ensure that you have Jupyter Notebook installed.

2. Open the Jupyter notebook file `analysis.ipynb`.

3. Run the notebook cells to load the data from the generated CSV file and perform preliminary analysis.

4. Modify and expand the notebook as needed to extract insights and visualize the data.

## Disclaimer

Please note that web scraping and data extraction from websites should be done responsibly and in compliance with the terms and conditions set by the website. Make sure to review and adhere to GitHub's usage policies and guidelines when using this script.

This repository is provided as a starting point, and you should customize it according to your specific needs and requirements.

Happy scraping and analyzing!
