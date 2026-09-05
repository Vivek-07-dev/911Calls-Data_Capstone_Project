# 911 Calls-Data_Capstone_Project


## Summary
* **Objective:** An exploratory data analysis of 911 emergency call data to uncover temporal trends, common call reasons and identify peak times of call arrival.
* **Dataset:** Sourced from [Kaggle's Emergency Calls Dataset](https://www.kaggle.com/datasets/mchirico/montcoalert), containing attributes like latitude, longitude, description, zipcode, timestamp, and township.
* **Key Finding:** Emergency calls sharply increase during standard daytime hours (15:00 – 17:00) and heavily taper off on weekends(Sat/Sun) compared to weekdays.

## Tech Stack
* **Language:** Python 3.12
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## Dataset Features
The raw dataset includes the following core fields:
* `lat` / `lng`: Latitude and Longitude coordinates
* `desc`: Description of the Emergency Call
* `zip`: Zipcode
* `title`: Emergency Title (formatted as `Reason: Specific Code`)
* `timeStamp`: YYYY-MM-DD HH:MM:SS
* `twp`: Township
* `addr`: General Address

## How to Run the Project

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Vivek-07-dev/911Calls-Data_Capstone_Project.git
   ```

2. **Install required dependencies:**
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3. **Open the notebook:**
   Launch Jupyter Notebook and run `911-calls-analysis.ipynb`.

## Project Steps & Methodology
* **Feature Engineering:** Splitting the `title` column to create a new `Reason` categorical column (EMS, Fire, Traffic).
* **Time Series Extraction:** Extracting `Hour`, `Month`, and `Day of Week` from the `timeStamp` string column.
* **Exploratory Data Analysis:** Grouping, aggregation, and querying to find the top townships and zip codes for emergency dispatches.
* **Advanced Visualizations:** Utilizing Seaborn `countplot`, `lmplot`, `heatmap`, and `clustermap` to map call frequencies over hours and days.

## Key Insights & Visualizations
* **Top Reason for Calls:** **EMS (Emergency Medical Services)** consistently stands out as the most common overall reason for emergency dispatches, followed closely by Traffic accidents.
* **Temporal Patterns:** Call volumes show a predictable daily curve, peaking in the late afternoon and dropping drastically during early morning hours (0:00 – 6:00).
* **Weekly Trends:** Heatmaps reveal that emergency call distributions are lighter on Saturdays and Sundays compared to working weekdays.

## Author
* **Vivek Pal** - [GitHub Profile](https://github.com/Vivek-07-dev/) / [LinkedIn](https://www.linkedin.com/in/vivek-pal-498145314)
