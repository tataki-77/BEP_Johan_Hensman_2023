# Cultural Differences and Similarities in Perceptions of Artificial Social Agents (ASAs) - Dutch version
## Overview of the Steps to Reproduce Analysis

**Author**:  Johan Hensman **Date**: June 2023
**Contributors**: Johan Hensman, Nele Albers, Willem-Paul Brinkman
**Code based on the code from:** Fengxiang Li

This file is meant to give an overview of reproducing our analyses. All code is based on Fenqxiang Li and adaptation to the Dutch survey has been written by the author Johan Hensman. Legends and other files have been written by Johan Hensman. 


### Type of analysis
We describe how you can reproduce our results for the analyses in the folders of this section. The analyses include ICC calculation for question 1 of the final assessment, mean differences between the English and Dutch items for question 2 and construct/dimension differences for question 3 of the final assessment.



### Folder Structure
Each folder roughly contains the same items, in the ‘Question 3’ folder there are 2 .Rmd files as the data pre-processing and the actual calculation is split as for the other folders they are combined in 1 Rmd file. The rest of the structure:
•	README.md/README.pdf: This file shows you how to reproduce the results of the particular question in the final assessment
•	Survey results are saved in a .sav file for the Dutch data or .xlsx file for the Chinese data
•	Header.tex: this file creates the header in the knitted files
•	An analysis file (.Rmd) where the analysis of the corresponding question is performed
•	A knitted file of the analysis file to show the results.



