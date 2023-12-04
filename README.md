# Universal Analysis Repository

## Project Overview

This repository contains a Flask web application for universal analysis, which includes data scraped from Wikipedia on world population, top insurance companies in Canada, and the safest countries in the world. The data is stored in an SQLite3 database with different tables for each dataset.

## Setup Instructions

1. Clone the repository:

   ```bash
   git clone https://github.com/whatizee/Universal_analysis_project.git


cd universal-analysis

pip install -r requirements.txt

python Universal_analysis_app.ipynb


-----------------------------------------------------------------------------------------------------------------------



```markdown
# Universal Analysis Repository

## Project Overview

This repository contains a Flask web application for universal analysis, which includes data scraped from Wikipedia on world population, top insurance companies in Canada, and the safest countries in the world. The data is stored in an SQLite3 database with different tables for each dataset.

## Setup Instructions

1. Clone the repository:

   ```bash
   git clone https://github.com/whatizee/Universal_analysis_project.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Universal_analysis_project
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
  - Columns: `Country`, `Global Peace Index`

- **Data Description Page:**
  - Information about the data and its sources.

- **About Page:**
  - General information about the project and its purpose.

Feel free to contribute to the project by opening issues or submitting pull requests!
