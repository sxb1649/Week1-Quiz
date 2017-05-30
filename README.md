# Week1-Quiz


Correct
1 / 1 points
1. 
R was developed by statisticians working at

Harvard University

The University of Auckland
Correct 
The R language was developed by Ross Ihaka and Robert Gentleman who were statisticians at the University of Auckland in New Zealand.

StatSci

Bell Labs

Correct
1 / 1 points
2. 
The definition of free software consists of four freedoms (freedoms 0 through 3). Which of the following is NOT one of the freedoms that are part of the definition? Select all that apply.

The freedom to study how the program works, and adapt it to your needs.
Un-selected is correct 

The freedom to prevent users from using the software for undesirable purposes.
Correct 
This is not part of the free software definition. Freedom 0 requires that the users of free software be free to use the software for any purpose.

The freedom to improve the program, and release your improvements to the public, so that the whole community benefits.
Un-selected is correct 

The freedom to run the program, for any purpose.
Un-selected is correct 

The freedom to sell the software for any price.
Correct 
This is not part of the free software definition. The free software definition does not mention anything about selling software (although it does not disallow it).

The freedom to redistribute copies so you can help your neighbor.
Un-selected is correct 

The freedom to restrict access to the source code for the software.
Correct 
This is not part of the free software definition. Freedoms 1 and 3 require access to the source code.

Correct
1 / 1 points
3. 
In R the following are all atomic data types EXCEPT: (Select all that apply)

complex
Un-selected is correct 

logical
Un-selected is correct 

data frame
Correct 
'data frame' is not an atomic data type in R.

list
Correct 
'list' is not an atomic data type in R.

array
Correct 
'array' is not an atomic data type in R.

matrix
Correct 
'matrix' is not an atomic data type in R.

table
Correct 
'table' is not an atomic data type in R.

integer
Un-selected is correct 

numeric
Un-selected is correct 

character
Un-selected is correct 

Correct
1 / 1 points
4. 
If I execute the expression x <- 4 in R, what is the class of the object `x' as determined by the `class()' function?

list

complex

integer

matrix

numeric
Correct 

real

vector

Correct
1 / 1 points
5. 
What is the class of the object defined by x <- c(4, TRUE)?

list

numeric
Correct 
The numeric class is the "lowest common denominator" here and so all elements will be coerced into that class.

integer

matrix

logical

character

Correct
1 / 1 points
6. 
If I have two vectors x <- c(1,3, 5) and y <- c(3, 2, 10), what is produced by the expression cbind(x, y)?

a 2 by 3 matrix

a vector of length 2

a matrix with 2 columns and 3 rows
Correct 
The 'cbind' function treats vectors as if they were columns of a matrix. It then takes those vectors and binds them together column-wise to create a matrix.

a 3 by 3 matrix

a vector of length 3

a 2 by 2 matrix

Correct
1 / 1 points
7. 
A key property of vectors in R is that

the length of a vector must be less than 32,768

elements of a vector can be of different classes

a vector cannot have have attributes like dimensions

elements of a vector all must be of the same class
Correct 

elements of a vector can only be character or numeric

Incorrect
0 / 1 points
8. 
Suppose I have a list defined as x <- list(2, "a", "b", TRUE). What does x[[1]] give me? Select all that apply.

a list containing the number 2.
Un-selected is correct 

a numeric vector containing the element 2.
Correct 

a numeric vector of length 1.
This should be selected 

a character vector containing the element "2".
Un-selected is correct 

a list containing the letter "a".
Un-selected is correct 

Correct
1 / 1 points
9. 
Suppose I have a vector x <- 1:4 and y <- 2:3. What is produced by the expression x + y?

a numeric vector with the values 3, 5, 3, 4.

an error.

a numeric vector with the values 1, 2, 5, 7.

a warning

an integer vector with the values 3, 5, 5, 7.
Correct 

an numeric vector with the values 3, 5, 5, 7.

an integer vector with the values 3, 5, 3, 4.

Correct
1 / 1 points
10. 
Suppose I have a vector x <- c(17, 14, 4, 5, 13, 12, 10) and I want to set all elements of this vector that are greater than 10 to be equal to 4. What R code achieves this? Select all that apply.

