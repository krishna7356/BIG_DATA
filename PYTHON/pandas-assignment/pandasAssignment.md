# PandasAssignment

Q1. How do you load a CSV file into a Pandas DataFrame?
ans:to load csv file to pandas read_csv(filepath) we use
eg: df=pandas.read_csv('C:\Users\Krishna\OneDrive\Desktop\CheetSheet\model.csv')

Q2. How do you check the data type of a column in a Pandas DataFrame?
ans: Use the .dtype attribute to get the data type of a particular column in a Pandas dataframe.

Q3. How do you select rows from a Pandas DataFrame based on a condition?
ans: using loc[] or iloc[] we can select rows from pandas dataframe

Q4. How do you rename columns in a Pandas DataFrame?
ans:Renaming the columns in a Pandas Dataframe is by using the rename() function. This method is quite useful when we need to rename some selected columns because we need to specify information only for the columns which are to be renamed.
eg:rankings_pd = pd.DataFrame(rankings)

rankings_pd.rename(columns = {'test':'TEST'}, inplace = True)

Q5. How do you drop columns in a Pandas DataFrame?
ans:

- Drop a single column from the DataFrame:
  df = df.drop('column name',axis=1)
- Drop multiple columns from the DataFrame:
  df = df.drop(['column 1','column 2','column 3',...],axis=1)

Q6. How do you find the unique values in a column of a Pandas DataFrame?
ans: dataframe.column.unique()
eg:# Import pandas package
import pandas as pd

#create a dictionary with five fields each
data = {
'A':['A1', 'A2', 'A3', 'A4', 'A5'],
'B':['B1', 'B2', 'B3', 'B4', 'B4'],
'C':['C1', 'C2', 'C3', 'C3', 'C3'],
'D':['D1', 'D2', 'D2', 'D2', 'D2'],
'E':['E1', 'E1', 'E1', 'E1', 'E1'] }
#Convert the dictionary into DataFrame
df = pd.DataFrame(data)
#Get the unique values of 'E' column
df.E.unique()

Q7. How do you find the number of missing values in each column of a Pandas DataFrame?
ans:dataframe.isnull().sum() It gives you pandas series of column names along with the sum of missing values in each column

Q8. How do you fill missing values in a Pandas DataFrame with a specific value?
ans: we can use fillna(specific value)
eg:
#importing pandas module
import pandas as pd

#making data frame from csv file
nba = pd.read_csv("nba.csv")

#replacing na values in college with No college
nba["College"].fillna("No College", inplace = True)
Q9. How do you concatenate two Pandas DataFrames?
ans:A concatenation of two or more data frames can be done using pandas.concat () method. concat () in pandas works by combining Data Frames across rows or columns. We can concat two or more data frames either along rows (axis=0) or along columns (axis=1).

Q10. How do you merge two Pandas DataFrames on a specific column?
ans: result=pandas.merge(dataframe1,dataframe2,on="column name")
dataframe1 and dataframe2 join based on column name default how='inner'that means common for both table will return.
eg:
import pandas as pd
df3 = pd.merge(df1,df2,on='column_name')

Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?
ans:Pandas groupby is used for grouping the data according to the categories and apply a function to the categories. It also helps to aggregate data efficiently. Pandas dataframe.groupby () function is used to split the data into groups based on some criteria. pandas objects can be split on any of their axes.

Q12. How do you pivot a Pandas DataFrame?
ans:table = df.pivot(index='Country',columns='Year',values='Value')
Q13. How do you change the data type of a column in a Pandas DataFrame?
ans: In pandas, you can do this by using several methods like astype(), to_numeric(), covert_dttypes(), infer_objects().

Q14. How do you sort a Pandas DataFrame by a specific column?
ans: sort_values() method use to sort columns in pandas data frame.
eg: Dataframe.sort_values(by['column name'])

Q15. How do you create a copy of a Pandas DataFrame?
ans:Use the pandas dataframe copy () function to create a dataframe’s copy. It takes a single parameter deep. Use deep=True (default value) to create a deep copy. Use deep=False to create a shallow copy.

Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
ans:Use the operators &, |, ~ instead of and, or, not respectively Pandas provides operators & (for and ), | (for or ), and ~ (for not) to apply logical operations on series and to chain multiple conditions together when filtering a pandas dataframe.Use parenthesis () to group multiple conditions
eg:
df_filtered = df[(df['Shares']>=100) and (df['Shares']<=150)]
print(df_filtered)

Q17. How do you calculate the mean of a column in a Pandas DataFrame?
ans:

- df2= df['column'].mean() it will return the mean of entire column
- Dataframe.describe() it will give stastical details including mean,std,min,max..

Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?
ans:The Pandas DataFrame std () function allows to calculate the standard deviation of a data set. The standard deviation is usually calculated for a given column

Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?
ans:Correlation is used to summarize the strength and direction of the linear association between two quantitative variables. It is denoted by r and values between -1 and +1. A positive value for r indicates a positive association, and a negative value for r indicates a negative association.By using corr() function we can get the correlation between two columns in the dataframe.

Q20. How do you select specific columns in a DataFrame using their labels?
ans:To select two columns from a Pandas DataFrame, you can use the.loc [] method. This method takes in a list of column names and returns a new DataFrame that contains only those columns. For example, if you have a DataFrame with columns ['A', 'B', 'C'], you can use.loc [] to select only columns 'A','B' and 'C'.

Q21. How do you select specific rows in a DataFrame using their indexes?
ans:Select Rows by Index in Pandas DataFrame using iloc The iloc [ ] is used for selection based on position.

Q22. How do you sort a DataFrame by a specific column?
ans:To sort the rows of a DataFrame by a column, use pandas. DataFrame. sort_values () method with the argument by = column_name. The sort_values () method does not modify the original DataFrame, but returns the sorted DataFrame.

Q23. How do you create a new column in a DataFrame based on the values of another column?
ans:We can use DataFrame.apply () function to achieve this task.

Q24. How do you remove duplicates from a DataFrame?
ans:Pandas drop_duplicates () method helps in removing duplicates from the Pandas Dataframe In Python. Syntax of df.drop_duplicates ().

Q25. What is the difference between .loc and .iloc in Pandas?
ans:The main difference between pandas loc [] vs iloc [] is loc gets DataFrame rows & columns by labels/names and iloc [] gets by integer Index/position. For loc [], if the label is not present it gives a key error. For iloc [], if the position is not present it gives an index error.
