Fundamental of data analytics


OVERVIEW
This Python script analyzes the Iris dataset using the pandas library for data manipulation and matplotlib/seaborn for data visualization. The analysis includes generating summary statistics, creating histograms for individual features, and producing pair plots for each species.

PREREQUISITES

Python 3.x
pandas
matplotlib
seaborn
Instructions


Ensure the required Python packages are installed. You can install them using the following:


pip install pandas matplotlib seaborn



Download the Iris dataset (CSV file) and update the file path in the script:



data = pd.read_csv('C:\\Users\\fifoa\\Downloads\\IRIS (1).csv')


Run the script:

python iris_analysis.py



This will generate summary statistics and visualizations for the Iris dataset.

Script Breakdown
1. Reading and Cleaning the Data
The script reads the Iris dataset from a CSV file and renames the columns for better readability.

2. Summary Statistics
Summary statistics are generated for each feature (sepal length, sepal width, petal length, and petal width) using the describe() function.

3. Histograms
Histograms are created for each feature and saved as PNG files (sep_len.png, sep_wid.png, pet_len.png, pet_wid.png).

4. Pair Plots
Pair plots are generated for each species separately (setosa_df, versicolor_df, virginica_df) and for all species combined, using seaborn.

5. Grouping and Counting
The script uses the groupby function to count the occurrences of each species in the dataset.

Outputs
Summary statistics are saved in iris_summary_stats.txt.
Histograms are saved as PNG files.
Pair plots are displayed or saved based on the species.


