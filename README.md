# Code-With-Enid-Data-Science
beginner-friendly machine learning demo using real-world data

## Online Music Store
Take the users age and gender 
Based on  the users profile recommends music albums the user can buy
Using machine learning to increase sales
The model is fed with sample data based on existing users
It learns patterns from data enabling it to make predictions

dataset - created using assumptions(made up data)
\ngender - 1 -> male, 0 -> female
\nmen 20 - 25 like HipHop
\nmen 26 - 30 like Jaz
\nmen and women 30+ like Classical music
\nwomen 20 - 25 like Dance music
\nwomen 26 - 30 like Acoustic music

# Steps
1. Import the Data
2. Clean the Data
3. Split the Data into Training/Test Sets
4. Create a Model
5. Train the Model
6. Make Predictions
7. Evaluate and Improve(EITHER BY CHANGING ALGORITHM OR FINE TUNE MODEL (HYPER PARAMETERS?))

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


# Preparing the data
Cleaning:
Removing duplicates/ null values/ incomplete values

# Training a model
Create instance of imported models class
Using the fit method -> model.fit(input_data, output_data)

# Prediction
Using the predict method -> model.predict([[ele1 input], [ele2 input]]) -> takes a 2d array outer array and each array inside is in element - input set

# Measuring Accuracy
There needs to be a training and testing set - using train_test_split from sklearn.model_selection
70% data - training, 20-30% - testing
- train_test_split(input_data,output_data,test_size=size) -> returns a tuple that you can unpack

- train using the training data
  model.fit(input_train,output_train)

- make predictions using the test data 
  model.predict(x_test)

- then confirm predictions with actual test data using accuracy_score from sklearn.metrics
  accuracy_score(expected values, predicted values) -> returns accuracy score between 0-1 * 100 = %


:- each time you split the data -> you might get a different accuracy score (train_test_split randomly splits data)


::- the more data you give the model and the cleaner the data is -> the better the result


# Model Persistence - Persisting a model