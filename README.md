# Universal Analysis Repository

## Project Overview

This repository contains a Flask web application for universal analysis, which includes data scraped from Wikipedia on world population, top insurance companies in Canada, and the safest countries in the world. The data is stored in an SQLite3 database with different tables for each dataset.

## Setup Instructions
 
1. Clone the repository:
 
   ```bash
   git clone https://github.com/whatizee/Universal_analysis_python_project
   ```
 
2. Navigate to the project directory:
 
   ```bash
   cd Universal_analysis_python_project
   ```
 
3. Install the required dependencies:
 
   ```bash
   pip install -r requirements.txt
   ```
 
4. Run the Flask application:
 
   ```bash
   jupyter notebook Universal_analysis_project.ipynb
   ```
 
5. Open your web browser and go to [http://localhost:5000](http://localhost:5000) to access the web application.

# Group Project
This project is a Python-based web scraping, data processing, and website interaction project that collects data from wikipedia, 
and stores it in an SQLite database, and serves the data through a Flask-based website. The collected data is processed and cleaned before being stored, 
and users can interact with the data on the website.

## Requirements

For the successfull completion of this project, the following requirements are met:

1. **Data Collection**: Data is collected (legally) from 3 wikipedia websites namely, 'https://en.wikipedia.org/wiki/List_of_countries_and_dependencies_by_population','https://worldpopulationreview.com/country-rankings/safest-countries-in-the-world', 'https://en.wikipedia.org/wiki/List_of_Canadian_insurance_companies' through web scraping. Table data has been extracted from these websites.
## Data Description
 
### World Population Data
 
- Table Name: `world_population`
- Columns: `Country`, `Population`, `% of World`, `Date`, `Source`
 
### Top Insurance Companies in Canada Data
 
- Table Name: `insurance_companies_canada`
- Columns: `Company`, `Merged`, `Year`, `Notes`
 
### Top 20 Safest Countries Data
 
- Table Name: `safest_countries`
- Columns: `Country`, `Global Peace Index`
 


   Following modules has been imported for the collection of data

   -datetime
   -BeautifulSoup
   -pandas
   -request
   -sqlite3

   Initially stripping and replacing has been done to get the column headings. And later same procedure has been followed to obtain the contents of table.

   2. **Data Processing**: The collected data should be processed to clean and enhance it. Following actions has been taken to modify data as per our requirement.

   - normalizing text
   - extracting numerical values
   - formatting specific columns

   3. **Database**: The processed data should is stored in an SQLite database named 'Universal_analysis.db'. Both database creation and data insertion is done using the sqlite3 package.

   4. **Website Interaction**: Users will be to interact with the data through this website which is built using Flask. The website should have basic formatting and include the following pages:

   ## Website Structure
 
- **Home Page:**
  - Three buttons: 
    - Top Insurance Companies in Canada
    - Get Population Details
    - Top 20 Safest Countries
  - Additional buttons: 
    - Data Description
    - About
 
- **Get Population Page:**
  - Columns: `Country`, `Population`, `% of World`, `Date`, `Source`
  - Search button to search for a specific country.
 
- **Top Insurance Companies Page:**
  - Columns: `Company`, `Merged`, `Year`, `Notes`
 
- **Top 20 Safest Countries Page:**
  - Columns: `Country`, `Global Peace Index2023`,`Global Peace Index2022`
 
- **Data Description Page:**
  - Information about the data and its sources.
 
- **About Page:**
  - General information about the project and its purpose.

  5. **Repository Structure**: All project-related code is saved in a single GitHub repository. The repository structure includes the following files:

   - data_collection.ipynb
   - data_processing.ipynb
   - database.ipynb
   - Universal_analysis_app.ipynb
   - Readme.md
   - requirements.txt
   - about.html
   -data_description.html
   -Home.html
   -population_table.html
   -Top_20_peace_index.html
   -Top_ten_insurance_company.html
