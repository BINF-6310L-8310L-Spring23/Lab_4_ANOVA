# Lab_3_ANOVA

To practice using ANOVA we will do the exercises in the Krijnen Introduction to Biostats 

This uses the Golub 199 gene expression data. To do this you will need to load the data. 

```
library(multtest)
data(golub)
```
Now the data will be stored in a matrix called golub

Now we do Exercies 1 and 2 from section 5.7


### 1. Analysis of gene expressions of B-cell ALL patients.

(a) Construct a data frame containing the expression values for the B-cell ALL patients in stage B, B1, B2, B3, B4 from the ALL data.

(b) How many patients are in each group.

(c) Test the normality of the residuals from the linear model used for analysis of variance for all gene expression values. Collect the p-values in a vector.

(d) Do the same for the homoscedasticity assumption.

(e) How many gene expressions are normally distributed and how many homoscedastic? For how many do both hold?


### 2. Further analysis of gene expressions of B-cell ALL patients. Continue with the previous data frame containing the expression values for the B-cell ALL patients in stage B, B1, B2, B3, B4 from the ALL data.

(a) Collect the overall p-values from ANOVA in a vector.

(b) Use featureNames() to report the afymetrix id's of the genes with smaller p-values than 0.000001.

(c) Collect the overall p-values from the Kruskal-Walles test in a vector.

(d) Use featureNames() to report the afymetrix id's of the genes with smaller p-values than 0.000001.

(e) Briefly comment on the di®erences you observe. That is, how many genes have p-values smaller than 0.001 from both ANOVA and Krusal-Wallis? How many only from one type of test? Hint: Collect TRUE/FALSES in logical vectors and use table.
