# learning_pandas
Pandas is an open-source Python library that provides easy-to-use data structures and data analysis tools for data manipulation and analysis. 
It is widely used in data science, machine learning, and other data-related fields for tasks such as data cleaning, exploration, transformation, and analysis. 
Pandas is built on top of NumPy, which makes it a powerful tool for working with structured data.

## [1] series.ipynb
### What is Pandas Series?
A Pandas Series is a one-dimensional labeled data structure provided by the Pandas library. Pandas Series are commonly used for data manipulation and analysis because they provide a powerful and convenient way to work with one-dimensional data, including data cleaning, filtering, and mathematical operations. Additionally, Series can be used as building blocks for more complex data structures, such as Pandas DataFrames, which are two-dimensional data structures often used in data analysis and manipulation.

Here are some key characteristics of Pandas Series:

- Homogeneous Data: A Pandas Series contains data of the same data type. This data type could be integers, floating-point numbers, strings, etc.

- Labeling: Each element in a Pandas Series has a label, which is known as its index. You can think of the index as a label or name for each data point, making it easy to access and manipulate data.

- Data Alignment: When performing operations on Series, Pandas automatically aligns data based on the labels, ensuring that data remains consistent and operations are performed element-wise.

### Topics covered in  file 'series.ipynb'
- creating series
- Series attributes:- size,dtype,name,is_unique,index,values
- Series using 'read_csv'
- Series Methods:- head(),tail(),sample(),value_counts(),sort_values(),sort_index()
- Series Maths methods:- describe(),count(),mean(),median(),mode(),var(),std(),min(),max(),sum(),prod()
- Seires Indexing:-Integer indexing, Negative Indexing, Fancy Indexing, Indexing with labels
- Series Slicing
- Series Editing
- Series with python functionalities:- len(),type(),sorted(),dir(),max(),min(),membership operator(in,not in)
- looping
- Operators
- Boolean Indexing on Series
- Plotting graphs on series
- astype(),between(),clip(),drop_duplicates(),isnull(),dropna(),fillna(),isin(),apply(),copy()

## [2] Dataframe.ipynb
### What is Pandas Dataframe?
A Pandas DataFrame is a two-dimensional, tabular data structure provided by the Pandas library.They are one of the most commonly used data structures in data analysis and manipulation, because they 
provide a rich set of functionalities for data cleaning, transformation, analysis, and visualization. They are widely used in data science, data analysis, and data engineering tasks, making them a fundamental tool for working with structured data in Python.
Here are some key characteristics of Pandas DataFrames:

- Tabular Structure: A DataFrame consists of rows and columns, where each column can contain data of different types (e.g., integers, floats, strings). This makes it suitable for handling structured data with different data types.
- Labeled Axes: DataFrames have both row and column labels, allowing for easy access to and manipulation of data. Rows are indexed, and columns have names, making it intuitive to select, filter, and manipulate specific subsets of data.
- Heterogeneous Data: Unlike NumPy arrays, which require all elements to be of the same data type, a Pandas DataFrame can store data of different data types within the same structure.
- Data Alignment: DataFrames are designed for data alignment, meaning that when you perform operations between DataFrames or between a DataFrame and a Pandas Series, data is aligned based on the row and column labels. This simplifies many common data manipulation tasks.
  
## [3] Groupby.ipynb
### What is 'groupby' in Pandas?
Groupby function is a powerful method that allows you to group rows in a DataFrame based on one or more columns' values and then perform various operations on these groups.
It's particularly useful for tasks like aggregation, summarization, and data analysis.
In file 'groupby.ipynb', certain groupby operations are performed on different datasets.

## [4] Merging, Joining & Concatenating.ipynb
### What are the 3 main operations for combining data in Pandas?
The three main operations are merging, joining, and concatenating. These operations are useful for combining data from different sources, joining tables, and merging data with different structures.
It's important to choose the appropriate operation based on your data and what you want to achieve. Understanding the structure and relationships between the DataFrames is essential for successful data combination. Each operation has its specific use case, and it's crucial to know which one to use in different scenarios to achieve the desired results when working with multiple datasets in Pandas.

1. Concatenation:-
- It is used to combine DataFrames along a particular axis (either rows or columns).
- It is performed using the pd.concat() function.
- By default, it stacks DataFrames on top of each other (along the rows) to create a new DataFrame.
- You can specify the axis (0 for rows, 1 for columns) and other parameters to control the behavior of concatenation.
2. Merging:-
- Itis used to combine DataFrames based on common columns (or indices).
- It is performed using the pd.merge() function, which performs database-style joins (similar to SQL joins).
- You specify which columns to join on, and Pandas merges the DataFrames accordingly (inner, outer, left, right joins).
3. Joining:-
- It is a convenient method for combining DataFrames with different column names or indices.
- It is performed using the join() method.
- You can specify the join method (left, right, inner, outer) and join on column names or indices.

## [5] MultiIndex Series and DataFrames.ipynb
- MultiIndex Series and MultiIndex DataFrames (also known as hierarchical indexing) allow you to work with data that has multiple levels of row or column labels. 
- This is useful when you have data with complex hierarchical structures and need to access and manipulate it at different levels of granularity.
- They allow for more flexible and precise data handling and analysis in Pandas.

## [6] Vectorised String Operations.ipynb
- Vectorized string operations in Pandas enable you to apply string functions and operations to entire columns of string data in a Pandas Series or DataFrame efficiently. 
- These operations are performed element-wise without the need for explicit looping, making them both faster and more concise. 
- To use vectorized string operations in Pandas, you can access the .str attribute of a Series containing string data.
- str.lower(), str.upper() ,str.capitalize() ,str.title() ,str.len() ,str.strip() ,str.split() ,str.get() ,str.replace, str.endswith(), str.startswith(),RegEx( str.contains(), str.extract()), slicing(str[:]) etc...

## Date Time
- pd.Timestamp()
- pd.DatetimeIndex()
- pd.date_range()
- pd.to_datetime()
- dt accessor:- dt.year, dt.month, dt.day, dt.month_name etc...
