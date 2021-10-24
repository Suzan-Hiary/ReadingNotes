## Pandas in 10

pandas is a Python package providing fast, flexible, and expressive data structures designed to make working with “relational” or “labeled” data both easy and intuitive. It aims to be the fundamental high-level building block for doing practical, real-world data analysis in Python. Additionally, it has the broader goal of becoming the most powerful and flexible open source data analysis/manipulation tool available in any language. It is already well on its way toward this goal.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/1200px-Pandas_logo.svg.png)

### What kind of data does pandas handle?

To load the pandas package and start working with it, import the package. The community agreed alias for pandas is pd, so loading pandas as pd is assumed standard practice for all of the pandas documentation.

***import pandas as pd ***


To manually store data in a table, create a ** DataFrame **. When using a Python dictionary of lists, the dictionary keys will be used as column headers and the values in each list as columns of the DataFrame.

A ** DataFrame ** is a 2-dimensional data structure that can store data of different types (including characters, integers, floating point values, categorical data and more) in columns. It is similar to a spreadsheet, a SQL table or the data.frame in R.

The table has 3 columns, each of them with a column label. The column labels are respectively Name, Age and Sex.

The column Name consists of textual data with each value a string, the column Age are numbers and the column Sex is textual data.



![](https://media.geeksforgeeks.org/wp-content/uploads/finallpandas.png)



### Object creation :

* Creating a ** Series ** by passing a list of values, letting pandas create a default integer index:




                    s = pd.Series([1, 3, 5, np.nan, 6, 8])

                    s
                    Out[4]: 
                    0    1.0
                    1    3.0
                    2    5.0
                    3    NaN
                    4    6.0
                    5    8.0

                    dtype: float64





















* Creating a ** DataFrame ** by passing a NumPy array, with a datetime index and labeled columns:









            dates = pd.date_range("20130101", periods=6)

            dates
            Out[6]: 
            DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
                          '2013-01-05', '2013-01-06'],
                          dtype='datetime64[ns]', freq='D')

            df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list("ABCD"))

            df
            Out[8]: 
                              A         B         C         D
            2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
            2013-01-02  1.212112 -0.173215  0.119209 -1.044236
            2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
            2013-01-04  0.721555 -0.706771 -1.039575  0.271860
            2013-01-05 -0.424972  0.567020  0.276232 -1.087401
            2013-01-06 -0.673690  0.113648 -1.478427  0.524988


![](https://shanelynnwebsite-mid9n9g1q9y8tt.netdna-ssl.com/wp-content/uploads/2019/10/pandas-python-group-by-named-aggregation-update-1024x451.jpg)


[referance](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)