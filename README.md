## TEIS Outcomes Calculation

[The Tennessee Early Intervention System (TEIS)](https://www.tn.gov/disability-and-aging/disability-aging-programs/teis.html) is a program program that offers therapy and other services to families of infants and young children with developmental delays or disabilities. 

TEIS is required to report outcomes data annually on children who exited early intervention services and received a minimum of 6 months of service. This is based on the first (entrance) assessment and last (exit) assessment. For the 2023-24 data, every exit assessment used the BDI-3, but there were three possible entrance assessments.

Your first objective in this project is to compare two sets of business rules for calculating Early Childhood Outcome (ECO). For more information on the sets of business rules, see the "TEIS Data Project" document. 

You can see the calculations for the original business rules in the ECO Data spreadsheet. Your first objective is to redo the calculations for children with either the BDI-2 or BDI-3 as the entrance assessment. See the new business rules in the TEIS Data Project document.

Your second objective is to investigate children who did not improve functioning (progress category a) and report demographic qualities of these children, including
* Point of Entry office (POE)
    - See the TEIS Acronyms and Terms document for the full for each POE
* Length of time in services
* Length between assessment and exit
* Length between entrance and exit assessments
* Difference between extrance and exit assessment instruments
* Age at assessment/exit

#### Data Overview

You've been provided several data files.

* NSS_ECO Data Ind 3 FFY 2023-24 20241211.xlsx: Contains the original data source for the 2023-24 TEIS ECO data
* NSS data_BDI3 Scores 20230101 20240630_Compiled20241107.xlsx: Contains raw BDI-3 data for recalculating outcomes data
* NSS data_BDI2_scores_20200101-20230131_20241106.csv: Contains raw BDI-2 data for recalculating outcomes data

In addition, there are a few additional documents for reference:

* TEIS Data Project – Jan. 2025.docx: Provides an overview of the project and outcome data. 
* BDI scoring resource.docx: Provides an explanation of scores on the BDI-3
* BDI3_ScoreReport Sample.pdf: A sample of BDI-3 Score Report used for training
* TEIS Acronyms and Terms.pdf: A resource document providing abbreviations commonly found in TEIS

----Child id= 542339

Philip Schingle
  1:02 PM
A quick update for clarity's sake:  I reached out to Shannon to get some clarification on some of the confusion and she got back to me with some answers
.
Good afternoon Shannon,
	This is Philip Schingle, we spoke a bit yesterday at the NSS zoom meeting and I wanted to touch base with you as we have a few questions if you don’t mind.
Just for clarity sake, The goal for question one is to use the new business rule to recalculate ECO data for children with BDI entrance and exit for 2023-24 to see how it would have impacted the reporting. Where the new business rule is to use the progress category i.e. the DQ scores sub domain scores as opposed to the 1-7 ratings used in the old business rule.
 Shannon's answer-Yes. This is correct.
Here are the new business rules for determining progress categories using DQ scores (these are found in the PowerPoint and in the Word document). A DQ of above/below 78 in a domain simply determines if a child is functioning compared to their typically developing peers on a BDI. Since our program serves children with disabilities and delays, we often see scores below 78. The sub-domains will be helpful to determine which progress category is most appropriate.

BDI to BDI Progress Category calculations:
The exit DQ is less than 78 and all exit raw subdomain scores are less than or equal to entry raw subdomain scores
The exit DQ is less than 78 and less than or equal to entry DQ and one or more exit raw subdomain scores are greater than the entry raw subdomain score
The exit DQ is less than 78 and greater than entry DQ and one or more exit raw subdomain scores are greater than the entry raw subdomain score
The entry DQ is less than 78 and the exit DQ is greater or equal to 78 Or The entry DQ greater than or equal to 78 and exit DQ greater than or equal to 78 and at least one entry subdomain Z-score of -1.50 or Less.
The entry and exit DQs are greater than or equal to 78
If you could CC Jennifer on this reply as we will probably have questions going forward about other aspects of the data as we are trying to recalculate with the new business rule.
Done.
Thank you so much as we are excited to get working on this project for TEIS! (edited) 

-----------------

Okay, round two for our questions have been answered: Good morning,
After digging into the data a bit more we have a few more questions. Some of these may cover some of the same ground as they were compiled from our different work groups.

Q. Are there any kids present in BDI2/BDI3 worksheets that aren't present in ECO worksheet? Or is ECO worksheet a consolidation/summary of the BDI2 and BDI3 worksheets?

Yes. The BDI-2 and BDI-3 workbooks include all of the children with assessments. The ECO workbook specifically includes children we are required to report on for the 2023-24 fiscal year (those who exited or turned 3).

Q. Are ECO entry/exit dates different than entry/exit dates in BDI2/BDI3?

Yes. ECO entry/exit dates are the child’s initial IFSP date and the child’s official exit date from TEIS. The dates on the BDI-2/BDI-3 are the dates that assessment was completed by an evaluator, which may be before or after the ECO dates.

Q. Is there any duplicate data?

A child may have been assessed multiple times but the dates should be different. The ECO data file should not have duplicates with the Child ID being a unique identifier.
If a kid has an assessment at 3 and then stays in TEIS, do we count both the assessment at age 3 and the assessment at exit, or only the exit assessment?
Count the last assessment

Q. What are the instruments referred to in "Difference between entrance and exit assessment instruments"? Does this refer to the method used for assessment? AEPS/BDI-2/BDI-3 or something else?
Yes, this refers to the methods used

Q. Which entry date do we choose if a child has BDI-2 and BDI-3 entry dates? The earliest date?

For ECO, the entry date would be the initial IFSP date. You would select the BDI-2 or BDI-3 that was completed prior to the initial IFSP. If more than one was completed prior to initial IFSP, you would select the one most recently completed prior to the initial IFSP.

Q. Should we be considering only the kids with both entry and exit dates?
Children in the extended option will not have an exit date (from TEIS). However, if the question is about entry and exit ECO dates (using the ECO dataset), if a child had missing ECO data, we would not anticipate you being able to find it in the records we provided.

Q. Which child ID do we use to map children in the diff datasets?
TEIDS ID

Final note: We found kids that had entry exams for both bdi2 and bdi3 (for example row 1869) and it's part of why there is confusion. Thank you so much!
This child’s initial IFSP date (column X) is 5/9/22, so you would look for an evaluation completed on/before 5/9/22 as your entrance. The BDI-2 was completed 3/1/22, so it is the entrance rating. The child exited (column Z) on 4/3/24, so we would look for the last assessment, which will always be a BDI-3. In this case, the one completed 2/9/24.
I think in the ECO file we were pulling over all possible data sources for children, so maybe think of the “BDI-3 entrance” headers as the earliest record of that assessment being completed.


 
ECO_Entry_DATE   -D
ECO_Exit_DATE    - H
Initial IFSP Date    X
"Exit Date 
Or end of FY"      -- Z
"TEIDS
ECO_Entry_DATE"	-- cf
"AEPSi
ECO_Entry_DATE"    -CU

"AEPS 202223.2
Entry only data
Entry date"      --DF

"BDI 3
ECO_Entry_DATE" 	- DL 

 "BDI 3
ECO_Exit_DATE"		- DW 
  
BDI2 Entry Date   -- EL


 


