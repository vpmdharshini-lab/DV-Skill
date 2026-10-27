# Week 9 - House Sales Data Analysis 

##  Project Overview
This project focuses on analyzing house sales data using Python. It uses the King County house sales dataset to explore the data and extract date-related information.

##  Objectives
- Load house sales data using Pandas.
- Explore the dataset structure and columns.
- Convert the sale date into a datetime format.
- Extract year, month, day, hour, minute, and second from the sale date.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

##  Dataset
**Dataset:** `kc_house_data.csv`

The dataset contains house sales information. The CSV file must be available in the correct path to run the project.

## Features
- Display the first and last five rows.
- Check dataset information and dimensions.
- View column names.
- Convert the `date` column to datetime format.
- Create new columns:
  - `sale_year`
  - `sale_month`
  - `sale_day`
  - `sale_hour`
  - `sale_minute`
  - `sale_second`

##  How to Run
1. Download or clone this repository.
2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Place `kc_house_data.csv` in the appropriate location.
4. Update the CSV file path in the Python code if necessary.
5. Run `house_sales.py` or open it in Google Colab.

##  Expected Output
- Dataset preview
- Dataset information and shape
- Column names
- Converted date values
- Extracted sale date and time components
