# PandasAssignment

Q1. How do you load a CSV file into a Pandas DataFrame?

Ans - 
import pandas as pd
df = pd.read_csv(r'Path where the CSV file is stored\File name.csv')
print(df)

Q2. How do you check the data type of a column in a Pandas DataFrame?

Ans - df.dtypes

Q3. How do you select rows from a Pandas DataFrame based on a condition?

Ans - selecting_row = dataframe.loc[dataframe['Percentage'] > 80]

Q4. How do you rename columns in a Pandas DataFrame?

Ans - df.rename(columns = {'test':'TEST'}, inplace = True)

Q5. How do you drop columns in a Pandas DataFrame?

Ans - df.drop('new_col', axis=1)

# drop two columns

df.drop(['one_col','two_col'], axis=1)

Q6. How do you find the unique values in a column of a Pandas DataFrame?

Ans - df.B.unique()

Q7. How do you find the number of missing values in each column of a Pandas DataFrame?

Ans - df.isnull()

Q8. How do you fill missing values in a Pandas DataFrame with a specific value?

Ans -

# filling missing value using fillna() 
df.fillna(0)

Q9. How do you concatenate two Pandas DataFrames?

Ans - 

# append method
result = df1.append(df2)
display(result)

Q10. How do you merge two Pandas DataFrames on a specific column?

Ans - 

# using merge method
df2.merge(df1)

Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?

Ams - 
# using group
result = df.groupby('Courses').aggregate('sum')
print(result)

Q12. How do you pivot a Pandas DataFrame?

Ans - table = df.pivot(index='Country',columns='Year',values='Value')  
print(table)

Q13. How do you change the data type of a column in a Pandas DataFrame?

Ans - DataFrame.astype() method is used to cast pandas object to a specified dtype. This function also provides the 
      capability to convert any suitable existing column to a categorical type.

# converting all columns to string type
df = df.astype(str)
print(df.dtypes)


Q14. How do you sort a Pandas DataFrame by a specific column?

Ans - Pandas sort_values() method sorts a data frame in Ascending or Descending order of passed Column.

# Sort the rows of dataframe by 'Name' column
sort_df = df.sort_values(by = 'Name')

Q15. How do you create a copy of a Pandas DataFrame?

Ans - There are many ways to copy DataFrame in pandas. A simple way of assigning a dataframe object to a variable.

Syntax: DataFrame.copy(deep=True)

res = df.copy(deep=True)
print(res)

Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?

Ans - using loc

# filter dataframe
display(dataFrame.loc[(dataFrame['Salary']>=100000)

Q17. How do you calculate the mean of a column in a Pandas DataFrame?

Ans - Pandas dataframe.mean() function return the mean of the values for the requested axis. If the method is applied on a pandas dataframe object,
then the method returns a pandas series object which contains the mean of the values over the specified axis.


# Even if we do not specify axis = 0,
# the method will return the mean over
# the index axis by default
df.mean(axis = 0)

Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?

Ans - Pandas dataframe.std() function return sample standard deviation over requested axis.

# finding STD
df.std(axis = 0, skipna = True)

Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?

Ans - By using corr() function we can get the correlation between two columns in the dataframe.

Syntax:

dataframe[‘first_column’].corr(dataframe[‘second_column’])
# correlation between column 1 and column2
print(df['column1'].corr(df['column2']))

Q20. How do you select specific columns in a DataFrame using their labels?

Ans - 
# to select a column
result = df["City"]

# select multiple columns
result = df[["Name", "Age", "Salary"]]

Q21. How do you select specific rows in a DataFrame using their indexes?

Ans - 
# to select single row
result = df.loc["Stuti"]

# to select multiple rows
result = df.loc[["Stuti", "Seema"]]

Q22. How do you sort a DataFrame by a specific column?

Ans - Pandas sort_values() method sorts a data frame in Ascending or Descending order of passed Column.

# Sort the rows of dataframe by 'Name' column
sort_df = df.sort_values(by = 'Name')


Q23. How do you create a new column in a DataFrame based on the values of another column?

Ans - Next, use the apply function in pandas to apply the function - e.g.

df.apply (lambda row: label_race(row), axis=1)

or

# create a new column
df['Discounted_Price'] = df['Cost'] - (0.1 * df['Cost'])
 
Q24. How do you remove duplicates from a DataFrame?

Ans - Pandas drop_duplicates() method helps in removing duplicates from the Pandas Dataframe In Python.

df = pd.DataFrame(data)
  
display(df.drop_duplicates())

Q25. What is the difference between .loc and .iloc in Pandas?

Ans - The loc() function is label based data selecting method which means that we have to pass the name of the row or column 
which we want to select. This method includes the last element of the range passed in it, unlike iloc(). 
loc() can accept the boolean data unlike iloc().

# selecting cars with brand 'Maruti' and Mileage > 25
display(data.loc[(data.Brand == 'Maruti') & amp(data.Mileage & gt 25)])

# selecting range of rows from 2 to 5
display(data.loc[2: 5])

The iloc() function is an indexed-based selecting method which means that we have to pass an integer index in the method to 
select a specific row/column. This method does not include the last element of the range passed in it unlike loc(). 
iloc() does not accept the boolean data unlike loc().

# selecting 0th, 2th, 4th, and 7th index rows
display(data.iloc[[0, 2, 4, 7]])


