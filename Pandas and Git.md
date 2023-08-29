# Pandas 🐼 and Git 🫴🏼 task
This task is fully customizable, you can choose to do it however may you like, but you have to do it. You are encouraged to use the internet to search for answers, use information from the task Menna sent you, and use info from this task there. And of course ask your colleagues for help whenever you need it! 🤗
## Pandas 🐼

### 1. What is Pandas?

Pandas is a Python library used for working with data sets, you should know this by now. It has functions for analyzing, cleaning, exploring, and manipulating data. The name "Pandas" has a reference to both "Panel Data", and "Python Data Analysis" and was created by Wes McKinney in 2008.

Speaking of *analyzing, cleaning, exploring, and manipulating* data, what functions can you use for each of these tasks? 🤔:
- **A**nalyze data?
- **C**lean data?
- **E**xplore data?
- **M**anipulate data?

**Fill the table below:**
  

function | what it does | category
------------ | ----------- | ---------
`astype()` |used to convert the data type of a pandas Series or DataFrame column to a specified data type |Manipulate Data
`groupby()` |split data into groups based on unique values |Analysis Data
`sort_values()` | sorts the rows of a DataFrame based on specified columns |Manipulate Data  
`pivot_table()` |create a spreadsheet-style pivot table as a DataFrame|Analyze Data
`merge()` |used to combine two or more DataFrames based on common columns|Manipulate Data  
`plot()` |create various types of visualizations from DataFrame|Explore Data  
`corr()` | used to calculate the correlation between numeric columns|Analyze Data  
`cov()` |used to calculate the covariance between numeric columns|Analyze Data  
`apply()` |used to apply a custom function to each element or row|Manipulate Data.  
`loc()` |used to select rows and columns from a DataFrame by index|Explore Data.  
`iloc()` | used to select rows and columns from a DataFrame by integer index|Explore Data  
`iterrows()` | used to iterate over rows of a DataFrame|Explore Data  
`aggregate()` |used to apply multiple aggregation functions simultaneously to columns|Analyze Data

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
**The output will be 6 cause it target the second row and the third column**

- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.intersect1d(a, b)

print(c)
```
**The output will be an empty array cause intersect1d() function is used to find the intersection of two arrays "the common element" and in this case there is no common elements**
  
- What is the output of the following code? And why is it so?

``` python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
c = np.setdiff1d(a, b)

print(c)
```
**The output will be [1,2,3] cause this function is used to find the difference between two arrays & it return the elements that are in a and not in b**

- Which of the following is a function in NumPy used for carrying out Einstein summations?

    - [ ]  `np.tensordot()`
    - [ ]  `np.dot()`
    - [x]  `np.einsum()`
    - [ ]  `np.outer()`

- The `np.outer` function is primarily intended for:

    - [ ]  Computing the tensor dot product of two arrays.
    - [x]  Computing the outer product of two arrays.
    - [ ]  Computing the inner product of two arrays.
    - [ ]  Computing the cross product of two arrays.


### 3. Pandas and Matplotlib 📈
Pandas can be used to visualize data using a wrapper for `matplotlib.pyplot.plot()`. You can plot data directly from your DataFrame using certain functions.

- What functions can you use to plot data directly from your DataFrame? 🤔
**plot() function can plot data, allows you to create various types of visualizations like bar plot and scatter plot.**

- What is the output of the following code? And why is it so?

``` python
df = pd.DataFrame(np.random.randn(10, 4), columns=['a', 'b', 'c', 'd'])
df.plot.scatter(x='a', y='b')

**The output will be a scatter plot of the data in columns 'a' and 'b' from the DataFrame, will display points where the x-coordinate "a" and the y-coordinate "b"**
![Alt text](data:image/png;base64,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)

```
- What do you know about `np.random.randn()`? And how does it depend on `np.random.seed()`?
   **np.random.randn() generates random numbers from a standard normal distribution**
   **sets the initial state for the random number generator in NumPy, affecting the sequence of random numbers generated by functions like np.random.randn()**
## Git 🫴🏼
I know you are all familiar with Git, but let's see how much you know about it! 🤓

- What is the default text editor for the Bash shell with a Windows-based Git install?

    - [ ] Emacs
    - [x] Vim
    - [ ] Notepad++
    - [ ] Bash

- Before you install Git, which of the following prerequisite products must be present and configured on your local OS?

    - [ ] Python
    - [ ] Java Development Kit 1.8 or newer
    - [ ] Apache Maven
    - [x] Nothing


- After you install Git and prior to issuing the first commit, which two configuration properties does the tool expect to be configured?

    - [x] username and email address
    - [ ] username and password
    - [ ] email address and password
    - [ ] username and IP address

- Which of the following commands is used to create a new Git repository?

    - [x] git init
    - [ ] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to clone a remote Git repository?

    - [ ] git init
    - [x] git clone
    - [ ] git commit
    - [ ] git push

- Which of the following commands is used to stage a file for inclusion in the next commit?

    - [x] git add
    - [ ] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to commit staged changes to the local repository?

    - [ ] git add
    - [x] git commit
    - [ ] git push
    - [ ] git pull

- Which of the following commands is used to push committed changes to a remote repository?

    - [ ] git add
    - [ ] git commit
    - [x] git push
    - [ ] git pull

- Who is attributed with inventing Git?

    - [ ] Junio Hamano
    - [ ] James Gosling
    - [ ] Kohsuke Kawaguchi
    - [x] Linus Torvalds

- After you initialize a new Git repository and create a file named git-quiz.html, which of the following commands will not work if issued?

    - [ ] git add git-quiz.html
    - [ ] git status
    - [ ] git add .
    - [x] git commit -m "git quiz web file added"

- Which file can you configure to ensure that certain file types are never committed to the local Git repository?

    - [ ] ignore.git
    - [x] .gitignore
    - [ ] gitignore.txt
    - [ ] git.ignore

- Under which circumstance should you use a single dash within a bash command, as opposed to a double dash?

- Which vendor acquired GitHub for $7.5 billion in June 2018?

You may want to check [this](https://www.youtube.com/watch?v=Q6G-J54vgKc&t=16813s)

## Problem Solving 🤔
[A. Panoramix's Prediction](https://codeforces.com/problemset/problem/80/A)

https://github.com/urfavnada/Task/blob/main/Problem%201%20and%202
[A. Again Twenty Five!](https://codeforces.com/problemset/problem/630/A)
https://github.com/urfavnada/Task/blob/main/Problem%201%20and%202