x[x >= 10] <- 4
Un-selected is correct 

x[x < 10] <- 4
Un-selected is correct 

x[x > 10] <- 4
Correct 
You can create a logical vector with the expression x > 10 and then use the [ operator to subset the original vector x.

x[x == 4] > 10
Un-selected is correct 

x[x > 4] <- 10
Un-selected is correct 

x[x >= 11] <- 4
Correct 
You can create a logical vector with the expression x >= 11 and then use the [ operator to subset the original vector x.

x[x == 10] <- 4
Un-selected is correct 

x[x > 10] == 4
Un-selected is correct 

Correct
1 / 1 points
11. 
Use the Week 1 Quiz Data Set to answer questions 11-20.

In the dataset provided for this Quiz, what are the column names of the dataset?

Ozone, Solar.R, Wind

Month, Day, Temp, Wind

Ozone, Solar.R, Wind, Temp, Month, Day
Correct 
You can get the column names of a data frame with the `names()' function.

1, 2, 3, 4, 5, 6

Correct
1 / 1 points
12. 
Extract the first 2 rows of the data frame and print them to the console. What does the output look like?



1
2
3
  Ozone Solar.R Wind Temp Month Day
1    18     224 13.8   67     9  17
2    NA     258  9.7   81     7  22



1
2
3
  Ozone Solar.R Wind Temp Month Day
1    41     190  7.4   67     5   1
2    36     118  8.0   72     5   2
Correct 
You can extract the first two rows using the [ operator and an integer sequence to index the rows.



1
2
3
  Ozone Solar.R Wind Temp Month Day
1     9      24 10.9   71     9  14
2    18     131  8.0   76     9  29



1
2
3
  Ozone Solar.R Wind Temp Month Day
1     7      NA  6.9   74     5  11
2    35     274 10.3   82     7  17

Correct
1 / 1 points
13. 
How many observations (i.e. rows) are in this data frame?

160

129

45

153
Correct 
You can use the `nrows()' function to compute the number of rows in a data frame.

Correct
1 / 1 points
14. 
Extract the last 2 rows of the data frame and print them to the console. What does the output look like?



1
2
3
    Ozone Solar.R Wind Temp Month Day
152    31     244 10.9   78     8  19
153    29     127  9.7   82     6   7



1
2
3
    Ozone Solar.R Wind Temp Month Day
152    11      44  9.7   62     5  20
153   108     223  8.0   85     7  25



1
2
3
    Ozone Solar.R Wind Temp Month Day
152    34     307 12.0   66     5  17
153    13      27 10.3   76     9  18



1
2
3
    Ozone Solar.R Wind Temp Month Day
152    18     131  8.0   76     9  29
153    20     223 11.5   68     9  30
Correct 
The `tail()' function is an easy way to extract the last few elements of an R object.

Correct
1 / 1 points
15. 
What is the value of Ozone in the 47th row?

63

18

34

21
Correct 
The single bracket [ operator can be used to extract individual rows of a data frame.

Correct
1 / 1 points
16. 
How many missing values are in the Ozone column of this data frame?

78

37
Correct 
The `is.na' function can be used to test for missing values.

43

9

Correct
1 / 1 points
17. 
What is the mean of the Ozone column in this dataset? Exclude missing values (coded as NA) from this calculation.

31.5

53.2

42.1
Correct 
The `mean' function can be used to calculate the mean.

18.0

Correct
1 / 1 points
18. 
Extract the subset of rows of the data frame where Ozone values are above 31 and Temp values are above 90. What is the mean of Solar.R in this subset?

205.0

334.0

185.9

212.8
Correct 
You need to construct a logical vector in R to match the question's requirements. Then use that logical vector to subset the data frame.

Correct
1 / 1 points
19. 
What is the mean of "Temp" when "Month" is equal to 6?

90.2

79.1
Correct 

75.3

85.6

Correct
1 / 1 points
20. 
What was the maximum ozone value in the month of May (i.e. Month is equal to 5)?

100

115
Correct 

18

97
