# ITEC4305 Final Project

**This project is for ITEC 4305 and focuses on understanding data patterns in 2013 flight data.**

_This project particularly aids in predicting optimal departure times using 2013 flight data to find the pattern in total delays._

_Final Project | ITEC4305 | York University_

## File Structure

      ```ssh
      ITEC4305_Group_Project/
      .
      ├── .gitignore    # Ignoring Python/Jupyter temp files
      ├── Failed_Process.ipynb
      ├── feature_engineering.csv      # ignored (too large)
      ├── flights_EDA.csv
      ├── flights.csv
      ├── merged_flight_weather_data_knn.csv    # ignored (too large)
      ├── merged_flight_weather_data.csv     # ignored (too large)
      ├── project.ipynb
      ├── README.md
      ├── weather.csv
      └── xgb_grid_search_results.csv     # ignored (too large)

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/erictracc/ITEC4305_Group_Project.git

   ```

2. open the file `project.ipynb` and run a cell and choose your python environment or use bash to open `project.ipynb`.

   ```sh
   jupyter notebook project.ipynb

   ```

3. make sure to run the first cell with all of the `!pip install library_name` statements or you will run into errors when running the cells.

4. Each cell, if reran, should be reran in sequential order, top-to-bottom. Failing to do so can result in errors.

## Key Findings

- 6-9AM Flights that depart 1, 2 or 3 hours earlier can achieve a small decrease in total delay (~38% in a batch of 100 flights)
- Any flights after 2PM show little to no improvement in total delay if scheduled 1,2 or 3 hours earlier

Original Data Sources:

- for flights.csv: https://www.kaggle.com/datasets/monareyhanii/flights?resource=download
- for weather.csv: https://github.com/tidyverse/nycflights13/blob/main/data-raw/weather.csv
