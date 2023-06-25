# Cultural Differences and Similarities in Perceptions of Artificial Social Agents (ASAs) - Dutch version
## Question 1

**Author**:  Johan Hensman **Date**: June 2023
**Contributors**: Johan Hensman, Nele Albers, Willem-Paul Brinkman
**Code based on the code from:** Fengxiang Li

This file is meant to guide you through reproducing our results for calculating the ICC values on an item-level and construct-level basis and for the short version of the questionnaire.

### Explanation of What is Done
Prior to this analysis, we have done 2 translation rounds of the English ASA Questionnaire. In the first round, we had 37 Dutch items that had a low correlation value with their corresponding first English Item. These got new translations and the correlation values were again calculated. In this analysis we combined the best translation together resulting in a list of items with the highest ICC (Intra Course Correlation) value. The ICC was calculated again to confirm the list was correct. 

The Construct level ICC is also calculated. The ICC can only be calculated if the whole construct is rated by 1 participant. For this reason, almost all values are from Round 1 (including the low values) and 1 construct from Round 2 (construct 17 Interaction Impact on Self-Image). For the short version of the ASA, the representing 24 items were chosen and their ICC has also been calculated.


### Requirements
You need to have R v4.2.3 installed. Rstudio is recommended to view and execute the files. All dependencies are listed in the RMD files

### Steps to Reproduce Analysis
1)	Make sure R is installed.
2)	Navigate to the folder where this README is located.
3)	Open the file Final_assessment_Q1.Rmd to start running the code
4)	Make sure all dependencies are downloaded
5)	Run the content of the selected files. It accesses the data files: Final_ASA_Dutch_Round_1_First_Half_anonym.sav, Final_ASA_Dutch_Round_1_Second_Half_anonym.sav and Final_ASA_Dutch_Round_2_anonym.sav. 
6)	Once run the program outputs the ICC values, their classification, mean, standard deviation and range for item-level construct-level and the short version of the ASA. 
7)	If you want to knit a pdf-file from the RMD-file, you can use the knit button in RStudio.

### Explanation of Files
•	README.md/README.pdf : This README-file
•	Final_ASA_Dutch_Round_1_First_Half_anonym.sav: Data from the first half of the survey used to compute the ICC values
•	Final_ASA_Dutch_Round_1_Second_Half_anonym.sav: Data from the second half of the survey used to compute the ICC values
•	Final_ASA_Dutch_Round_2_anonym.sav: Data from the 2nd round to compute the ICC values
•	Final_assessment_Q1.Rmd: Code to reproduce to obtain the ICC values 
•	Legend Q1.txt: Explanation of all columns in the three datafiles (Final_ASA_Dutch_Round_1_First_Half_anonym.sav, Final_ASA_Dutch_Round_1_Second_Half_anonym.sav and Final_ASA_Dutch_Round_2_anonym.sav ). 
•	Final_assessment_Q1.pdf: The knitted file of Final_assessment_Q1.Rmd
•	Header.tex: Latex file to create the table of contents at the head of the PDF file
•	Best_ICC_and_translations.xlsx: List of the chosen translation with their corresponding ICC values. 
