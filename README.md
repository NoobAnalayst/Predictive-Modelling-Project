# Predictive-Modelling-Project<br>
In this project we have learned about predictive modelling techniques and algo's used like Linear reggresion, Logistic regression linear Discrimenant Analysis and Decision Tree (CART).
<br>


Problem 1: Linear Regression<br>
The comp-activ databases is a collection of a computer systems activity measures .
The data was collected from a Sun Sparcstation 20/712 with 128 Mbytes of memory running in a
multi-user university department. Users would typically be doing a large variety of tasks ranging
from accessing the internet, editing files or running very cpu-bound programs.
As you are a budding data scientist you thought to find out a linear equation to build a model to
predict 'usr'(Portion of time (%) that cpus run in user mode) and to find out how each attribute
affects the system to be in 'usr' mode using a list of system attributes.
<br>
Dataset for Problem 1: compactiv.xlsx
DATA DICTIONARY:
-----------------------
System measures used:<br>
lread - Reads (transfers per second ) between system memory and user memory<br>
lwrite - writes (transfers per second) between system memory and user memory<br>
scall - Number of system calls of all types per second<br>
sread - Number of system read calls per second .<br>
swrite - Number of system write calls per second .<br>
fork - Number of system fork calls per second.<br>
exec - Number of system exec calls per second.<br>
rchar - Number of characters transferred per second by system read calls<br>
wchar - Number of characters transfreed per second by system write calls<br>
pgout - Number of page out requests per second<br>
ppgout - Number of pages, paged out per second<br>
pgfree - Number of pages per second placed on the free list.<br>
pgscan - Number of pages checked if they can be freed per second<br>
atch - Number of page attaches (satisfying a page fault by reclaiming a page in memory) per
second<br>
pgin - Number of page-in requests per second<br>
ppgin - Number of pages paged in per second<br>
pflt - Number of page faults caused by protection errors (copy-on-writes).<br>
vflt - Number of page faults caused by address translation .<br>
runqsz - Process run queue size (The number of kernel threads in memory that are waiting for a
CPU to run.<br>
Typically, this value should be less than 2. Consistently higher values mean that the system might
be CPU-bound.)<br>
freemem - Number of memory pages available to user processes<br>
freeswap - Number of disk blocks available for page swapping.<br>
------------------------
usr - Portion of time (%) that cpus run in user mode<br>

Questions For Problem 1 :----- 

1.1 Read the data and do exploratory data analysis. Describe the data briefly. (Check the Data
types, shape, EDA, 5 point summary). Perform Univariate, Bivariate Analysis, Multivariate
Analysis.<br>
1.2 Impute null values if present, also check for the values which are equal to zero. Do they
have any meaning or do we need to change them or drop them? Check for the possibility of
creating new features if required. Also check for outliers and duplicates if there.<br>
1.3 Encode the data (having string values) for Modelling. Split the data into train and test (70:30).
Apply Linear regression using scikit learn. Perform checks for significant variables using
appropriate method from statsmodel. Create multiple models and check the performance of
Predictions on Train and Test sets using Rsquare, RMSE & Adj Rsquare. Compare these
models and select the best one with appropriate reasoning.<br>
1.4 Inference: Basis on these predictions, what are the business insights and recommendations.<br>


Problem 2: Logistic Regression, LDA and CART
You are a statistician at the Republic of Indonesia Ministry of
Health and you are provided with a data of 1473 females collected
from a Contraceptive Prevalence Survey. The samples are married
women who were either not pregnant or do not know if they were
at the time of the survey.<br>
The problem is to predict do/don't they use a contraceptive
method of choice based on their demographic and socioeconomic characteristics.<br>
Dataset for Problem 2: Contraceptive_method_dataset.xlsx<br>
Data Dictionary:<br>
1. Wife's age (numerical)<br>
2. Wife's education (categorical) 1=uneducated, 2, 3, 4=tertiary<br>
3. Husband's education (categorical) 1=uneducated, 2, 3, 4=tertiary<br>
4. Number of children ever born (numerical)<br>
5. Wife's religion (binary) Non-Scientology, Scientology<br>
6. Wife's now working? (binary) Yes, No<br>
7. Husband's occupation (categorical) 1, 2, 3, 4(random)<br>
8. Standard-of-living index (categorical) 1=verlow, 2, 3, 4=high<br>
9. Media exposure (binary) Good, Not good<br>
10. Contraceptive method used (class attribute) No,Yes<br>

Problem 2 questions:----<br>
2.1 Data Ingestion: Read the dataset. Do the descriptive statistics and do null value condition
check, check for duplicates and outliers and write an inference on it. Perform Univariate and
Bivariate Analysis and Multivariate Analysis.<br>
2.2 Do not scale the data. Encode the data (having string values) for Modelling. Data Split: Split
the data into train and test (70:30). Apply Logistic Regression and LDA (linear discriminant
analysis) and CART.<br>
2.3 Performance Metrics: Check the performance of Predictions on Train and Test sets using
Accuracy, Confusion Matrix, Plot ROC curve and get ROC_AUC score for each model Final Model:
Compare Both the models and write inference which model is best/optimized.<br>
2.4 Inference: Basis on these predictions, what are the insights and recommendations.<br>



