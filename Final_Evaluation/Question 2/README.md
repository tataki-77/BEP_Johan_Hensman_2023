# Cultural Differences and Similarities in Perceptions of Artificial Social Agents (ASAs) - Dutch version
## Question 2

**Author**:  Johan Hensman **Date**: June 2023
**Contributors**: Johan Hensman, Nele Albers, Willem-Paul Brinkman
**Code based on the code from:** Fengxiang Li

This file is meant to guide you through reproducing our results for calculating the mean differences between the English and the Dutch questionnaire items on an item-level and construct-level and for the short version of the questionnaire with the Bayesian paired t-test.

### Explanation of What is Done
Prior to this analysis, we have done 2 translation rounds of the English ASA Questionnaire. In the first round, we had 37 Dutch items that had a low correlation value with their corresponding first English Item. These got new translations and the correlation values were again calculated. In the analysis we combined the best translation together resulting in a list of items with the highest ICC (Intra Course Correlation) value. The ICC was calculated again in the analysis of question 1 to confirm the list was correct. 

In this analysis, the variation between the Dutch and the English questionnaire is calculated. This is done with the calculations of the Bayesian t-test, which outputs a 95% credibility interval of the mean differences between the 2 groups. If this interval doesn’t contain 0, we can speak of bias. This has been done on item-level, construct-level and for the short ASA questionnaire.


### Requirements
You need to have R v4.2.3 installed. Rstudio is recommended to view and execute the files. All dependencies are listed in the RMD files

### Steps to Reproduce Analysis
1)	Make sure R is installed.
2)	Navigate to the folder where this README is located.
3)	Open the file Final_assessment_Q2.Rmd to start running the code
4)	Make sure all dependencies are downloaded
5)	Run the content of the selected files. It accesses the data files: Final_ASA_Dutch_Round_1_First_Half_anonym.sav, Final_ASA_Dutch_Round_1_Second_Half_anonym.sav and Final_ASA_Dutch_Round_2_anonym.sav. 
6)	Once run the program outputs the means and the standard deviations of English and Dutch items, the mean and standard deviation differences of both groups and the 95% credibility interval for item-level and construct-level and for the short version of the questionnaire.
7)	If you want to knit a pdf-file from the RMD-file, you can use the knit button in RStudio.


### Explanation of Files
•	README.md/README.pdf : This README-file
•	Final_ASA_Dutch_Round_1_First_Half_anonym.sav: Data from the first half of the survey used to compute the ICC values
•	Final_ASA_Dutch_Round_1_Second_Half_anonym.sav: Data from the second half of the survey used to compute the ICC values
•	Final_ASA_Dutch_Round_2_anonym.sav: Data from the 2nd round to compute the ICC values
•	Final_assessment_Q2.Rmd: Code to reproduce to obtain the mean differences
•	Legend Q2.txt: Explanation of all columns in the three datafiles (Final_ASA_Dutch_Round_1_First_Half_anonym.sav, Final_ASA_Dutch_Round_1_Second_Half_anonym.sav and Final_ASA_Dutch_Round_2_anonym.sav ). 
•	Final_assessment_Q1.pdf: The knitted file of ICC_Round_1_All_Data.Rmd
•	Header.tex: Latex file to create the table of contents at the head of the PDF file

