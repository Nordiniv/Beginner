# Pandas 🐼 and Git 🫴🏼 task
This task is fully customizable, you can choose to do it however may you like, but you have to do it. You are encouraged to use the internet to search for answers, use information from the task Menna sent you, and use info from this task there. And of course ask your colleagues for help whenever you need it! 🤗
## Pandas 🐼

### 1. What is Pandas?

Pandas is a Python library used for working with data sets, you should know this by now. It has functions for analyzing, cleaning, exploring, and manipulating data. The name "Pandas" has a reference to both "Panel Data", and "Python Data Analysis" and was created by Wes McKinney in 2008.

Speaking of *analyzing, cleaning, exploring, and manipulating* data, what functions can you use for each of these tasks? 🤔:
- **A**nalyze data?
    `describe()`: Provides descriptive statistics for a DataFrame.<br>
    `corr()`: Calculates the correlation between two or more columns.<br>
    `cov()`: Calculates the covariance between two or more columns.<br>
    `plot()`: Plots the data of a DataFrame.<br>
    `pivot_table()`: Creates a pivot table from a DataFrame.<br>
    `groupby()`: Groups data by one or more columns and performs aggregate operations on the groups.<br>
- **C**lean data?
    `dropna()`: Drops rows or columns that contain missing values.<br>
    `fillna()`: Fills missing values with a specified value.<br>
    `replace()`: Replaces specific values with a different value.<br>
    `unique()`: Returns the unique values in a column.<br>
    `value_counts()`: Counts the number of occurrences of each value in a column.<br>
    `isnull()`: Returns a Boolean value indicating whether a value is missing.<br>
- **E**xplore data?
    `head()`: Returns the first few rows of a DataFrame.<br>
    `tail()`: Returns the last few rows of a DataFrame.<br>
    `info()`: Provides information about the DataFrame, such as the number of rows and columns, the data types of the columns, and the    missing values.<br>
    `describe()`: Provides descriptive statistics for a DataFrame.<br>
    `hist()`: Plots the distribution of the values in a column.<br>
    `boxplot()`: Plots the distribution of the values in a column, along with the outliers.<br>

- **M**anipulate data?
    `merge()`: Combines two or more DataFrames based on common columns.<br>
    `join()`: Combines two or more DataFrames based on common rows.<br>
    `concat()`: Combines two or more DataFrames along a common axis.<br>
    `reshape()`: Changes the shape of a DataFrame.<br>
    `sort_values()`: Sorts a DataFrame by one or more columns.<br>
    `apply()`: Applies a function to each row or column of a DataFrame.<br>
**Fill the table below:**
  

function | what it does | category
------------ | ----------- | ---------
`astype()` |Converts the data type of a column or multiple columns|Data transformation.
`groupby()` |Groups data by one or more columns and performs aggregate operations on the groups|Data aggregation.  
`sort_values()` |Sorts a DataFrame by one or more columns.|Data wrangling.
`pivot_table()` |Creates a pivot table from a DataFrame.|Data analysis.
`merge()` |Combines two or more DataFrames based on common columns|Data manipulation.
`plot()` |Plots the data of a DataFrame|Data visualization.
`corr()` |Calculates the correlation between two or more columns.|Data analysis.
`cov()` |Calculates the covariance between two or more columns.|Data analysis.
`apply()` |Applies a function to each row or column of a DataFrame.|Data manipulation.
`loc()` |Selects rows and columns by label.|Data selection
`iloc()` |Selects rows and columns by integer location.|Data selection.
`iterrows()` |Iterates over the rows of a DataFrame|Data iteration.
`aggregate()` |Performs aggregate operations on a DataFrame.|Data aggregation.

$\rightarrow$ You may insert code snippets here if you like!

### 2. Pandas and NumPy 🔢 [BONUS 🎁](https://www.imdb.com/title/tt1068680/)

Pandas is built on top of the NumPy package, which means that many of the methods in NumPy are also available in Pandas. Data in pandas is often used to feed statistical analysis in SciPy, plotting functions from Matplotlib, and machine learning algorithms in Scikit-learn.

Speaking of NumPy, here are questions about it:

- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.vstack((a, b))

print(c[1][2])
```
- First, the `np.vstack()` function concatenates the two arrays a and b vertically. This means that the first row of the resulting array will be the elements of a, and the second row will be the elements of b.

Then, the print() function prints the element at index [1][2] of the array c. Index [1] refers to the second row of the array, and index [2] refers to the third element of that row. Therefore, the output of the print() function is the value `6`, which is the third element of the second row of the array c.

- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.intersect1d(a, b)

print(c)
```
- The `np.intersect1d()` function finds the intersection of two arrays. In this case, the arrays a and b do not have any elements in common, so the output of the np.intersect1d() function is `an empty array`.
  
- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.setdiff1d(a, b)

