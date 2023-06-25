# Cultural Differences and Similarities in Perceptions of Artificial Social Agents (ASAs) - Dutch version
## Question 3

**Author**:  Johan Hensman **Date**: June 2023
**Contributors**: Johan Hensman, Nele Albers, Willem-Paul Brinkman
**Code based on the code from:** Fengxiang Li

This file is meant to guide you through reproducing our results for calculating construct/dimension differences between the Dutch and the Chinese speakers.

### Explanation of What is Done
Prior to this analysis, we have done 2 translation rounds of the English ASA Questionnaire. In the first round, we had 37 Dutch items that had a low correlation value with their corresponding first English Item. These got new translations and the correlation values were again calculated. In the analysis we combined the best translation together resulting in a list of items with the highest ICC (Intra Course Correlation) value. The ICC was calculated again in the analysis of question 1 to confirm the list was correct. 

In this analysis, the construct/dimension differences are calculated to show the differences and similarities between the Dutch and Chinese speakers. This was calculated by using a multi-level linear regression model. Before this was possible the data had to be transformed and pre-processed, which is explained in the Transform_raw_data.pdf/.RMD.



### Requirements
You need to have R v4.2.3 installed. Rstudio is recommended to view and execute the files. All dependencies are listed in the RMD files

### Steps to Reproduce Analysis
1)	Make sure R is installed.
2)	Navigate to the folder where this README is located.
3)	Open the file Transform_raw_data.Rmd to start running the code
4)	Make sure all dependencies are downloaded
5)	Run the content of the selected files. It accesses the data files: Final_ASA_Dutch_Round_1_First_Half_anonym.sav, Final_ASA_Dutch_Round_1_Second_Half_anonym.sav,
ASA_Chinese_Round1_Part1.xlsx and ASA_Chinese_Round1_Part2.xlsx. 
6)	Once run, the program (over)writes the file data_cultures.sav to the folder with the data for the construct/dimension difference analysis.
7)	Open the file Final_assessment_Q3.Rmd to start running the code
8)	Make sure all dependencies are downloaded
9)	Run the content of the selected file. It accesses the data file: data_cultures.sav
10)	Once run, the program outputs the means of Dutch and Chinese speakers, the mean and standard deviation differences of both groups and the credibility interval of the mean differences



### Explanation of Files
•	README.md/README.pdf : This README-file
•	Final_ASA_Dutch_Round_1_First_Half_anonym.sav: Data from the first half of the Dutch  survey used to compute the ICC values
•	Final_ASA_Dutch_Round_1_Second_Half_anonym.sav: Data from the second half of the Dutch survey used to compute the ICC values
•	ASA_Chinese_Round1_Part1.xlsx: Data from the first half of the first round of the Chinese study to compute the ICC values
•	ASA_Chinese_Round1_Part2.xlsx: Data from the second half of the first round of the Chinese study to compute the ICC values
•	Transform_raw_data.Rmd: Code to obtain the datafile used to compute the construct/dimension scores
•	Final_assessment_Q3.Rmd: Code to reproduce the construct/dimension scores
•	Legend Q2.txt: Explanation of all columns of the two datafiles (Final_ASA_Dutch_Round_1_First_Half_anonym.sav, Final_ASA_Dutch_Round_1_Second_Half_anonym.sav) 
•	Transform_raw_data.pdf: The knitted file of Transform_raw_data.Rmd Final_assessment_Q3.pdf: The knitted file of Final_assessment_Q3.Rmd
•	Header.tex: Latex file to create the table of contents at the head of the PDF file
•	data_cultures.sav: Datafile containing all construct scores of each participant in a long format


