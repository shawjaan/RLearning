# RLearning

## R: An introduction to Graphs

### Barcharts
The most basic graphic for the most basic data. Great for starting analysis. 

We need to create a summary table to use bar charts.
Example: cylinders (a variable) <- table(mtcars$cyl)

### Histograms
Used to data that is quantitative, scaled, measured, interval.
It allows to see what we have.

We look for the Shape, Gaps in distribution, Outliers, and Symmetry in the Histograms.

### Scatterplots
used when we want to visualize the association between two quantitative variables.

We look if our two variables are Linear, consistent Spread, Outliers, and Corralation.

### Overlayiny Plots
We get increased infomation densisty, but we should use restraint. 

## R: An introduction to Basic Statistics
After we have done the graphs we want to get some precision.

Example:
Count -> for categories
Quartiles & mean -> for quantitative variables 

### Summary()
Categorical variable -> get the count of 
Quantitive variable -> the Min, Meadian, and Max

### Describe()
gets more detail.

Example: n, mean, SD, median,10% trimmed mean, MAD, min/max, range. 

### Selecting Cases
Focus on analysis by selecting a row using []. We can do this by
selecting by category
or selecting by value
or selecting both

## Accessing data
### Data formates
we can have different data Types and data Structures
the data structures are Vectors (scalar), Matrix (array), Data frame (vector of multiple types, closest thing to a spreadsheet but must have all the same length), and List (most flexable, can include any class, length, or stucture)
 
### Factors
it has to do with Categories and Names. it is an "attribute" of a vector that specifies the possible values and their order.

### Enterting data
we can enter data manually, however we usually use data sets but we might want to add more data manually.

Many methods:
colon, seq, c (concatante), scan (input from the consol), & rep (repeat).
also "<-" the assignment operator to assign value to variable.

### Importing data
CSV files (comma seprated values)
TXT files 
XLSX files (excel spreadsheets)
JSON files (Java Script Object Notation for web)

rio (R Input Output) is a package loader commonaly used
https://cran.r-project.org/doc/manuals/R-data.html#Reading-Excel-spreadsheets

## Modeling Data
Hierarchical vs. set K
Measures of distance
Divisive vs. agglometative

But for now, I will study it simple.
Euclidean distance,
hierarchical clustering,
and divisive method

### Hierarchical Clustering
which cases belong with each other. it depended on our criteria. In the example file, we are able to group the cars with similarites.

### Principle Components
aka Dimensional Reduction 
Less = More sometimes.
That is, less noise and fewer unhelful variables in data = more meaning 

![Screen Shot 2023-05-03 at 2 20 21 PM](https://user-images.githubusercontent.com/114831110/236008450-ae968e2c-2c52-47a2-9149-10279f4c3984.png)

![Screen Shot 2023-05-03 at 2 20 47 PM](https://user-images.githubusercontent.com/114831110/236008562-8a18de42-4199-4409-ab2d-ab660c891a77.png)

![Screen Shot 2023-05-03 at 2 21 32 PM](https://user-images.githubusercontent.com/114831110/236008714-90a540cf-2a6d-447a-8e02-ea53c5985922.png)

We went from 2D to 1D but maintained the most important information

The reason we did this is so we can make the analysis and interpretation easier and more reliable
`
![Screen Shot 2023-05-03 at 2 20 47 PM](https://user-images.githubusercontent.com/114831110/236008562-8a18de42-4199-4409-ab2d-ab660c891a77.png)

### Regression
Out of many variables, we get one variable.
We use many variables to predict scores on one variable. There are many version and adaptations of regression that make it flexible and powerful

lm -> (linear model)