print(c)
```
- In this case, the array a contains the elements 1, 2, and 3. The array b contains the elements 4, 5, and 6. The set difference of these two arrays is the collection of elements which are in a but not in b, which is the array `[1, 2, 3]`.

- Which of the following is a function in NumPy used for carrying out Einstein summations?

    - [ ]  `np.tensordot()`
    - [ ]  `np.dot()`
    - \[True\]  `np.einsum()`
    - [ ]  `np.outer()`

- The `np.outer` function is primarily intended for:

    - [ ]  Computing the tensor dot product of two arrays.
    - \[True\]  Computing the outer product of two arrays.
    - [ ]  Computing the inner product of two arrays.
    - [ ]  Computing the cross product of two arrays.


### 3. Pandas and Matplotlib 📈
Pandas can be used to visualize data using a wrapper for `matplotlib.pyplot.plot()`. You can plot data directly from your DataFrame using certain functions.

- What functions can you use to plot data directly from your DataFrame? 🤔
- There are many functions you can use to plot data directly from a DataFrame in Python. Some of the most common ones are:

    - `DataFrame.plot()`: This is the most general function for plotting data from a DataFrame. It can be used to plot a variety of different plots, such as line plots, bar plots, and scatter plots.
    - `DataFrame.hist()`: This function can be used to plot a histogram of the data in a DataFrame. A histogram is a graphical representation of the distribution of the data.
    - `DataFrame.boxplot()`: This function can be used to plot a box plot of the data in a DataFrame. A box plot is a graphical representation of the distribution of the data, including the median, quartiles, and outliers.
    - `DataFrame.scatterplot()`: This function can be used to plot a scatter plot of the data in a DataFrame. A scatter plot is a graphical representation of the relationship between two variables.

- What is the output of the following code? And why is it so?

``` python
df = pd.DataFrame(np.random.randn(10, 4), columns=['a', 'b', 'c', 'd'])
df.plot.scatter(x='a', y='b')
```
- What do you know about `np.random.randn()`? And how does it depend on `np.random.seed()`?
- The NumPy function `np.random.randn()` generates random numbers from the standard normal distribution. The standard normal distribution is a bell-shaped distribution with mean 0 and standard deviation 1.
- The `np.random.randn()` function takes an optional argument called `seed`. The `seed` is an integer that is used to initialize the random number generator. If the `seed` is not specified, then the random number generator will use the current system time as the `seed`.
- If you set the seed to a specific value, then `np.random.randn()` will always generate the same sequence of random numbers. This can be useful for debugging or for comparing the results of different code runs.

## Git 🫴🏼
I know you are all familiar with Git, but let's see how much you know about it! 🤓

- What is the default text editor for the Bash shell with a Windows-based Git install?

    - [ ] Emacs
    - \[True\] Vim
    - [ ] Notepad++
    - [ ] Bash

- Before you install Git, which of the following prerequisite products must be present and configured on your local OS?

    - [ ] Python
    - [ ] Java Development Kit 1.8 or newer
    - [ ] Apache Maven
    - \[True\] Nothing


- After you install Git and prior to issuing the first commit, which two configuration properties does the tool expect to be configured?

    - \[True\] username and email address
    - [ ] username and password
    - [ ] email address and password
    - [ ] username and IP address

- Which of the following commands is used to create a new Git repository?

    - \[True\] git init
    - [ ] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to clone a remote Git repository?

    - [ ] git init
    - \[True\] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to stage a file for inclusion in the next commit?

    - \[True\] git add
    - [ ] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to commit staged changes to the local repository?

    - [ ] git add
    - \[True\] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to push committed changes to a remote repository?

    - [ ] git add
    - [ ] git commit
    - \[True\] git push
    - [ ] git pull

- Who is attributed with inventing Git?

    - [ ] Junio Hamano
    - [ ] James Gosling
    - [ ] Kohsuke Kawaguchi
    - \[True\] Linus Torvalds

- After you initialize a new Git repository and create a file named git-quiz.html, which of the following commands will not work if issued?

    - [ ] git add git-quiz.html
    - [ ] git status
    - [True] git add .
    - [ ] git commit -m "git quiz web file added"

- Which file can you configure to ensure that certain file types are never committed to the local Git repository?

    - [ ] ignore.git
    - [<div style="border: 1px solid black; padding: 10px;">
         <span style="color: green">&#10004;</span>
       </div>] .gitignore
    - [ ] gitignore.txt
    - [ ] git.ignore

- Under which circumstance should you use a single dash within a bash command, as opposed to a double dash?
    - You should use a single dash (-) within a bash command when you are specifying a single-character option. For example, the -n option tells the grep command to print only the lines that match the pattern, but not the lines themselves.
    - You should use a double dash (--) within a bash command when you are specifying a multi-character option. For example, the --help option tells the grep command to print a help message.

- Which vendor acquired GitHub for $7.5 billion in June 2018?
    - Microsoft
You may want to check [this](https://www.youtube.com/watch?v=Q6G-J54vgKc&t=16813s)

## Problem Solving 🤔
[A. Panoramix's Prediction](https://codeforces.com/problemset/problem/80/A)<br>
    [link](https://codeforces.com/contest/80/submission/220905484)<br>
[A. Again Twenty Five!](https://codeforces.com/problemset/problem/630/A)<br>
    [link](https://codeforces.com/contest/630/submission/220622939)<br>