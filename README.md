# Rainfall Prediction Analysis

This project analyses and predicts rainfall patterns using historical weather data from Austin, Texas. The analysis is performed using Python libraries such as NumPy, Pandas, Scikit-learn, and Matplotlib.

## Dataset

The dataset used in this project is the `austin_weather.csv` file, which contains weather data for Austin, Texas. The dataset includes various features such as temperature, dew point, humidity, sea level pressure, visibility, wind speed, and precipitation.

## Data Preprocessing

The data preprocessing steps performed in this project are as follows:

1. **Loading the Dataset**: The `austin_weather.csv` file is loaded into a Pandas DataFrame using the `pd.read_csv()` function.

2. **Removing Unnecessary Columns**: Columns that are not required for the analysis, such as 'Events', 'Date', 'SeaLevelPressureHighInches', and 'SeaLevelPressureLowInches', are dropped from the DataFrame.

3. **Handling Missing Values**: Missing values represented by 'T' (trace) and '-' (missing) are replaced with 0.0.

4. **Saving the Preprocessed Data**: The preprocessed data is saved as a new CSV file named `austin_final.csv` for further analysis.

## Rainfall Prediction

The project uses a Linear Regression model from the Scikit-learn library to predict rainfall based on the provided weather features. The steps involved are as follows:

1. **Feature and Target Variable Separation**: The target variable ('PrecipitationSumInches') is separated from the feature variables (all other columns).

2. **Model Training**: A Linear Regression model is initialized and trained using the feature variables (X) and the target variable (Y).

3. **Visualization**: Two plots are generated:
  - **Precipitation Trend Graph**: A scatter plot showing the precipitation levels over time, with a specific day highlighted in green.
  - **Precipitation vs. Attributes Trend Graph**: A series of subplots depicting the relationship between precipitation and various weather attributes (temperature, dew point, humidity, sea level pressure, visibility, and wind speed).

## Usage

To run this project, follow these steps:

1. Clone the repository or download the project files.
2. Ensure you have installed Python and the required libraries (NumPy, Pandas, Scikit-learn, Matplotlib).
3. Place the `austin_weather.csv` file in the same directory as the project files.
4. Run the Jupyter Notebook or Python script containing the code.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
