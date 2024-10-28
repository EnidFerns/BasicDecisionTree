# Code-With-Mosh-Data-Science
beginner-friendly machine learning tutorial using real-world data


# Steps
1. Import the Data
2. Clean the Data
3. Split the Data into Training/Test Sets
4. Create a Model
5. Train the Model
6. Make Predictions
7. Evaluate and Improve(EITHER BY CHANGING ALGORITHM OR FINE TUNING HYPER PARAMETERS)

# Libraries for ML
- Numpy - provides multidimensional array
- Pandas - Data Analysis library - dataframes - 2D data structure (similar to Excel spreadsheet) - rows and columns
- MatPlotLib - 2D plotting library to create graphs and plots
- SciKit-Learn - provides algorithms

# Loading a dataset
pd.read_csv("filepath") - returns a dataframe object

some attributes and methods of the dataframe object
- shape -> (rows, columns)
- describe() -> basic info/statistics about the columns in the dataset - count(can show existence of missing values -> data cleaning [assign default values or eliminate the row]), mean, std - quantifies amount of variation, min, 25%, 50%, 75%, max

- values -> 2D array 

# Pandas Documentation /tutorial


# Jupyter Shotcuts
activated cell - command mode(blue) or edit mode(green)
ESC -> command mode:
- h -> all keyboard shortcuts
- b -> inserts new cell below
- a -> inserts new cell above
- dd -> delete cell

. tab -> shows attributes and methods of the object
cursor on the name of method + shift + tab -> tooltip describing what the method does and its params

ctrl + / -> comment